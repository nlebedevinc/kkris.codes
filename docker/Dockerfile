FROM node:14 as base

LABEL maintainer="nickllebedev<nlebedevme@gmail.com>"

ARG NODE_ENV
ENV NODE_ENV "${NODE_ENV}}"

WORKDIR /app

# deps stage
FROM base AS dependencies
COPY package.json package-lock.json /app/
RUN npm ci

# build stage
FROM base AS release
COPY --from=dependencies /app/node_modules ./node_modules
COPY package.json package-lock.json nuxt.config.ts tsconfig.json /app/
COPY ./src/ /app/src
RUN npm run build

# start container
CMD ["npm", "run", "start"]
