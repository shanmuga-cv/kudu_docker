run: clean_container build
	docker-compose up -d --scale tserver=2

build:
	docker-compose build

clean_container:
	docker-compose down
