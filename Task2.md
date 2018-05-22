Bob's Epic Drone Shack Inc. manufactures drones. They have made an API available at
[bobs-epic-drone-shack-inc.herokuapp.com](https://bobs-epic-drone-shack-inc.herokuapp.com) listing all of their products and providing information about these products. The API is poorly documented, and fails frequently with a variety of status errors. The documentation lists the following routes:

GET -> /api/v0/drones

GET -> /api/v0/drone/:id

No other documentation is provided.

1) Using tools of your choice, build a UI which lists the results of `GET -> /api/v0/drones` in a readable manner. 
2) The API is unstabile and has a high failure rate. You are tasked with building an integration that masks this from the end user. Your solution should be reliably demoable despite the broken API.
3) (Bonus - only attempt if you have time): The API returns drone crash statistics. Build a UI which allows you to filter the drones by crash rate range (for example: between 0-10%).

## Submission guidelines
- Please ensure that your submission is runnable. Bonus points if in addition to the code, you deploy this to a PaaS provider of your choice.
- Please submit your code as a link to a version control system of your choice. We would love to see your commit process.
- Assume this is a spike which could evolve into a fully fledged product, and architect your code accordingly.
- In addition to your code, please submit a brief document (as a README or otherwise), answering the following questions:
  1) What assumptions did you have to make?
  2) What technical compromises did you have to make in order to achieve a solution? What is the severity of this tech debt, and what would a path to paying it down look like?
  3) How do we run your code?
  4) What future features do you think we might be able to build based on this API?
