FROM openjdk:8
COPY . /app
WORKDIR /app
RUN ["javac" ,"Main.java"]
ENTRYPOINT ["java","Main"]