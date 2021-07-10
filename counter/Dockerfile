FROM node:12-alpine

# Build
COPY ./package* /app/
WORKDIR /app
RUN npm install

COPY . /app/

# Using Tiny Process
RUN        apk add --no-cache tini
ENTRYPOINT ["/sbin/tini", "--"]

# Run
EXPOSE 3000
CMD ["node", "app.js"]