FROM node:10-alpine
WORKDIR /app
COPY . .
RUN yarn install --production
VOLUME [ "/etc/todos" ]
CMD ["node", "/app/src/index.js"]
# docker run -p 3000:3000 -v todo-db:/etc/todos todoapp