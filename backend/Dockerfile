FROM openjdk:17
WORKDIR /app
COPY . .
RUN chmod u+x mvnw
RUN ./mvnw clean package
RUN mv target/*.jar app.jar
EXPOSE 8080
CMD ["java", "-jar", "app.jar"]