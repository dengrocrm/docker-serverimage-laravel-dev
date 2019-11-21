# DenGro Docker Server Image for Laravel Development and Testing

This is the repo for the Docker image used for development and testing, including CI/CD. It is built on `dengrocrm/docker-serverimage-laravel`.

# Running

Note that this image does not contain any application code. Run the following command to run and `exec` an interactive bash shell:

	docker exec -it dengrocrm/serverimage-laraveldev:latest /bin/bash

# Building and publishing

**Images are built automatically when pushed to Github, the following is here for reference purposes.**

Build the image by run the following command:

	docker build --tag dengrocrm/serverimage-laraveldev:latest .
	docker push dengrocrm/serverimage-laraveldev:latest

Note that `--tag` is rquired in order to publish the image.