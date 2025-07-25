FROM nginx:1.25-alpine

# Копируем дефолтный конфиг (можно заменить позже)
COPY default.conf /etc/nginx/conf.d/default.conf

# Оставляем контейнер в интерактивном режиме
CMD ["nginx", "-g", "daemon off;"] 