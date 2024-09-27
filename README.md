# firstGithubAction

# Github action is free
Did not know Github provides such a free service for CI/CD, which is very good.

# what is the use of Github action
Automate testing and checking your code base.

It is usually written in the form of `yml` file, where you specify certain actions to take when you pushed the code into a repo. In our repo here, we put in a basic linter checking action - checking if your code conform to writing standards e.g. space and lines etc.

In the yml file, it will contains below config:
1. Events - usually on the action when push code into repo
2. jobs
3. runners
4. steps - steps to run
5. Actions

Github action provide free workers/servers to do this action - Ubuntu in this case.

# How to set up the yml file
It must be inside the repo with the format of `.github/workflows/yourAction.yml`. Then github automatically knows this is a Github action.

# How to integrate with deployment
When the pushed code passed the Github action test, it will show a green tick or passed status.

Through Github API, then you could use your servers to pull the code down for staging or production deployment when your code passed the test.

# Github action marketplace
This a place for many yml templates, so that you do not have to create from scratch.
