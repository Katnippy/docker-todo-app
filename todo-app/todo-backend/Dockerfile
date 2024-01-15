FROM node:20.11.0-bookworm-slim

WORKDIR /usr/src/app

COPY --chown=node:node . .
RUN npm ci --only=production

ENV DEBUG=todo-backend:*

USER node
CMD npm start

