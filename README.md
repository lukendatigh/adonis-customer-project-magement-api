# Adonis Customer Project Management API

Adonis API-only version of a customer project management app.
Customers have projects. Projects have tasks.

## Setup
1. Install AdonisJS using `npm i -g @adonisjs/cli`
2. Clone the repository 
3. Install dependencies using `npm install`
4. Set up your database server
5. Duplicate `.env.example` and rename to `.env` then set your environment variables
6. Run migration with `adonis migration:run`  
7. Run dev server using `nodemon server.js` or `adonis serve --dev`
8. Run postman and start sending requests to endpoints

## API Endpoints
1. List customers
`GET localhost:3333/customers`
2. Retrieve customer
`GET localhost:3333/customers/id`
3. Create customer
`POST localhost:3333/customers`
4. Update customer
`PATCH localhost:3333/customers/id`
5. Delete customer
`DELETE localhost:3333/customers/id`

#### Note:
1. `FindCustomer` middleware implemented so you don't query database in controller methods (avoiding repitition and controller methods looking bulky)
2. Model relationships are already defined for Projects and Tasks, just code on!

## Endpoints To-Do  - for fun!
- [ ] List projects of customer
- [ ] Retrieve project
- [ ] Create project
- [ ] Update project
- [ ] Delete project
- [ ] List tasks in project
- [ ] Retrieve task
- [ ] Create task
- [ ] Update task
- [ ] Delete task


## Built with
 - [Sublime Text](https://www.sublimetext.com) - text editor
 - [AdonisJS](https://www.adonisjs.com) - web framework
