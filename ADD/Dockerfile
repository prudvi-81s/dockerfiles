FROM almalinux:9
RUN dnf install nginx -y 
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/prudvi-81s/expense-infra-dev/refs/heads/main/60-backend/data.tf /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]