# Components of GitHub Actions

![Components of GitHub Actions](./images/github-actions-components.jpg){: style="width:100%"}

## **Workflow**

A workflow is a configurable automated process for a repository. Workflows are triggered by an event in the repository, manually, or on a schedule. Workflows are defined in a YAML file in the `.github/workflows` directory of a repository. A repository can have multiple workflows, and each workflow can have one or more jobs.

Workflow Examples: CI, Release, Publish Documentation, etc.

## **Jobs**

A job is a specific task performed within a workflow. It consists of multiple steps and is executed in order to complete the task. A job runs on a specific runner. Jobs in a workflow can run in parallel, and you can also configure dependencies between jobs.

Job Examples: Build and test code, Push a container to a registry, etc.

## **Steps**

A step is either a script that will be executed or an action that will run. Steps in a job depend on each other, and since all steps are executed on the same runner, you can share data from one step to another.

Step Examples: Install dependencies, Build, Test, etc.

## **Actions**

An action is a part of a step that performs a complex but frequently repeated task. Actions help reduce the amount of repetitive code in your workflow files. You can write your own reusable actions or find existing actions in the [GitHub Actions Marketplace](https://github.com/marketplace?type=actions).

Action Examples: Set up code, Install Python, Authenticate to a cloud provider, etc.
