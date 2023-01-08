#Выбор базового образа
FROM nginx:alpine
#Копирование html-страницы
COPY index.html /usr/share/nginx/html/
#Удаление дефолтного файла конфигурации
RUN rm /etc/nginx/conf.d/default.conf
#Копирование файла конфигурации
COPY nginx.conf /etc/nginx/conf.d/
#Команда для запуска в контейнере
CMD ["nginx", "-g", "daemon off;"]