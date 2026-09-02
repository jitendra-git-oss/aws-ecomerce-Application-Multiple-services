# 1. Official lightweight Nginx image
FROM nginx:alpine

# 2. Default static files remove karein
RUN rm -rf /usr/share/nginx/html/*

# 3. 'main' folder ke andar ka content seedha web root me copy karein
COPY main/ /usr/share/nginx/html/

# 4. Custom Nginx configuration file apply karein
COPY main/google-store.conf /etc/nginx/conf.d/default.conf

# 5. Web traffic port expose karein
EXPOSE 80

# 6. Start Nginx
CMD ["nginx", "-g", "daemon off;"]