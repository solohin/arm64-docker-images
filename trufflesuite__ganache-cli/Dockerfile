FROM node:18

# ganache version
ARG VERSION
ENV VERSION=$VERSION

RUN npm install ganache@$VERSION -g

ENTRYPOINT ["ganache"]
