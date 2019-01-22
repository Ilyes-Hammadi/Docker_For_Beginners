CURRENT_DIR=$(shell pwd)
IMAGE=docker.io/ilyeshammadi/foo
VERSION=latest

# Start local development
start:
	docker run \
	--expose 3000 \
	-p 3000:3000 \
	-it \
	-v ${CURRENT_DIR}:/app \
	-w /app \
	node:9 npm start

build:
	docker build -t ${IMAGE}:${VERSION} .

push: build
	docker push ${IMAGE}:${VERSION}
	