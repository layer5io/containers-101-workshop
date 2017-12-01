FROM nginx:latest

COPY index.html /usr/share/nginx/html
COPY linux.svg /usr/share/nginx/html
COPY swlogo.svg /usr/share/nginx/html

EXPOSE 80 443 	

CMD ["nginx", "-g", "daemon off;"]
