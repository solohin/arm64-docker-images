VERSION = 7.5.0

dev: build
	docker build -t solohin/ganache:${VERSION} .
	docker run --rm -it solohin/ganache:${VERSION} --accounts 1 --seed 123456789

build: 
	docker build --build-arg VERSION=${VERSION} -t solohin/ganache:${VERSION} .

push: build
	docker push solohin/ganache:${VERSION}
	docker tag solohin/ganache:${VERSION} solohin/ganache:latest
	docker push solohin/ganache:latest