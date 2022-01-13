# GoBarber (back-end)

An API for GoBarber app developed using Node.js (with Typescript) for study purposes.

This API is used by the ReactJS app available on the following repository:

https://github.com/josealexandre/gobarber-frontend-web

## Useful resources:

Here are some of the packages and tools used in this project:
- Typescript
- Express.js
- jsonwebtoken
- bcryptjs
- uuidv4
- mysql
- typeorm
- date-fns
- multer
- eslint
- prettier
- ts-node-dev

## Instructions to run the project

1) Before you run the application it's necessary to get all the dependencies of the project using the command `yarn` from inside the project folder.

2) Then you can start a MySQL container and create a database into it or just create a database in your MySql server if you have one. To create a MySql container run the following command:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `docker run --name mysql -e MYSQL_ROOT_PASSWORD=admin -p 3306:3306 -d mysql`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; :warning: The command above is only for **development** environment! Do **NOT** use this command in **production** environments!

3) After creating the database you have to setup the ormconfig.json file with you database access info.

4) Then run migrations using the following command:
`yarn typeorm migration:run`

5) Now you should be good to go. To start the application just run:
`yarn dev:server`
