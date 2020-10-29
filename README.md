# <div align="center">Deployment process instruction (vanhelsing.cf)</div>

# General information
> * 1-core instance, 1 GB RAM, Ubuntu installed
> * nginx web server is installed on the server
> * CF-plugin acme.sh for a free Let's Encrypt certificate

The production version of the site runs on the `domain vanhelsing.cf`, the dev version is `dev.vanhelsing.cf` 

**be careful! Access to the server is not provided, editing site files is carried out through the version control system - git**

## Deployment process

> * Gitlab permissions will be issued to you in the Developer role

> * Step 1: log in to gitlab.com

> * Step 2: go to the Repository item, you will see a list of all the files and directories of your site

<div align="center">![Step 2](https://files.access.pp.ua/step_2.png)</div>

> * Step 3: you can edit files directly in gitlab.com, for this you need to select the desired file from the list and click the blue `Edit button`

<div align="center">![Step 3](https://files.access.pp.ua/step_3.png)</div>

<div align="center">![Step 3](https://files.access.pp.ua/step_3_1.png)</div>

> * Step 4: edit our site code

<div align="center">![Step 4](https://files.access.pp.ua/step_4.png)</div>

> * Step 5: make a commit (save our changes) in the `сommit message` enter what changes in the code are valid

<div align="center">![Step 5](https://files.access.pp.ua/step_5.png)</div>

> * Step 6: Deploy.
> When we commit, the code will automatically load into dev environment, go to the menu `CI / CD -> jobs`

<div align="center">![Step 6](https://files.access.pp.ua/step_6.png)</div>

> If you are satisfied with the changes on the site (I recall the address dev environment - https://dev.vanhelsing.cf) go to the CI / CD 
-> jobs menu and start the manual deployment in the prod environment with the `Play button on the right`

<div align="center">![Step 6](https://files.access.pp.ua/step_6_1.png)</div>
