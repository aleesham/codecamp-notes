# <center> __Learning Objectives__ </center>

# __Lesson 1__
### __HTML__
- Identify the main type of content on the W.W.W.  
HTML is the main document type of the web.

- Know what HTML stands for.  
HyperText Markup Language

- Describe the request/respone flow defined by HTTP.
<!-- I don't know what goes in here. -->

- Describe the components of HTML tag structure.
<!-- I don't know what goes in here. -->

- Describe what an HTML element is, and how an element is related to a tag.
<!-- I don't know what goes in here. -->

- Name, describe the purpose of, and use common HTML tags:  
    - `<b>`: This is the bold tag, which boldfaces its contents.
    - `<em>`: This is the emphasis or italize tag, which italicizes its contents.
    - `<a>`: This is the anchor tag which makes its content a link to its href attribute content.
    - `<img>`: This is an image tag. It is self closing. It has a src attribute which you set equal to the URL of your image and an alt attribute which is what is shown should the src code be incorrect, or should that webpage break.
    - `<br>`: This is the inline line-break tag. It is a void tag. 
    - `<p>`: This is the paragraph tag. It is like a line-break tag, however it is a block tag. You can imagine this tag creates an invisible box around its contents.
    - `<span>` 
    <!-- I don't know what goes in here. -->
    - `<div>`
    <!-- I don't know what goes in here. -->
    - `<form>`
    <!-- I don't know what goes in here. -->

- Define HTML attributes and how they are used.
<!-- I don't know what goes in here. -->

- Describe how whitespace in HTML documents affects rendering.
<!-- I don't know what goes in here. -->

- Describe inline and block display; for common elements identify their default display.
<!-- I don't know what goes in here. -->

- Describe HTML document structure and associated elements:
    - doctype
    <!-- I don't know what goes here. --> 
    - `<html>`
    <!-- I don't know what goes here. --> 
    - `<head>`
    <!-- I don't know what goes here. --> 
    - `<body>`
    <!-- I don't know what goes here. --> 
    - `<title>`
    <!-- I don't know what goes here. --> 

- Create a properly-structured document head.
```{html}
<!DOCTYPE html>
<html>
    <head>
        <title>Contents</title>
    </head>

    <body>
        <!-- Add your body here -->
    </body>
</html>
```

### __GIT__
- Describe the main functionality provided by a version control system (VCS).
<!-- I don't know what goes here. --> 
- Describe the practical applications of this functionality:
    - revision
    <!-- I don't know what goes here. --> 
    - history
    <!-- I don't know what goes here. --> 
    - collaboration 
    <!-- I don't know what goes here. --> 
    - backup
    <!-- I don't know what goes here. --> 
- Explain what a repository is.
<!-- I don't know what goes here. --> 
- Explain what a commit is. 
<!-- I don't know what goes here. --> 
- Describe the basic commit flow and commands:
    - status
    <!-- I don't know what goes here. --> 
    - add
    <!-- I don't know what goes here. --> 
    - commit
    <!-- I don't know what goes here. --> 
    - log
    <!-- I don't know what goes here. --> 
- Initialize a new Git repository.
<!-- I don't know what goes here. --> 
- Commit to a local repository.
<!-- I don't know what goes here. --> 
- Clone a project from a remote Git repository.
<!-- I don't know what goes here. --> 
- Explain the two Git file status: tracked and untracked.
<!-- I don't know what goes here. --> 
- Explain what types of changes should be within a commit.
<!-- I don't know what goes here. --> 






<!--
#
# __Lesson 2__ 
### __HTML__
- Describe the purpose of, and use additional HTML tags:
    - `<ul>`
    - `<ol>`
    - `<li>`
    - `<table>`
- Create HTML comments.

### __CSS__
- Explain how CSS allows for separation of display and document structure.
- Describe the three locations that style rules may be placed:
    - external
    - document
    - inline
- Use CSS rules at each of the three possible locations.
- Describe precedence between CSS rules based on location.
- Use basic CSS rule types: `font-size`, `color`, `font-family`, `background-color`, `text-align`, etc.
- Describe the following simple selector types and situations in which each is preferred:
    - element
    - ID
    - class

