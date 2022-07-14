
FROM nginx:latest
RUN apt update -y && apt upgrade -y && apt autoremove -y && apt clean && rm -rf /var/lib/apt/lists/*
RUN rm -f /usr/share/nginx/html/index.html
WORKDIR /usr/share/nginx/html
COPY ./web/index.html .
RUN date >> index.html
