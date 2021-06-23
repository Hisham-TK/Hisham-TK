# Restaurant API

## Description:

This task for Index-Group Company

```markdown

We need a simple APIs for restaurants with these requirements

    1. Authentication and authorization (a System admin and normal users).
    2. System admin can add , update and delete restaurants.
    3. Find nearest restaurants from a given location (point).
    4. Type ahead search on restaurants names.
    5. Statistics endpoint to group restaurants and their count by city .

---

Models

    User
        name
        email
        password
        role
    City
        name
    Restaurant
        city
        image
        name
        email
        location

---

Recommended technology stack

- Nest js
- Mongoose
- Swagger
- Passport

---

Notes

- Consider REST standards while writing your api
- Consider a clear project architecture
- Add a dummy system admin on app startup if not exists
- Write a clear swagger documentation
- Deploy your api on any free hosting service

```

---

## Installation

```bash
$ npm install
```

---

## Running the app

```bash
# development
$ npm start
```

---

## Architecture

<p align="center">
 <img src="https://i.ibb.co/6Hxz1Dm/My-first-service.jpg" width="800" alt="Nest Logo" />
</p>
<!-- ![Service Overview](https://i.ibb.co/6Hxz1Dm/My-first-service.jpg) -->

We need a simple api for restaurants with these requirements:-

- Authentication and authorization (a System admin and normal users).
- System admin can add , update and delete restaurants.
- Find nearest restaurants from a given location (point).
- Type-ahead search on restaurants names.
- Statistics endpoint to group restaurants and their count by city .

Models :

User:

- name
- email
- password
- role

City:

- name

Restaurant:

- city
- image
- name
- email
- location

Recommended technology stack :

- Nest js , Mongoose , Swagger , Passport.

Notes:

- Consider rest standards while writing your api.
- Consider a clear project architecture.
- Add a dummy system admin on app startup if not exists.
- Write a clear swagger documentation.
- Deploy your api on any free hosting service.

## License

Nest is [MIT licensed](LICENSE).

# TODO:

## Build

- <s>Activate version incrementing for documents changes</s>
- <s>Exclude password from any response about user or auth</s>
- <s>Create generic interceptor to delete fields fields</s>
- <s>Activate soft delete</s>
- Complete the Geo-point mongo to location interceptor
- Numbering system
- Generic service
- Pagination for all "find many" and "search"
- Create base Schema for all models
- Document every mongo ACL for create and update
- Front-End: Angular, React
- Mobile: Ionic, React-native

## Config

- Elasticsearch
- Web sockets: Gateways
- Organize structure flixable to extend modules
- Email for forget password
- OAuth for authentication
- Add validators and district them into decorators
