(Based in large part on https://github.com/FaztWeb/crud-mean-angular5)

### Instructions

install mongo (https://docs.mongodb.com/manual/installation/)

`mongod`

in another tab `git clone https://github.com/mark-mcdermott/mean-crud.git`

`cd mean-crud`

`npm install`

`node api-server`

in another tab, `ng serve`

go to localhost:4200

the app should be working now, but not Auth0 yet

to get Auth0 working, get an Auth0 account https://auth0.com/

create an Auth0 client

in the Auth0 client settings get your clientID, domain.

in the Auth0 client settings set a callback url to <yourdomain.com>/callback

in /src/app/auth-vars/ rename auth0-variables.ts.example to auth0-variables.ts

follow the instructions in auth0-variables.ts to add your clientID, domain & callback url in there

upload the app to your server (Auth0 doesn't work on localhost sometimes)

run mongod and ng serve as separate processes again

Auth0 should be working now, too.
