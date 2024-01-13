# GitHub-Actions-Zero-to-Hero
Repository to kick start your journey with GitHub Actions

## Comparing with Jenkins 

### Advantages of GitHub Actions over Jenkins

- Hosting: Jenkins is self-hosted, meaning it requires its own server to run, while GitHub Actions is hosted by GitHub and runs directly in your GitHub repository.

- User interface: Jenkins has a complex and sophisticated user interface, while GitHub Actions has a more streamlined and user-friendly interface that is better suited for simple to moderate automation tasks.

- Cost: Jenkins can be expensive to run and maintain, especially for organizations with large and complex automation needs. GitHub Actions, on the other hand, is free for open-source projects and has a tiered pricing model for private repositories, making it more accessible to smaller organizations and individual developers.

### Advantages of Jenkins over GitHub Actions

- Integration: Jenkins can integrate with a wide range of tools and services, but GitHub Actions is tightly integrated with the GitHub platform, making it easier to automate tasks related to your GitHub workflow.

In conclusion, Jenkins is better suited for complex and large-scale automation tasks, while GitHub Actions is a more cost-effective and user-friendly solution for simple to moderate automation needs.


### To set up Github selfhosted runner

#### To launch EC2 instance

To launch ubuntu22 EC2 instance and install below commands on ubuntu machine

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/2f230961-e78f-4247-9cf7-91c14aab768a)

```
#!/bin/bash
sudo apt-get update -y
sudo apt-get upgrade -y
sudo apt-get install net-tools -y
sudo apt-get install zip unzip -y
```

#### You can use below link github link to work on it

```
https://github.com/kohlidevops/GithubActions-ZeroToHero.git
```

#### To add Github Self hosted runner

Navigate to Github -> Select your repository (GithubAction-ZeroToHero is my repo)

Repository -> Settings -> Actions -> Runners -> Add new selfhosted runner

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/d24a497a-913b-43ee-ad01-9b93668c3f41)

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/23be8f1d-e176-4a42-aceb-c4c497ada977)

Now you have download and configure the selfhosted runner with the help of commands that provided by Github

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/d67bba2e-f28c-406c-89c9-152beb16efe9)

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/39f86f08-626a-4b54-8831-91909f18a031)

Finally run

```
./run.sh
```

Then add the "self-hosted" in .github/workflows/first-actions.yml

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/8839b0d2-b0fd-4314-8729-28633e7177b3)
