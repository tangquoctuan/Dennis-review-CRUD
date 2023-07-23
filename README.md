# Dennis-review-CRUD
- Using ignored file config to avoid un-necessary file. Especially node_module (Refer: Why_you don't have to commit node modules folder :
DEV Community)
- Need add README.md file to demonstrate main content, how to run/start project as well.
- Setup up start command in package.json to make project can run/start easy
"""
"scripts": {
"test": "echo\ "Error: notestspecified\" &6 exiti"
"start": "node app"
// or "start": "nodemon app"
"""
- Need to naming unique endpoint.
    https://github.com/DennisChin 1022/CRUD-refactor/blob/1d6dd5643c2a03689ddd94957129ae243750be5/routes/retailer.route.js/L8
    https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643c2a03689ddd94957129ae243750be5/routes/admin.route.js#L131
- Using general error message in login process - (ex: Login info not correct)
    https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643cb2a03689ddd94957129ae243750be5/utils/passport.auth.js#L24
    https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643cb2a03689ddd94957129ae243750be5/utils/passport.auth.js#L17
- Provide docker-compose file to help the data server preparation steps be quick (ex below). Need to install docker on your local machine before run script below.
'''
# docker-compose. yml
version: '3.1' #format version for this docker compose file services:
mongo-container:
image: mongo: latest environment:
- MONGO_INITDB_ROOT_USERNAME=admin
- MONGO INITOR ROOT PAsswORDsadmin
# !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
# Here you are setting the username and password
" so chance it to whatever vou want
!!!!!!!!!!!!!!!!!
DOrTS:
- "27017:27017"
commanor mongod
'''
- Using required prop in HTML input tag for mandary input
- Cause UserSchema is use required validators for: name, phone, email, password login.ejs
    https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643cb2a03689ddd94957129a243750be5/views/login.eis#L6
    https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643c2a03689ddd94957129ae243750be5/views/login.eis#L10
    profile.ejs
        https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643c2a03689ddd94957129ae243750be5/views/profile.eis#118
    register-customer.es
        https://github.com/DennisChin1022/CR
refactor/blob/1 d6d5643cb2a03689ddd94957129ae243750be5/views/register-
customer.ejs#Li
        https://github.com/DennisChin10221
factor/blob/1 d6d5643cb2a03689ddd94957129ae243750be5/views/register-
    customer.eis#L15
        https://github.com/DennisChin1022/CR
-refactor/blob/1d6dd5643cb2a03689ddd94957129ae243750be5/views/register-
customer.eis#L40
        https://github.com/DennisChin1022/CR
D-refactor/blob/1d6dd5643cb2a03689ddd94957129a243750be5/views/register-
customer.e|s#_44
    register-retailer.ejs
        https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643cb2a03689ddd94957129a243750be5/views/register-retailer.eis#L7
        https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643cb2a03689ddd94957129a243750be5/views/register-retailer.eis#L15
        https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643cb2a03689ddd94957129a243750be5/views/register:
retailer.ejs#L23
        https://github.com/Dennis
actor/blob/1
29ae243750be5/views/register-
retailer.eis#L40
        https://github.com/DennisC
factor/blob/1 d6dd5643cb2a03689ddd94957129a243750be5/views/register.
retailer.ejs#L44 update-customer.ejs
        https://github.com/DennisChin1022/CR
factor/blob/1d6dd5643c2a03689ddd94957129a243750be5/views/update-
customer.es#L12
        https://github.com/DennisChin1022/CRU
I- refactor/blob/16dd5643cb2a03689ddd94957129ae243750be5/views/update-
customer.eis#L16
        https://github.com/DennisChin1022
factor/blob/1d6dd5643cb2a03689ddd94957129a243750be5/views/update-
customer.ejs#L28
    update-user.ejs
        https://github.com/DennisChin1022/CR
refactor/blob/1d6dd5643cb2a03689ddd94957129ae243750be5/views/update:
user.eis#L12
        https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643c2a03689ddd94957129a243750be5/views/update:
user.eis#L16
        https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643cb2a03689ddd94957129ae243750be5/views/update-
user.ejs#L20
        https://github.com/DennisChin1022/CRUD-refactor/blob/1d6dd5643cb2a03689ddd94957129a243750be5/views/update-
user.ejs#L29
- Password field have to use type="password" to hidden text input.