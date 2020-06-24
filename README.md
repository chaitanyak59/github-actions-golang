# Github Actions Demonstration
This Project illustrates the usage of GithubActions with a simple Golang Code

## Getting Started
Idea is to exploit the basic options and usage of Actions in Github. <br>
This example uses Github Hosted Runners. <br>
Following are covered:
- Matrix Strategy (Using combinations of Platform and Go version)
- Publishing Custom Docker Image to Docker Registry
- Trigger Lint Checks for a Golang Project


### Prerequisites
1) Understand Github Actions , [Go to Documentation](https://help.github.com/en/actions)
2) Basic Understanding of CI and CD

### Souce Code Details

Under .github./workflows folder, you'll find the yml configuration for each workflow.
Tip: Filename explains its usage

```
1) lint.yml
This configuration runs on ubuntu-18.04 runner,
which wil trigger golang lint action.
```

```
2) docker-flow.yml
This configuration runs on ubuntu-18.04 runner,
which has 2 custom actions
 a) Building Docker Image
 b) Publishing to Docker Registry using an existing github action

Note: To use this illustration, make sure that you add your username and password under secrets tab(under settings) of Github
```

```
3) matrix-flow.yml
This configuration runs on ubuntu-18.04 runner,
which has custom strategy to run the Workflow in
 - Multi Platforms X Multi GO versions

Note: Please go thru matrix_test JOB for understanding
```

## Built With

* [Github Actions](https://help.github.com/en/actions) 

## Authors

* **Chaitanya Kumar** -[Github](https://github.com/chaitanya-apty)

