# GitLab CI/CD

- GitLab CI/CD is also another CI/CD plateform like Jenkins
- CI/CD is in the heart of DevOps process.
- It is a method to frequently deliver application changes to customer end in automated way.
- Complete CI/CD Process

  - CI - Continuos Integration

    - Code Push to Remote Repo
    - Test
    - Build & Package
    - Artifact Repository

  - CD - Continuos Deployment

    - Deploy to Dev/Staging
    - Testing UI and Changes
    - Deploy to Prod

  - CD - Continuos Delivery
    - Deploy to Dev/Staging
    - Testing UI and Changes
    - Manual agreement by someone responsible
    - Deploy to Prod

# GitLab CICD vs Jenkins vs Azure DevOps

    - GitLab CICD
        1. GitLab is new to industry and its community is in growing phase.
        2. Many Feature Built-In: Self-Monitoring, Container Registry, Docker CI Runner etc.
        3. Allows Keeping CICD and Code Management at same place
        4. Open Source or Commercial (Both) and Self-Hosted or SAAS

    - Jenkins
        1. Jenkins is old, industry leader, powerful, open-source tool and have big community.
        2. Feature can be integrated through multiple plugins; Maintenance Required.
        3. Only CICD Tool, Code mangement not possible
        4. Self Hosting Required and is only option (OpenSource/Self-Managed)

    - Azure DevOps
        1. Azure DevOps is cloud based CICD tools and community still growing
        2. Best Integration for features can be easily possible with Microsoft Services. Other tool integrtion not so easy to integrate.
        3. Commercial/SAAS Tool

### In Complete Learning, We use GitLab on Self-Hosted Servers.

# GitLab Basic CICD Pipeline
### Job Name Limitations
- We Can't Use these keywords as jobs-name
    - image, services, stages, types, before_script, after_script, variables
    - cache, include, true, false, nil

- .gitlab-ci.yml -> It is a yaml based scripted pipeline file where we define all the action or workflows. (Jenkinsfile in Jenkins)
- Jobs -> Jobs are the most fundamental building block of pipelines. (Steps in terms of Jenkinsfile)
    - example 
        ```yml
            job1:
                script: "execute-script-for-job-1"
            job2:
                script: "execute-script-for-job-2"
        ```
![Gitlab-Jobs-Image](https://github.com/nirdeshkumar02/GitLab-CICD/blob/master/job.png)
