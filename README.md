# Data engineer position at Sephora: First test

You can write your code in the language of your choice. But we have preferences for the language of our stack:

- Python
- Go
- NodeJS

We're also interested by these languages:

- Scala
- Haskel
- R
- Rust

Please organise, document and write some tests.
Also precise if a specific setup is required to make your code run.

## Data structure

1. Write a clean binary tree structure (from scratch, no external library!) in your favorite language.
2. Populate it with few samples.

*Now, imagine this tree is a depedance tree. Each node is a task (a function/procedure) which has to be ran, but not before all it's children's tasks are all executed and done.*

3. How would you search this tree to run the tasks in a correct order?
4. Apply on your structure, and test it

*Going further, we would like to parallelize the execution of few of these tasks: tasks from different nodes can work simultaneously, but, still, must not be executed before it's children's tasks are done.*

5. If you had to parallelize these tasks' executions, how would you do that?
6. Apply on your tree structure, and test it

*Sample of task function (in js):

```js
function task (callback){
    setTimeout(callback, parseInt(1000 * Math.random()));
}
```