# Blog system

## Description

```markdown
The task is to create a backend API for a simple blog system consisting of Articles, Users and Comments.

**Features:**

    Articles:
        - Create a new article ( title, body, and author )
        - Read/retrieve a given Article by ID.
        - List all articles.
        - Search for a specific article.
        - Add comments to a given article.
        - Thumbs up to a given article.
    Author:
        - Create a new author ( name and job title )
        - Read/retrieve given Author info by ID.
        - List all authors.

**Requirements:**

    - The features above need to be implemented in the form of a Restful API.
    - The API needs to be implemented using Node.js
    - Use MySQL as a Database to store the data.
    - Use Expressjs as the HTTP server for your API.
    - Implement input validation for all the endpoints.
    - Write unit and end to end test cases.
    - Write design documentation for both the API and the data model.
    - The code should be hosted on one of the following source management systems ( Github, Gitlab )

**Bonus:**

    - Implement the task using one of the frameworks that support Typescript, e.g. NestJs ( https://nestjs.com/ )
    - Use Docker and docker-compose to automate building and provisioning of the API and the database.
    - Add functionality to sort articles by the number of thumbs up given.
    - Enhance articles searching ( i.e. text scoring, search engines )
    - Deploy your API to one of the free hosting services, e.g. Heroku.
```

# Accomplishments

- Most of the previous requirements and more extra features as the following

  - Authorization and authentication

    - Router /auth
      - GET /me retrieve authenticated user data
      - POST /register registration form for an anonymous user
      - POST /login for all system users
      - POST /update-profile authenticated user to update his updatable profile fields
      - POST /forget-password will log the user password code for use in the reset password form
      - POST /reset-password will change forgotten user password
      - POST /change-password to let the authenticated user update this password from his profile
    - Router /users CRUD for admin only manipulate users and register new users from dashboard
      - GET /users
      - POST /users
      - GET /users/:id
      - PATCH /users/:id
      - DELETE /users/:id

  - Generic API DTOs you will be able to fetch records generically

  - Join allowed fields optionally
  - choose displayed fields
  - paginate via page and limit
  - filter fields as a key-value array
  - order fields as a key-value [ASC, DESC] array

  - Docker will create init the database and bootstrap the application
  - Generic repository for database CRUD operations
  - All users authorized (admin, author, user) to create any comment or article comment.

---

### Missing

- Tasks

  - Jest Unit or end to end tests cases

- Bonus

  - Search engine as elastic search for text score and filtering

- Extra

  - Send emails on forgetting the password, Welcome email via node mailer
  - Search engine connector as stream processing for database operations
  - Generic search engine repo, CRUD (service, controller)
  - Publish source code for privacy considerations

---

## Users scenarios

- System admin
  A system admin will be seed on bootstrap the application (email: admin@dev.com, password: string)
  Admin will be able to delete any articles, comments, manage all users, and only one able to create admins, that will cascade in their nested reference relations

- User
  You have to register a new user and use his token to create comments, and like or dislike (undo him like)

- Author of articles
  You have to register a new user and use his token to register as an author for creating articles
  Authors own to be able to change, delete their own articles, comments only
  On delete article it's Comments, Likes will be deleted

---

## Links

- GitHub [Repo](https://github.com/Hisham-TK/node-nest-trufla)
- APIs [Documentation](http://hisham.work:3001/docs)
- Challenge [Board](https://trello.com/c/Z5R7nAsT)
