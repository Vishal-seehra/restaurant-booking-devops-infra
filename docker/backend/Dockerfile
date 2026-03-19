FROM openjdk:17

WORKDIR /app

RUN apt-get update && apt-get install -y git

RUN git clone https://github.com/Vishal-seehra/Restaurant-Booking-Management-Application.git

WORKDIR /app/Restaurant-Booking-Management-Application


RUN javac Main.java

EXPOSE 5000

CMD ["java", "Main"]
