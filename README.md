### Stack choice
| Type | Stack | Why |
|--|--|--|
| Front-end framework | React | It's a classic framework for handling single-page web application that are scalable, maintaiable and with many features |
| Client Side routing | React Router | It's the recommanded way to do routing with React |
| CSS framework | Material UI | It was recommended by several sites, it has many styling features and it's well-integrated with React |
| Static type checking | TypeScript | It adds a lot of safety to the code, it reduces chances of runtime errors when launching to production |
| Database | PostgreSQL | No need for a NoSQL database for such a basic product. And PostgreSQL seams to be the best compromise between all SQL databases (in terms of performance & features) |
| Server | Express.js | It's the framework of choice for building web APIs - popular, fast, and easy to use |
| Auth system | JWT | It's a standard way of handling tokens, it works great and is easy to implement (e.g no need to store anything on the server) |
| DB interaction | knex.js | It's less heavy than an actual ORM (it's just a query builder) and still easy to use (you don't write SQL queries). I also implemented a kind of MVC folder structure on top of knex |

### Setup
The project is composed of 3 subfolders:
- `python` which contains the Python script. This one doesn't need any perticular setup.


- `app` which contains the frontend. To setup:

   If not yet done, install NPM and Node.js

   Then run `npm install`

   And `npm start`.

   This should compile the react application and launch a web browser with the app.


- `server`, which contains the backend. This one is a bit more difficult to setup:

   First install [PostgreSQL](https://www.postgresql.org/) on your machine and create a database with the name of your choice

   Then go to folder `config` and copy file `development.json.dist` to `development.json`. Edit the database configuration.

   Now run `npm install`.

   Then run `npm run db:reset` to create the database tables.
   [Only windows users: intall npm install -g win-node-env]
   Finally, `npm start` will launch the server. 

The DB is prefilled with 2 users:
- A client with credentials t.malahieude@gmail.com / aaaaaa
- A farmer with credentials timothe@malahieude.net / aaaaaa

Feel free to use those users to play with the app!
