FROM python:3-alpine

COPY ./index.html /app/index.html

WORKDIR /app

CMD [ "python3", "-m",  "http.server"]

EXPOSE 8000