FROM nginx:alpine

RUN rm -rf /usr/share/nginx/html/*

# main folder ke andar ka saara content seedhe web root me copy karein
COPY main/ /usr/share/nginx/html/

# Config file replace karein
COPY main/google-store.conf /etc/nginx/conf.d/default.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]