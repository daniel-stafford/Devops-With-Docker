FROM ubuntu
WORKDIR /app
RUN apt-get update && apt-get install -y curl
COPY script.sh .
CMD [ "bash", "./script.sh" ]
