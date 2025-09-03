# استخدم صورة Nginx خفيفة
FROM nginx:alpine

# احذف default page
RUN rm /usr/share/nginx/html/*

# انسخ ملفات اللعبة إلى مجلد Nginx
COPY . /usr/share/nginx/html

# افتح البورت 80
EXPOSE 80

# شغل Nginx في foreground
CMD ["nginx", "-g", "daemon off;"]
