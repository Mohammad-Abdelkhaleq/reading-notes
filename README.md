# reading-notes
![note place holder](https://media.wired.co.uk/photos/606d9e60fd9831b13e447105/master/w_1600%2Cc_limit/notespr.jpg)

this website is to list my **notes** and track my progress in web development

<!-- - ### Code 102 - *Intro to Software Development*
- ### Code 201 - *Foundations of Software Development*
- ### Code 301 - *Intermediate Software Development* -->
<hr>

- ### Code 401 - *Class 1 readings *

**How would you describe Node to a non-technical friend?**

*Node.js is like a powerful engine that allows developers to run JavaScript outside of web browsers. Just like how you can use JavaScript to make things happen on a website, Node.js lets you use JavaScript to build all sorts of things on a computer, It's a popular tool because it's fast, efficient, and can handle many things happening at the same time without slowing down. So, think of Node.js as a way for developers to use JavaScript to build cool stuff that runs on computers and servers, not just in web browsers* 

**What does it mean that Node is a JavaScript runtime?**

*it means that Node.js provides an environment for executing JavaScript code outside of a web browser. It allows you to run JavaScript code on the server-side, rather than just in the browser*

**What is Node used for?**

*Node is particularly suited to building applications that require some form of real-time interaction or collaboration*

<hr>


- ### Code 401 - *Class 2 readings *

**Explain middleware, answer as though I were a non-technical recruiter.**

"middleware functions typically perform some operation on the request or response and then call the next function in the "stack", which might be more middleware or a route handler."
it is basically a code that perform some operations on a request to the server and also on the output of the server 

**Express the most popular __ __ ____.**

 Express is the most popular **Node web framework** 

 **Express is “unopinionated.” What does that mean?**

 "Opinionated frameworks are those with opinions about the "right way" to handle any particular task. They often support rapid development in a particular domain (solving problems of a particular type) because the right way to do anything is usually well-understood and well-documented. However they can be less flexible at solving problems outside their main domain, and tend to offer fewer choices for what components and approaches they can use."

  **What is a module and why is modularity useful to us as developers?**
  it allows us apply these concepts on our code Reusability, Maintainability, Collaboration and  Scalability and allow easer testing to our application 

**What version of npm are you running on your machine?**

 npm: '9.5.0'

 **What command would you type to install a library/package called ‘jshint’ into your node project?**

 npm i jshint

 **Explain why tests are important. Please explain as though I were your non technical elder.**

 testing is important to avoid unexpected errors before merging to the main code and to test as many senarios as possible contineously and the tester can ba a third party also.

 **What are three expected benefits of testing**
 - many teams report significant reductions in defect rates, at the cost of a moderate increase in initial development effort
 - the same teams tend to report that these overheads are more than offset by a reduction in effort in projects’ final phases
 - although empirical research has so far failed to confirm this, veteran practitioners report that TDD leads to improved design qualities in the code, and more generally a higher degree of “internal” or technical quality, for instance improving the metrics of cohesion and coupling

 **Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.**
 Typical individual mistakes include:
 - forgetting to run tests frequently
- writing tests that are too large or coarse-grained

Typical team pitfalls include:

- partial adoption – only a few developers on the team use TDD
- poor maintenance of the test suite – most commonly leading to a test suite with a prohibitively long running time

**What are three benefits of Continuous Integration?**
- Enhanced Collaboration and Code Quality
- Faster Feedback Loop
- Early Detection of Integration Issues

**What is the difference between Continuos Delivery and Continuous Deployment?**

The main difference between Continuous Delivery and Continuous Deployment lies in the release stage. In Continuous Delivery, the software is ready for deployment, but the release decision is made manually. In Continuous Deployment, the software changes are automatically released to production once they pass the necessary tests and criteria.

**Explain how GitHub fits into this process assuming the listener comes from a non-technical background**

using github make it easier for teams to work together on software projects using Continuous Delivery or Continuous Deployment.
