## Learning project

there are two servers in this project

one is playing role of our service that we work on
and can be spined up running `node server.js` inside of root folder

second one playing role of external api that we send a request to get data from DB
and can be spined up running `npm run json:server` inside of root folder 

So that is how we run two servers in parallel 

to send some simple GraphQL request go to `localhost:4000/graphql`

and inside of `GraphiQL` - `is a tool that helps building queries in dev mode`
build your query, query in `GraphQL` is always begins with curly brackets
and hits `Root query` - is entry point to GraphQL

example of queries:
```
{
  user(id: "40") {
  	firstName
  }
}
```

or 
```
{
  user(id: "40") {
    firstName
    age,
    companyId
  }
}
```