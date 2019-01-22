
PATH_TO_PROJECT="/Users/ilyes/YouTube_Tutorials/Docker_For_Beginners/5_Volumes/whats_your_age"

sandbox:
	@docker run \
	-v ${PATH_TO_PROJECT}:/app \
	-it \
	gcc /bin/bash

run: compile
	@./myapp

compile:
	@gcc -o myapp main.c 