# 1. Official lightweight Nginx image
FROM nginx:alpine

# 2. Default static files remove karein
RUN rm -rf /usr/share/nginx/html/*

# 3. Frontend ka saara content Nginx web directory me copy karein
COPY . /usr/share/nginx/html/

# 4. Custom Nginx configuration file apply karein
COPY main/google-store.conf /etc/nginx/conf.d/default.conf

# 5. Web traffic port expose karein
EXPOSE 80

# 6. Start Nginx
CMD ["nginx", "-g", "daemon off;"]