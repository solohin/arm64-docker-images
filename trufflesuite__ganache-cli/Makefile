GANACHE_VERSION = 7.5.0

dev:#linux/arm64/v8,
	docker buildx build --platform=linux/amd64,linux/arm64/v8 --build-arg GANACHE_VERSION=${GANACHE_VERSION} --push --tag ghcr.io/solohin/arm64-docker-images:${GANACHE_VERSION} .
