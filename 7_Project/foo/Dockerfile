FROM node:9-alpine
WORKDIR /app
COPY package.json yarn.lock ./
RUN yarn
COPY . ./
RUN yarn build --production

RUN yarn global add serve
CMD serve -s build

EXPOSE 5000