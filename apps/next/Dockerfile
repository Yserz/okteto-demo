FROM node:16-alpine
COPY apps/next/.next/ .
RUN yarn --frozen-lockfile --production

CMD yarn start