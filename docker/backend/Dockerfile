FROM eclipse-temurin:17-jdk-jammy

WORKDIR /app

RUN apt-get update && apt-get install -y git wget

RUN git clone https://github.com/Vishal-seehra/Restaurant-Booking-Management-Application.git

WORKDIR /app/Restaurant-Booking-Management-Application

RUN wget https://repo1.maven.org/maven2/mysql/mysql-connector-j/8.4.0/mysql-connector-j-8.4.0.jar

RUN javac -cp .:mysql-connector-j-8.4.0.jar Main.java

EXPOSE 5000

CMD ["java", "-cp", ".:mysql-connector-j-8.4.0.jar", "Main"]
