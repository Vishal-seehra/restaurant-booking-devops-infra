FROM eclipse-temurin:17-jdk-jammy

WORKDIR /app

RUN apt-get update && apt-get install -y git

RUN git clone https://github.com/Vishal-seehra/Restaurant-Booking-Management-Application.git

WORKDIR /app/Restaurant-Booking-Management-Application

RUN find . -name "*.class" -delete

RUN javac $(find . -name "*.java")

EXPOSE 5000

CMD ["java", "Main"]
