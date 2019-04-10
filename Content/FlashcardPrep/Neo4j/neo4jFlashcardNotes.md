## What is a graph database?

## How can I query a graph?

## What do people do with Neo4j?

## What is a Node?
*Nodes are the name for data records in a graph*

## What is a relationship?
*a connection of nodes. Relationships always have a direction, Relationships always have a type, Replationships form patterns of data.*

```
Emil KNOWS johan and Ian
Johan KNOWS Ian and Rik
Rik and Ian KNOWS Alison
```

## What is a Property?
*simple name/value pairs of stored data*

```
name: "herman"
from: "Morocco"
```

## How do you add a property to a relationship?

## What is a label?
*Labels are grouping objects that have no properties of themselves, like tags or types they get applied to nodes*

`'Apply the label 'person' to the node whe made for Herman`

## How can similar nodes have different properties?

## How do you create a string property in neo4j?

## How do you create a number property in neo4j?

## How do you create a boolean property in neo4j?

## How many nodes can Neo4j store?
*billions*

## What is the query language used by Neo4j?
*Cypher*

## How do you export tabular results of a query result?

## How do you view a graph visualization of query results containing nodes and relationships?

## what is a simple example of Neo4j's REST API?

## How do you access help from the cypher shell?
*by using the help command*

`:help`

## What are the three major topics that can be found by issuing the ':help' command?
*Cypher Syntax and Grammar, Clint-Side Administration CLI command reference, and a keyboard shortcut cheatsheat*

```cypher
:help cypher
:help commands
:help keys
```

## What is the keyboard combination to switch to mutli-line editing in the Cypher shell?
`<shift-enter>`

## What is th keyboard combination to submit a query from the cypher shell?
`<ctrl-enter`

## How do you clear the result stream?
*by using the clear command*

`:clear`

## How do you create a node with a label and properties in cypher?
*by using the `CREATE` clause*

```cypher
CREATE {var:[label] { prop1: [data], prop2: [data], ... } }
RETURN var.prop1
```
```cypher
CREATE (ee:Person { name: "Emil", from: "Sweden", klout: 99 })
RETURN ee.name
```

## How do find a node using cypher?
*by using the `MATCH` clause*

`MATCH (var:[label]) WHERE var.prop = [data] RETURN var;`

```cypher
MATCH (ee:Person) WHERE ee.name = "Emil" RETURN ee;
```

## How do you use the `CREATE` clause to create many nodes and relationships at once
*by separating valid create statements with commas*

```cypher
MATCH (ee:Person) WHERE ee.name = "Emil"
CREATE (js:Person { name: "Johan", from: "Sweden", learn: "surfing" }),
(ir:Person { name: "Ian", from: "England", title: "author" }),
(rvb:Person { name: "Rik", from: "Belgium", pet: "Orval" }),
(ally:Person { name: "Allison", from: "California", hobby: "surfing" }),
(ee)-[:KNOWS {since: 2001}]->(js),(ee)-[:KNOWS {rating: 5}]->(ir),
(js)-[:KNOWS]->(ir),(js)-[:KNOWS]->(rvb),
(ir)-[:KNOWS]->(js),(ir)-[:KNOWS]->(ally),
(rvb)-[:KNOWS]->(ally)
```

## How 
## HOw do you use the `MATCH` clause to serach for a pattern?

```cypher
MATCH (js:Person)-[:KNOWS]-()-[:KNOWS]-(surfer)
WHERE js.name = "Johan" AND surfer.hobby = "surfing"
RETURN DISTINCT surfer
```

## How do you test a query for performance?
*by using the `profile` clause*

```cypher
PROFILE MATCH (js:Person)-[:KNOWS]-()-[:KNOWS]-(surfer)
WHERE js.name = "Johan" AND surfer.hobby = "surfing"
RETURN DISTINCT surfer
```

## How do you test a query to see the steps it took to complete?
*by using the `EXPLAIN` clause*

```cypher
EXPLAIN MATCH (js:Person)-[:KNOWS]-()-[:KNOWS]-(surfer)
WHERE js.name = "Johan" AND surfer.hobby = "surfing"
RETURN DISTINCT surfer
```

## How do you comment a line of code in cypher?
*by using double forwar-slashes `//`*

```cypher
//This is a full line comment

MATCH (n) RETURN (n) //This is an end of line comment
```
## What is a query to show all nodes in cypher?

```cypher
MATCH (n) RETURN (n)
```

## what is a query to return all nodes, including orphans, and all relationships?

```cypher
MATCH (n) OPTIONAL MATCH (n)-[r]-() RETURN n, r;
```

## What is the difference betweent the `DELETE` and `REMOVE` clauses in cypher?
*The Delete clause is used for deleting nodes, while the Remove clause is for removing properties from nodes and relationships, and to remove labels from nodes.*

```cypher
MATCH (n:Person { name: 'UNKNOWN' })
DELETE n
```

```cypher
MATCH (a { name: 'Andy' })
REMOVE a.age
RETURN a.name, a.age
```

## How do you get all nodes with a label in cypher?

```cypher
MATCH (n:Person)
RETURN (n)
```



CREATE (a:Role { name: "front-end web developer" }),
(a:Role { name: "devops engineer" }),
(a:Role { name: "ui designer" }),
(a:Role { name: "ux designer" }),
(a:Role { name: "game developer" }),
(a:Role { name: "ai/ml engineer" }),
(a:Role { name: "iOS developer" }),
(a:Role { name: "mobile developer" }),
(a:Role { name: "reactJS developer" }),
(a:Role { name: "vue.js developer" }),
(a:Role { name: ".net developer" }),
(a:Role { name: "data sciencist" }),
(a:Role { name: "hacker" }),
(a:Role { name: "software architect" }),
(a:Role { name: "angular developer" }),
(a:Role { name: "software quality assurance" }),
(a:Role { name: "full-stack web developer" }),
(a:Role { name: "back-end web developer" })


MATCH (a:Artist),(b:Album)
WHERE a.Name = "Strapping Young Lad" AND b.Name = "Heavy as a Really Heavy Thing"
CREATE (a)-[r:RELEASED]->(b)
RETURN r

MATCH (a:Artist),(b:Album),(p:Person)
WHERE a.Name = "Strapping Young Lad" AND b.Name = "Heavy as a Really Heavy Thing" AND p.Name = "Devin Townsend" 
CREATE (p)-[pr:PRODUCED]->(b), (p)-[pf:PERFORMED_ON]->(b), (p)-[pl:PLAYS_IN]->(a)
RETURN a,b,p

MATCH (u:User {username:'admin'}), (r:Role {name:'ROLE_WEB_USER'})
CREATE (u)-[:HAS_ROLE]->(r)



//Get all roles
MATCH (role:Role)
RETURN role.name


MATCH (:Role { name: 'web developer' })--(role:Role)
RETURN role.name

MATCH (role:Role { name: 'web developer' })
RETURN role.name


MATCH (a:Role) WHERE a.name = "web developer"
RETURN a.name

MERGE (person)-[r:HAS_CHAUFFEUR]->(chauffeur:Chauffeur { name: person.chauffeurName })
RETURN person.name, person.chauffeurName, chauffeur