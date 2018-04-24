## Getting started

```bash
npm install
npm start
```

Then open [http://localhost:3000/graphiql](http://localhost:3000/graphiql)

When you paste this on the left side of the page:

```graphql
{
  author(firstName: "Edmond", lastName: "Jones") {
    firstName
    lastName
  }
  getFortuneCookie
}
```

and hit the play button (cmd-return), then you should get this on the right side:

```json
{
  "data": {
    "author": {
      "firstName": "Edmond",
      "lastName": "Jones"
    },
    "getFortuneCookie": "What boots up must come down."
  }
}
```
