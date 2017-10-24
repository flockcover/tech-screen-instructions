# Flock Tech Screen
Bob's Epic Drone Shack Inc. manufactures drones. As a community service they have made an API available at
[bobs-epic-drone-shack-inc.herokuapp.com](https://bobs-epic-drone-shack-inc.herokuapp.com) listing all of their products and providing safety and other information. The API is poorly documented, and fails frequently with a variety of status errors. The documentation lists the following routes:

GET -> /api/v0/drones

GET -> /api/v0/drone/:id

No other documentation is provided.

Using tools of your choice, build a UI which enumerates the results of `GET -> /api/v0/drones` in a readable manner. Given that we are an insurance provider, you should furthermore attempt to see if there is any useful information, and highlight it as you deem appropriate or provide any other features you feel would demonstrate this API's utility. As you want to demo this integration to a potential customer, make sure that the API's notorious instability and failure rate is appropriately handled.

## Submission guidelines
- Please ensure that your submission is runnable. Non executing submissions will be diqualified without further review. Bonus points if in addition to the code, you deploy this to a PaaS provider of your choice (unless your solution is a mobile solution, we understand that makes this impossible, and will not mark you down).
- Please submit your code as a link to a version control system of your choice. We would love to see your commit process.
- Assume this is a spike which could evolve into a fully fledged product, and architect your code accordingly
- In addition to your code, please submit a brief document (as a README or otherwise), answering the following questions:
  1) What assumptions did you have to make?
  2) What technical compromises did you have to make in order to achieve a solution? What is the severity of this tech debt, and what would a path to paying it down look like?
  3) How do we run your code?
  4) What future features do you think we might be able to build based on this API?
