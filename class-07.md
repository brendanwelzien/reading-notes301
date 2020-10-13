# What Google Learned About Teams
- What Google learned from its question to build the perfect team

- conflict with leadership in a team, who was in charge

- talking simply outside of group work time was more pleasant than when working together

- shift in increased efficiency of work stems from group collaboration

- important for a company to influence how their employeees work together

- In 2012, Google launched Project Aristotle

- group norms seemed to be the reason to how team's could improve
    - success also stemmed from not intelligence, but how teammates treated each other,
    - social sensitivity, collectively retains an increased intelligence
- psychological safety is critical for a positive team-work environment
- no one wants to put on a 'work-face' at the office, leaving your personality out of it can be detrimental

# How I explained REST with my brother
- http is the foundation of the web, similar to GPS coordinates for knowledge and information
    - REST is a resource, a web page is a representation of a resource
    - the URL is the common communication-ground for the various systems, databases, and languages out there... Allows machines to talk to each other

# SuperAgent
- progressive ajax API created for flexibility and is compatible with node.js

*request*
- a request can be made by invoking a `method` on the `request` object, then calling `.then()` or     `end()` or `await()` to send request
```js
.get('/search')
.then(res => {
    //res.body, res.headers, res.status
})
.catch(err => {
    //err.message, err.response
});
```

```js
request('GET', '/search').then(success, failure);
```

- head requests use .query() methods
- post/put requests calls then waits for the response string
- 
[<=Back](README.md)