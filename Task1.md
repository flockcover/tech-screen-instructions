Bob's Epic Drone Shack Inc. manufactures drones. They have made an API available at
[bobs-epic-drone-shack-inc.herokuapp.com](https://bobs-epic-drone-shack-inc.herokuapp.com) listing all of their products and providing safety information about them. The API is poorly documented, and fails frequently with a variety of status errors. The documentation lists the following routes:

GET -> /api/v0/drones

GET -> /api/v0/drone/:id

No other documentation is provided.

Unfortunately, the server is unstable, due to the limited resources and technical expertise available to Bob. Build an in house caching layer on top of Bob's Epic Drone Shack. Your solution should be a webserver with a routing structure of your choice. It should forward requests sensibly to Bob's Epic Drone Shack. If the request is succesful, it should use the response and forward it to the requestor, before caching the response, using sensible caching technology of your choice, and expiring the previous value if necessary. If Bob's Epic Drone Shack responds with a failure code, you should fetch the latest cache if it is available, and retry the request if it is not.

If you have never worked with caching in the past, this problem is frequently addressed using Redis, Memcached, or Varnish. Other solutions are also possible.

## Submission guidelines
- Please ensure that your submission is runnable. Bonus points if in addition to the code, you deploy this to a PaaS provider of your choice.
- Please submit your code as a link to a Version Control System of your choice. We would love to see your commit process.
- Assume the code you write could evolve into a more fully fledged product, and architect your code accordingly.
- In addition to your code, please submit a brief document (as a README or otherwise), answering the following questions(brief answers will suffice):
  1) What assumptions did you have to make?
  2) Which technologies did you choose? Why?
  3) What technical compromises did you have to make in order to achieve your solution? What is the severity of this tech debt, and what would a path to resolving it look like?
  4) How do we run your code?
  5) What future features do you think we might be able to build based on this API?
