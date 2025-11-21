---
{"dg-publish":true,"permalink":"/02-notes/ucr-mwa-rest-api-design-principles/","tags":["notes/atomic","UCR-WWA"]}
---


A restful API dominates the modern web, and it has the following characteristics
- Uses [[02Notes/HTTP\|HTTP]] and a [[02Notes/Client-Server Architecture\|client-server protocol]]
- Stateless (each connection is independent),
- [[02Notes/Cacheable\|Cacheable]]
- Resources Based: A resource is data that is distinguishable and operations can be performed on it. 

## End Points

A Restful API web service provides an end point, a distinct URL and [[02Notes/HTTP Action\|HTTP Action]]. An endpoint is commonly called a route, because it routes the URL to some function. 

A client will send a request to the restful endpoint. A request is anything we send to the server, and we are requesting for something to happen.

The **thing** we want to occur is essentially just an HTTP action


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/02-notes/ucr-mwa-http-actions/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





When we make an HTTP request we have access to the following actions/verbs. 

- **POST**: Create (write)
- **PUT**: Modify completely (replace)
- **PATCH**: Modify partially(update)
- **GET**: get (read and retrieve)
- **DELETE**: delete




</div></div>



When sending a request to the endpoint we provided data in the following areas of the HTTP message
- Headers
- The URL string
- Query Parameters
- Body Values

Finally after a HTTP request we will get a response with an associated status code

- **100**: Info, keep going
- **200**: Success
- **300**: Redirection
- **400**: Client Error
- **500**: Server Error


---
## Examples of Rest API 

- [[02Notes/UCR-WMA FastAPI Intro\|Fast API is an example of a rest api]] 

---
# Source
- Bill Lubanovic - FastAPI_ Modern Python Web Development-O'Reilly Media (2023) pg 4