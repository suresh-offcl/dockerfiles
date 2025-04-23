FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://github.com/daws-81s/expense-infra-dev/blob/main/readme.MD /usr/share/nginx/html/index.html
RUN chmod +x /usr/share/nginx/html/index.html
ADD sample-1 /tmp/
RUN chmod +r /tmp/

CMD ["nginx","-g","daemon off;"]