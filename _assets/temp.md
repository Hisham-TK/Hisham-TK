# Notifications service

## Description

#### Case: xxx

```markdown

```

---

## Architecture

### Whole app architecture

![](./)

---

## Chosen technologies

- Nest.js
  : Node.js framework using TypeScript based on some "angular/core" packages

---

## Requirement

- Install Node.js v12+

---

## How to start

### Running on Docker

```bash
# Docker
$ docker-compose up -d
```

### Running on local development

- After install Node.js, Erlang, Rabbit-MQ

```bash
# Local development
$ npm install

# development
$ npm run start

# watch mode
$ npm run start:dev
```

### Test application

```bash
# Run unit tests
$ npm run test

# Run end to end tests
$ npm run test:e2e

# Run coverage tests
$ npm run test:cov
```

---

## Future improvements

- Implement more bushiness, and validation instead of just payload pipe-line validation
- Add email notification and mail message to notification module depend on bushiness needs
- Create push notification module that will have multi devices tokens
- Use event source with subscribers on (user, user-group) events; instead of (user, users-groups) mocks
- Mirror queuing to the message broker for High availability
- Integrate with a real push notification, sms services providers
- test cases and write more unit tests

---

## Stay in touch

- Repo Author - [Hisham Taha](https://www.linkedin.com/in/hisham-taha-kamal-al-din/)

---

## License

Nest is [MIT licensed](LICENSE).
