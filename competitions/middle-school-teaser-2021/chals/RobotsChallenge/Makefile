build:
<<<<<<< Updated upstream
	@docker build . -t robots_txt-377546445
=======
	@docker build  --platform linux/amd64 . -t robots_txt-8739167580398 -q
>>>>>>> Stashed changes

run: build
	@docker run -p 8080:80 robots_txt-377546445

clean:
	@docker rm -f -v robots_txt-377546445

generate-img:
	@docker run -d --name robots_txt-377546445 robots_txt-377546445:latest
	@docker export robots_txt-377546445 -o vm.tar.gz
	@docker rm robots_txt-377546445
	@docker rmi robots_txt-377546445