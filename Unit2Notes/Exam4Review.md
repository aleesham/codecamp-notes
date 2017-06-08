# <center> __Exam 4 Learning Objectives__ </center>

### __HTML Basics__
- Identify the main type of content on the W.W.W.  
HTML is the main document type of the web.

- Know what HTML stands for.  
HyperText Markup Language

- Describe the request/respone flow defined by HTTP.  
Your browser makes requests via the internet to servers. These requests are using a protocol called http, and the servers respond with files that your browser displays.

- Describe the components of HTML tag structure.  
The compo
`<NAME ATTR="value"> Contents </NAME>` 
<!-- I don't know what goes in here. -->

- Describe what an HTML element is, and how an element is related to a tag.
The complete code from an opening tag to its respective closing tag is called an element.
<!-- I don't know what goes in here. -->

- Name, describe the purpose of, and use common HTML tags:  
    - `<b>`: This is the bold tag, which boldfaces its contents.
    - `<em>`: This is the emphasis or italize tag, which italicizes its contents.
    - `<a href="url">`: This is the anchor tag which makes its content a link to its href attribute content.
    - `<img src="url" alt="text" title="text">`: This is an image tag. It is self closing. It has a src attribute which you set equal to the URL of your image and an alt attribute which is what is shown should the src code be incorrect, or should that webpage break.
    - `<br>`: This is the inline line-break tag. It is a void tag. 
    - `<p>`: This is the paragraph tag. It is like a line-break tag, however it is a block tag. You can imagine this tag creates an invisible box around its contents.
    - `<span>`: This is an inline tag. This element does nothing but contain its content.
    ```
    <span>this is one line</span>

    yep, one line
    ## This displays "this is online yep, one line"
    ```
    <!-- I don't know what goes in here. -->
    - `<div>`: This is a block tag. This element does nothing but contain its content.
    ```
    <div>this is not one line</div>.

    yep, two lines
    ## This displays "this is not one online
    ##                .yep, two lines"
    ```
    <!-- I don't know what goes in here. -->
    - `<form>`: This is a block tag.
    <!-- I don't know what goes in here. -->
    - `<ul>`: This is an unordered list tag.
    - `<ol>`: This is an ordered list tag.
    - `<li>`: This is a list-item tag.
    - `<table>`
    <!-- I don't know what goes in here. -->

- Define HTML attributes and how they are used.
<!-- I don't know what goes in here. -->

- Describe how whitespace in HTML documents affects rendering.
<!-- I don't know what goes in here. -->

- Describe inline and block display; for common elements identify their default display.
<!-- I don't know what goes in here. -->

- Describe HTML document structure and associated elements:
    - doctype: This is what kind of html this is. 
    - `<html>`: This surrounds the entire document.
    - `<head>`: This part of the document has meta-data, js, CSS, and other random stuff. 
    - `<body>`: This contains the contents of the document. This is where all the interesting stuff happens. 
    - `<title>`: This appears in the head tag. This appears in the top of the brower window or your browser tab.

##### CSS Basics
- Explain how CSS allows for separation of display and document structure.
- Describe the three locations that style rules may be placed:
    - external
    - document
    - inline
- Describe precedence between CSS rules based on location.
- Describe the following simple selector types and situations in which each is preferred:
    - element
    - ID
    - class

### __Branching Out with Git__
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
- Explain the two Git file status: tracked and untracked.
<!-- I don't know what goes here. --> 
- Explain what types of changes should be within a commit.
<!-- I don't know what goes here. --> 
- Explain some common use cases for branches.
- Identify the master branch as the default branch for most projects.
- Stash and un-stash changes making up partially-completed work.
- Merge one branch into another.
- Describe what happens when, during a merge, there are conflicting changes in the two branches.
- Describe the common branching strategies of feature branches and long-running branches.
- Describe what is remote repository.


### __How the Web Works__
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


### __Dynamic Webpages__
- Create an HTML form using `<form>`: 
<!-- I don't know what goes here. --> 
- Create form input elements with common types: text, submit, password, email, checkbox, radio.  
<!-- I don't know what goes here. --> 
- Use the `name` attribute of form inputs to name request parameters.
<!-- I don't know what goes here. --> 
- Create handlers in Flask for GET and POST request types.
- Use the `value` attribute to spcify the data value that is sent to the server upon form submission.
<!-- I don't know what goes here. --> 
- Describe the differences betweem GET and POST, and what each request type should be used for.
<!-- I don't know what goes here. --> 
-  Describe common HTTP status codes by group (2xx, 3xx, 4xx, 5xx).
    - 2xx: Success
    - 3xx: Redirection
    - 4xx: Client Errors
    - 5xx: Server Errors
- Describe the common HTTP status codes: 200, 302, 400, 404, 405, 500.
    - 200: This is the standard response for successful HTTP requests.
    - 302: The HTTP/1.0 specification required the client to perform a temporary redirect.
    - 400: The server cannot or will not process the request due to an apparent clint error such as malformed request syntax.
    - 404: The requested source could not be found but may be available in the future.
    - 405: A request method is not supported for the requested source; for example, a GET request on a form that requires data to be presented via POST.
    - 500: A generic error message, given when an unexpected condition was encountered and no more specific message is suitable.
- Explain why we receive a 405 error when submitting a form to a handler with a decorator like `@app.route('/')`.
<!-- I don't know what goes here. --> 
- Use `str.format()` to create strings from template strings and data values.
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
