# Reading Assignment - 12

## Readings: CRUD

### Date 10-26-2021

1. [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

In your own words, describe what each group of status code represents:
100’s = Informational status codes - typically indicate an error prior to the error being recognized 
200’s = Success Codes - clients request was accepted
300’s = Redirection Codes - Resource requested isn't available and a request is required for a different location.
400’s = Client Error Codes - Invalid request from the client sent to the server
500’s = Server Error Code - indicate problems or overwhelmed servers beyond proxies.
What is a status code 202? Asynchronous processing of a request - request met all validation requirements but may not have been processed
What is a status code 308? Permanent Redirection
What code would you use if an update didn’t return data to a client? (204) no Content
What code would you use if a resource used to exist but no longer does? (410) Gone
What is the ‘Forbidden’ status code? (403)

1. [Build A REST API With Node.js, Express, & MongoDB - Quick](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

Why do we need to pull our MongoDB database string out of our server and put it into our .env?
- Security - do not want our passwords and API keys pushed to public repos
What is middleware?
- A medium like axios or other to bridge the gap between the client and the server
What does app.use(express.json()) do?
What does the /:id mean in a route?
What is the difference between PUT and PATCH?
How do you make a default value in a schema?
- use the || operator
What does a 500 error status code mean?
- Internal Server Error
What is the difference between a status 200 and a status 201?
- 200 is status ok, while 201 represents the operation is created

## Things I want to know more about
