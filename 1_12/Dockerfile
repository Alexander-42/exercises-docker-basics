FROM ubuntu:latest

WORKDIR /usr/src/app

COPY . .

RUN apt-get update && \
    apt-get install -y curl ca-certificates && \
    curl -sL https://deb.nodesource.com/setup_16.x | bash - && \
    apt-get install -y nodejs && \
    node --version && \
    npm --version

RUN npm install

RUN npm run build

RUN npm install -g serve

CMD ["serve", "-s", "build", "-l", "5001"]
