# Nginx Headers
>_Sample nginx.conf content._

```
 add_header Server "";
 
   server {
 
     listen 80;
     listen [::]:80;
 
     server_name $IP_ADDRESS;
 
     root /usr/share/nginx/html/project_folder;
     index index.tsx;
 
     location /{
        proxy_pass http://localhost:3000;
        proxy_pass_header Server;
        proxy_set_header Host 192.168.227.104;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection "upgrade";
        proxy_hide_header X-Powered-By;
        proxy_hide_header Server;
        add_header Content-Security-Policy "default-src 'self' data:; font-src 'self' https://kit.fontawesome.com https://fonts.gstatic.com https://fonts.googleapis.com/ https://fonts.googleapis.com https://fonts.google.com https://fontawesome.com https://kit-pro.fontawesome.com ; style-src 'self' https://*.googleapis.com 'unsafe-inline' 'strict-dynamic'; script-src 'self' 'unsafe-eval' 'strict-dynamic'; object-src 'self'; img-src 'self' data:; base-uri 'self'; form-action 'self';";
        add_header X-Frame-Options "DENY";
        add_header Cache-Control "s-maxage=86400";
        add_header X-Content-Type-Options 'nosniff';
        }
    }
```
