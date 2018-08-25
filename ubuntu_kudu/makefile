run: clean_container build
	docker run  -i -t -p 8050:8050 -p 7050:7050 -p 8051:8051 -p 7051:7051 --name kudu_ubuntu kudu_ubuntu_img

build:
	docker build -f Dockerfile_ubuntu -t kudu_ubuntu_img .

clean_container:
	docker container rm kudu_ubuntu