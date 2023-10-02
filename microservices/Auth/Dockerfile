FROM node:20-alpine3.17

# Create app directory

RUN apk add --no-cache git
RUN git clone https://github.com/NightBase/Authentication-Service

WORKDIR /Authentication-Service

RUN npm install
RUN npm run build

# Run production
CMD ["npm", "run", "start:prod"]
