FROM node
WORKDIR /usr/src/app
COPY example-frontend* ./
EXPOSE 5000
RUN curl -sL https://deb.nodesource.com/setup_16.x | bash
RUN apt install -y nodejs
RUN npm update
RUN npm install
RUN npm audit fix --force
RUN REACT_APP_BACKEND_URL=http://localhost:8080 npm run build
RUN npm install -g serve



ENTRYPOINT ["npm","start"]