### __GIT__
- Explain some common use cases for branches.
- Identify the `master` branch as the default branch for most projects.
- Create a new Git branch.
- Checkout a branch.
- Stash and un-stash changes making up partially-completed work.
- Merge one banch into another.
- Describe what happens when, during a merge, there are conflicting changes in the two branches.
- Describe the common branching strategies of feature branches and long-running branches.
- Describe what a remote repository is.
- Create and push to a remote repository.
- Collaborate with another student on a Git project via GitHub

#
# __Lesson 3__
### __HOW THE WEB WORKS__
- Identify the main parts of a URL and describe the role of each:
    - protocol:
    - host:
    - port: 
    - path:
    - query parameter:
    - fragment
- Name the default port(s) for HTTP requests.
- Nae the two most common HTTP request types and describe common use cases for each. 
- Describe usage of HTTP request headers.
- Provide examples of common request header parameters.
- Describe common HTTP response status codes: 200, 404, 500.
- Describe the meaning  of HTTP response headers, alone with common response headers. 
- Describe the role of web servers in providing web content.
- Explain the difference between statis and dynamic requests/content.
- Explain what a web application does.
- Identify and explain the basic role of the components of network communication: HTTP, TCP/IP, DNS.
- Explain the flow of an HTTP request made from a web browser.

### __HELLO WORLD FLASK APPLICATION__
- Create a virtual Python environment using conda.
- Activate a virtual environment.
- Install packages into a virtual environment.
- Create and run a basic Flask application.

#
# __Lesson 4__
- Create an HTML form using `<form>`   
- Create form input elements with common types: text, submit, password, email, checkbox, radio.
- Use the `name` attribute of form inputs to name request parameters.
- Create handlers in Flask for GET and POST request types.
- Use the `value` attribute to spcify the data value that is sent to the server upon form submission.
- Describe the differences betweem GET and POST, and what each request type should be used for.
-  Describe common HTTP status codes by group (2xx, 3xx, 4xx, 5xx).
- Describe the common HTTP status codes: 200, 302, 400, 404, 405, 500.
- Explain why we receive a 405 error when submitting a form to a handler with a decorator like `@app.route('/')`.
- Use `str.format()` to create strings from template strings and data values.


#
# __Lesson 5__
- Describe why we must validate form submissions, even when providing limited options via a form.
- Describe the various ways that we can control and verify the data that the users submit in an HTTP request:
    - form restrictions
    - client-side validation
    - server-side validation
- Describe advantages and disadvantages of both client-side and server-side validation.
- Validate request data based on numeric range or string length.
- Return descriptive error messages within an HTML page when form data doesn't validate. 
- Upon validation errors, render a form with valid data left in-place.
- Describe why HTML escaping is necessary when putting user-submitted data in a response.
- Return a redirect respone.

#
# __Lesson 6__
- Describe the benefits of using templates.
- Use the Jinja2 template environment.
- Use autoescaping within Jinja2 templates.
- Create stand-alone Jinja2 templates.
- Pass data from request handlers into templates.
- Create Jinja2 templates that use base templates and content blocks.
- Write conditionals and loops within Jinja2 templates.

#
# __Lesson 7__
- Explain what relational databases are used for and what SQL is.
- Perform CRUD (Create, Read Update, Delete) operations using SQL queries.
- Explain what joins are used for.
- Describe the difference between the four types of joins:
    - inner:
    - left outer:
    - right outer:
    - full outer:
- Write queries using joins.
- Utilize foreign keys.
- Explain the similarities between Python objects and database tables.
- Create tables with an understanding of one-to-many relationships.

#
# __Lesson 8__
- Utilize _phpMyAdmin_ and build a database locally.
- Create a new user and database.
- Import tables using a `.sql` file.
- Explain how and why data is split into related tables.
- Perform complex SQL queries with joins and subqueries.

#
# __Lesson 9__
_Coming Soon_

#
# __Lesson 10__
_Coming Soon_

#
# __Lesson 11__
_Coming Soon_

#
# __Lesson 12__
_Coming Soon_

#
# __Lesson 13__
_Coming Soon_

#
# __Lesson 14__
_Coming Soon_
-->