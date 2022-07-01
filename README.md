# GraphQL
# Introduction
GraphQL is an open source data query and manipulation language for API. It was developed internally by Facebook coorporation in 2012.GraphQL is a query language to build client application by providing flexible and intuitive syntax for asking the data requirements.

# Objective
It was developed to optimize RESTFUL API calls. And provide s flexibilty,robust and more effiecient alternative to REST.

# Why GraphQL

* It overcome the problem of problem of Over-Fetching or Under-Fetching.With GraphQL, developers can fetch only what is required. Nothing less, nothing more. This solves the issues that arise due to over-fetching and under-fetching.

* GraphQL allows making multiple resources request in a single query call, which saves a lot of time and bandwidth by reducing the number of network round trips to the server. It also helps to save waterfall network requests, where our need to resolve dependent resources on previous requests. 

* With GraphQL, there is no need to maintain versions. The resource URL or address remains the same. You can add new fields and deprecate older fields. This approach is intuitive as the client receives a deprecation warning when querying a deprecated field.


# GraphQL Components


There are 2 types of GraphQL application components:

         GraphQL Server-side Components
         GraphQL Client-side Components
         
         
# GraphQL Server-side Components : 
The GraphQL API uses three main components that reside on the GraphQL server. These components are query, resolver, and schema. Server-side components allow parsing the queries coming from GraphQL client applications.


            A. Query
            B. Resolver
            C. Schema


A. Query: The Query is an API request made by the client machine application. It supports augments and points to arrays. Query is used to read or fetch values.
Parts of Query:
 1. Fields : A field simply indicates that we are asking the server for particular information. Following is a GraphQL example of a field in graphQL 
 
 
                                  query {
                                      student {
                                            id name
                                            }
                                   }
                                   
                                   
                                   
This is a typical GraphQL query. Queries are made up of two distinct parts:

      The root field (student): The object containing the payload.
     
      The payload (id name): The field(s) requested by the client.
                                  
                                  
  2. Arguments : GraphQL queries allow us to pass in arguments into query fields and nested query objects. We can pass arguments to every field and every nested object in our query.
  
                             
                             {
                               student(id : "sumit") {
                                    name,
                                     stuff {
                                        laptop,
                                        smartphone
                                    }
                                }
                              }
                              
                              
  Here, we are requesting the desired fields on the student sumit because of the id argument we passed into the query. Just like fields, there are no type restrictions. Arguments can be of different types, too.
  
  
 
 B. Resolver: Resolvers provide the directions for converting GraphQL operation into data. They resolve the query to data by defining resolver functions.
    It displays the server the process as well as location to fetch data according to a specific field. The resolver also separates database schema           and API schema. The separated information helps to modify the content obtained from the database.
    
    
    
 C. Schema : A GraphQL schema is the center of GraphQL implementation. It describes the functionality available to the clients which are connecting to     it.
 
 
 
 
 
 
 # GraphQL Client-side Components : 
 The client-side components reside on GraphQL clients. The GraphQL client is a code or a JavaScript library that makes POST requests to the GraphQL server. It may be a CMS like Drupal, a single page application, a mobile application, etc.
  
  
  * GraphiQL: It is a browser-based interface used for editing and testing GraphQL queries and mutations.
  
  * ApolloClient: It is one of the best tools to build GraphQL client applications. It can be easily integrated with all JavaScript
front-end.


# GraphQL Architecture

GraphQL architecture is a set of guidelines on how requests and responses should be handled like supported protocols,format of the data that can be accepted by the server, format of the response returned bythe server, etc. The request made by a client to the GraphQL server is called a Query.

GraphQL Server can be deployed by using any of the three methods listed below:
* GraphQL server with connected database
* GraphQL server that integrates existing systems
* Hybrid approach


* GraphQL server with connected database: 
This architecture has a GraphQL Server with an integrated database and can often be usedwith new projects. On the receipt of a Query,the server reads the request payload and fetches data from the database. This is called resolving the query. The response returned to the client adheres to the format specified in the official GraphQL specification.


* GraphQL server that integrates existing systems: 
 
This approach is helpful for companies which have legacy infrastructure and different APIs. GraphQL can be used to unify microservices, legacy infrastructure and third-party APIs in the existing system.

* Hybrid approach :
This is the combination of two architecture that is GraphQl server with connected databse and GraphQl server that integrates existing systems. In this architecture, the GraphQL server will resolve any request that is received. It will eitherretrieve data from connected database or from the integrated API’s. 


# Summary

* GraphQL is an application layer server-side technology which is developed by Facebook for executing queries with existing data.
* We can use GraphQL to fetch data with a single API call.
* Important GraphQL query components are: 1) Query, 2) Resolver, 3) Schema.
* GraphQL client is a code that makes POST requests to a relevant GraphQL Server.
* GraphQL servers are servers side implementation of GraphQL’s specification.

# Refrences

 * https://www.javatpoint.com/graphql

 * https://youtube.com/playlist?list=PL4cUxeGkcC9iK6Qhn-QLcXCXPQUov1U7f

 * https://graphql.org

 * https://developers.facebook.com/docs/graph-api/
  
