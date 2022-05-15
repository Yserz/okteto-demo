FROM node:16-alpine as builder
COPY ./ .
RUN yarn --frozen-lockfile
RUN yarn build

FROM node:16-alpine
COPY --from=builder ./.next .
RUN yarn --frozen-lockfile --production
CMD yarn start