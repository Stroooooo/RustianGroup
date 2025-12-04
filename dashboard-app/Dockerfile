FROM node:20-alpine AS deps
WORKDIR /app

COPY ./ ./
RUN rm -rf node_modules package-lock.json

RUN npm i --force

EXPOSE 3000

ENV PORT=3000
ENV HOSTNAME="0.0.0.0"

CMD ["npm", "run", "dev"]