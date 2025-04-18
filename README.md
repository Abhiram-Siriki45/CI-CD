### Continuous Integration-Continous Deployment 
************

## What is it?

Continuous Integration and Continuous Delivery/Deployment (CI/CD) is a Development Methodology, That solves typical problems found during the integration process. As multiple developers work in parallel, It becomes increasingly difficult to maintain a main branch that works and is free of bugs and errors. With CI/CD, Steps in the integration process are automated and the lifecycle of the app is constantly monitored. Ideally, this methodology will avoid "Integration hell", A situation where multiple developers that have been working on separate features on their own find it impossible to integrate all their code without major conflicts, and have to spend time reviewing all of their code to fix it.

For Reference, This is the definition of "Integration Hell" based on the [Agile glossary](https://www.solutionsiq.com/agile-glossary/integration-hell/):
> Integration Hell refers to the point in production, When the members of a delivery team integrate their individual code. In traditional software development environments, this integration process is rarely smooth and seamless, instead resulting in hours or perhaps days of fixing the code so that it can finally integrate. Continuous Integration (CI) aims to avoid this completely by enabling and encouraging team members to integrate frequently (e.g., hourly, or at least daily).

<img src="https://www.synopsys.com/content/dam/synopsys/sig-assets/images/agile-cicd-devops-difference.jpg.imgw.850.x.jpg" style="display: block; margin: auto; width: 50%">

## Continuous Integration

The goal of continuous integration (CI) is to quickly produce code that works. Successful CI means the changes to an app are built, tested and merged regularly. This integration can happen many times a day, and it usually involves automated test cases and a well-defined build sequence that minimizes errors. The main focus when using CI methodologies should be:
1. Smaller code: reduce the size of your contributions to the main branch, and make them instead more frequently. This will make it easy to detect bugs early and reduce conflicts with other contributions. Smaller integrations also mean test cases can run faster and your code becomes available to others that might be impacted by your feature.
2. Automated testing: Although there are CI "pipelines" that do not use automated testing, in practice automation vastly outweighs the benefits of manual testing. If a developer is integrating code several times a day, manual testing becomes troublesome, inconsistent and generally a waste of the developer's productivity.

## Continuous Delivery

This term is often used interchangeably with Continuous Deployment, but it can be nuanced. Usually Continuous Delivery will refer to how a developer is constantly *delivering* code that has already been tested for bugs. This does not mean the integrated code will be used in a live production environment. With Continous Delivery the process of pushing code from the developers' environment to the repository is automated, reducing the number of or eliminating the manual steps required.

## Continuous Deployment

Although it varies from team to team, Continuous Deployment will refer to code that, when integrated, is also deployed automatically to the live production site of the app. The reason this and Continuous Delivery are often both included in CD is because typical CI/CD pipelines will include both, and they both complement each other.

## Elements of a CI/CD pipeline

RedHat provides the following definitions in their article [What is a CI/CD pipeline?](https://www.redhat.com/en/topics/devops/what-cicd-pipeline):

The steps that form a CI/CD pipeline are distinct subsets of tasks grouped into what is known as a pipeline stage. Typical pipeline stages include:

* Build - The stage where the application is compiled.
* Test - The stage where code is tested. Automation here can save both time and effort.
* Release - The stage where the application is delivered to the repository.
* Deploy - In this stage code is deployed to production.
* Validate and check compliance - The steps to validate a build are determined by the needs of your organization. Image security scanning tools, like Clair, can ensure the quality of images by comparing them to known vulnerabilities (CVEs).
<br>
<br>

[![Maintened by - Abhiram-Siriki45](https://img.shields.io/badge/Maintained%20by-Abhiram%20Siriki45-red)](https://github.com/Abhiram-Siriki45)
