# Evaluation Test

Note: For all the following exercises optimize your pipeline to reach the most optimized code and pipeline performance/reliability.
Configure your repository as follow:

- [x]   Name should be your CTW number - CTW00000
- [x]   Create an additional branch - dev
- [x]   Create 3 environments: dev, test, prod
- [x]   Protect your main branch to only accept push from a Pull Request
- [x]   Configure a required status check to be passed before merge to main - use your test Job
- [x]   Configure a self-hosted runner in your ~~WSL 2 (Linux)~~ Real Linux Installation

1. Using your Node.js application from classes, create a pipeline named CI to:

- [x]   Test your app - npm test
- [x]   Analyse you app code with SonarQube
- [ ]   Build a tagged (v1) docker image with your app and store it as an artifact
- [ ]   Output the image name in your pipeline logs
- [ ]   Output the image name using Job Outputs

2. Create a pipeline named CD to:

- [ ]   Run your docker image and print the /api/latest-releases endpoint in your pipeline
- [ ]   Using the stored image from your previous exercise push a docker with your app to DockerHub

Configure your pipeline as follow:

- [ ]   CI pipeline is triggered on open Pull Request to main branch
- [ ]   CI pipeline should be possible to be triggered manually
- [ ]   CI pipeline should run on merge to main
- [ ]   CD pipeline should run on merge to main, after CI pipeline finished with success status

Extra Security configuration

- [ ]   Enable GitHub Advanced Security in your repository Settings with*  Default configuration
- [ ]   You should see Typescript/Javascript language is auto detected
- [ ]   Setup the CodeQL Analysis Workflow by GitHub - you should have a codeql.yml workflow after setup complete
- [ ]   Inspect your Security tab in your repository for Vulnerability alerts

Luck comes with preparation! Good luck! 🤗