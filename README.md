## CRUD Express Graphql Next MongoDB

### Please Read
This project is about perfom simple CRUD operations with Node.js, Express, GraphQL, Next.js and MongoDB

### How to Run
To run the project please nevigate to the project root folder

First, install the project dependencies with npm or yarn

```bash
yarn install
```

Second, run the GraphQL server:

```bash
yarn start-gql
```

Open [http://localhost:4000/api/graphql](http://localhost:4000/api/graphql) with your browser to see the result. These will open Apollo Server for intarect with GraphQL API using their tools.

#### Example Query

**Operation**
```bash
mutation AddUser($inputUser: InputUser!) {
  addUser(inputUser: $inputUser)
}
```

**Variables**
```bash
{
  "inputUser": {
    "firstName": "Asraful",
    "lastName": "kadir",
    "email": "kadir@gmail.com",
    "password": "3",
    "videos": [
      {
        "title": "Nice Dog",
        "category": "dog",
        "tags": ["dog","animal"],
        "url": "videos/dog.mp4",
      }
    ]
  }
}
```

Third, run the Next.js development server:
```bash
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

**Thanks**