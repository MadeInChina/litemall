FROM registry.homelab.org/node:12.13.0-slim

# Create app directory
WORKDIR /usr/src/app/

# Install app dependencies
ADD . ./

RUN npm install -g cnpm --registry=https://registry.npm.taobao.org

RUN cnpm install

EXPOSE 9527

CMD cnpm run dev
