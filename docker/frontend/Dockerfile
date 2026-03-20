FROM nginx:latest

RUN apt-get update && apt-get install -y git

RUN git clone https://github.com/Vishal-seehra/Restaurant-Booking-Management-Application.git

RUN rm -rf /usr/share/nginx/html/*

RUN cp Restaurant-Booking-Management-Application/*.html /usr/share/nginx/html/
RUN cp -r Restaurant-Booking-Management-Application/Images /usr/share/nginx/html/

EXPOSE 80
