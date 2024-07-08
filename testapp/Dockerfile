FROM node:latest

WORKDIR  ./testapp

COPY package*.json /testapp/

RUN npm install

COPY . .

RUN npm run build

CMD [ "npm","start" ]

#COPY --from=installer /testapp/build /usr/share/react/html