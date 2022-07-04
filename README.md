# GraphQL
# Introduction
GraphQL is an open-source data query and manipulation language for API. It was developed internally by the Facebook corporation in 2012.GraphQL is a query language to build client applications by providing flexible and intuitive syntax for asking the data requirements.

# Objective
It was developed to optimize RESTFUL API calls. And provides flexible, robust, and more efficient alternative to REST.

# Why GraphQL

* It overcomes the problem of Over-Fetching or Under-Fetching. With GraphQL, developers can fetch what is required. Nothing less, nothing more. It solves the issues that arise due to over-fetching and under-fetching.

* GraphQL allows making multiple resource requests in a single query call, which saves a lot of time and bandwidth by reducing the number of network round trips to the server. It also helps to save waterfall network requests, where our need to resolve dependent resources on previous requests. 

* With GraphQL, there is no need to maintain versions. The resource URL or address remains the same. You can add new fields and deprecate older ones. This approach is intuitive as the client receives a deprecation warning when querying deprecated fields.


# GraphQL Components


There are two types of GraphQL application components:

         GraphQL Server-side Components
         GraphQL Client-side Components
         
         
# GraphQL Server-side Components : 
The GraphQL API uses three main components that reside on the GraphQL server. These components are the query, resolver, and schema. Server-side components allow parsing of the queries coming from GraphQL client applications.


            A. Query
            B. Resolver
            C. Schema


A. Query: The query is an API request made by the client machine application. It supports augments and points to arrays. A query is used to read or fetch values.
Parts of Query:
 1. Fields: A field simple indicates that we are asking the server for particular information. The following is a GraphQL example of fields in a graph
 
 
                                  query {
                                      student {
                                            id name
                                            }
                                   }
                                   
                                   
                                   
This is a typical GraphQL query. Queries are made up of two distinct parts:

     The root field (student): the object containing the payload
     
      The payload (id name): the client-requested field(s).
                                  
                                  
  2. Arguments: GraphQL queries allow us to pass in arguments into query fields and nested query objects. We can pass arguments to every field and every nested object in our query. 
  
                             
                             {
                               student(id : "sumit") {
                                    name,
                                     stuff {
                                        laptop,
                                        smartphone
                                    }
                                }
                              }
                              
                              
 Here, we are requesting the desired fields on the student sumit because of the id argument we passed into the query. Just like fields, there are no type restrictions. Arguments can be of different types too.
  
  
 
 B.Resolver: Resolvers provide the directions for converting GraphQL operations into data. They resolve the query to data by defining resolver functions.
It displays the server's process as well as the location to fetch data according to a specific field. The resolver also separates the database schema and the API schema. The separated information helps to modify the content obtained from the database
    
    
    
 C.Schema:A GraphQL schema is the heart of GraphQL implementation. It describes the functionality available to the clients that are connected to it.
 
 
 
 
 
 
 # GraphQL Client-side Components : 
 The client-side components reside on GraphQL clients. The GraphQL client is a piece of code or a JavaScript library that makes POST requests to the GraphQL server. It may be a CMS like Drupal, a single-page application, a mobile application, etc.
  
  
  * GraphiQL: It is a browser-based interface used for editing and testing GraphQL queries and mutations.
  
  * ApolloClient: It is one of the best tools to build GraphQL client applications. It can be easily integrated with all JavaScript front-ends.


# GraphQL Architecture

The GraphQL architecture is a set of guidelines on how requests and responses should be handled, like supported protocols, the format of the data that can be accepted by the server, the format of the response returned by the server, etc. The request made by a client to the GraphQL server is called a query.

The GraphQL Server can be deployed by using any of the three methods listed below.

                  * GraphQL server with a connected database.
                  * GraphQL server that integrates existing systems.
                  * Hybrid approach.




* GraphQL server with a connected database: 
This architecture has a GraphQL Server with an integrated database and can often be used with new projects. On the receipt of a query, the server reads the request payload and fetches data from the database. This is called "resolving the query." The response returned to the client adheres to the format specified in the official GraphQL specification.


* GraphQL server that integrates existing systems: 
 This approach is helpful for companies that have legacy infrastructure and different APIs. GraphQL can be used to unify microservices, legacy infrastructure, and third-party APIs in the existing system.

* Hybrid approach :
This is the combination of two architectures: a GraphQL server with  a connected database and a GraphQL server that integrates existing systems. In this architecture, the GraphQL server will resolve any requests that are received. It will either retrieve data from a connected database or from the integrated API.


# Summary

*GraphQL is an application layer server-side technology that was developed by Facebook for executing queries with existing data.
* We can use GraphQL to fetch data with a single API call.
*   (I) Query, (II) Resolver, and (III) Schema are important GraphQL query components.
* A GraphQL client is a code that makes POST requests to a relevant GraphQL server.
* GraphQL servers are server-side implementations of GraphQL’s specifications.
# Refrences

 * https://www.javatpoint.com/graphql

 * https://youtube.com/playlist?list=PL4cUxeGkcC9iK6Qhn-QLcXCXPQUov1U7f

 * https://graphql.org

 * https://developers.facebook.com/docs/graph-api/
  
