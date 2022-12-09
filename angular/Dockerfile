# base image
FROM node:14.20

# set working directory
#RUN mkdir /proch/git/project/angular
WORKDIR C:/Users/proch/git/project/angular

# add `/usr/src/app/node_modules/.bin` to $PATH
ENV PATH proch/git/project/angular/node_modules/.bin:$PATH

# install and cache app dependencies
COPY package.json proch/git/project/angular/package.json
RUN npm install

# add app
COPY . proch/git/project/angular

EXPOSE 4200

# start app
CMD ng serve --host 0.0.0.0 --port 4200