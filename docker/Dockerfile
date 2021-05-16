FROM node:14 as base

WORKDIR /app

ENV HOST=0.0.0.0

# deps stage
FROM base AS dependencies
COPY package.json package-lock.json /app/
RUN npm ci

# build stage
FROM base AS build
COPY --from=dependencies /app/node_modules ./node_modules
COPY package.json package-lock.json nuxt.config.ts tsconfig.json /app/
COPY ./src/ /app/src
RUN npm run build

# release stage
FROM base AS release
COPY --from=dependencies /app/node_modules ./node_modules
COPY --from=build /app/.nuxt ./.nuxt
COPY package.json package-lock.json /app/

# start container
CMD ["npm", "run", "start"]
