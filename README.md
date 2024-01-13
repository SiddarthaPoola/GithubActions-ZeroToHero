
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

After update the first-actions.yml, my build has been started and succeeded.

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/980a83ff-3165-4379-aff0-885f678bc310)

You can check your selfhosted runner that is EC2 instance

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/d9e85824-f043-4b0e-8fd7-4615f227ac79)

ONce the build has been succeeded the you can see the green tick mark in the repository

![image](https://github.com/kohlidevops/GithubActions-ZeroToHero/assets/100069489/24b3f031-09e1-4dee-9c82-67f0bfb25a77)

Thats it!
