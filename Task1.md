# Flock Tech Screen
Bob's Epic Drone Shack Inc. manufactures drones. As a community service they have made an API available at
[bobs-epic-drone-shack-inc.herokuapp.com](https://bobs-epic-drone-shack-inc.herokuapp.com) listing all of their products and providing safety and other information. The API is poorly documented, and fails frequently with a variety of status errors. The documentation lists the following routes:

GET -> /api/v0/drones

GET -> /api/v0/drone/:id

No other documentation is provided.

Unfortunately, the server is unstable, due to the limited resources and technical expertise available to Bob. Build an in house caching layer on top of Bob's Epic Drone Shack. Your solution should be a webserver with a routing structure of your choice. It should forward requests sensibly to Bob's Epic Drone Shack. If the request is succesful, it should use the response and forward it to the requestor, before caching the response, using sensible caching technology of your choice, and expiring the previous value if necessary. If Bob's Epic Drone Shack responds with a failure code, you should fetch the latest cache if it is available, and retry the request if it is not.

If you have never worked with caching in the past, this problem is frequently addressed using Redis, Memcached, or Varnish. Other solutions are also possible.

## Submission guidelines
- Please ensure that your submission is runnable. Non-executing submissions will be diqualified without further review. Bonus points if in addition to the code, you deploy this to a PaaS provider of your choice (unless your solution is a mobile solution, we understand that makes this impossible, and will not mark you down).
- Please submit your code as a link to a version control system of your choice. We would love to see your commit process.
- Assume this is a spike which could evolve into a fully fledged product, and architect your code accordingly.
- In addition to your code, please submit a brief document (as a README or otherwise), answering the following questions:
  1) What assumptions did you have to make?
  2) Which technologies did you chose? Why?
  3) What technical compromises did you have to make in order to achieve a solution? What is the severity of this tech debt, and what would a path to paying it down look like?
  4) How do we run your code?
  5) What future features do you think we might be able to build based on this API? How would the server you have written have to evolve to accomodate?
