# CPD
CustomUser - PostgreSql - Docker

How to use?

If you want to get notified about the future changes Follow my github account + CustomUser.

First clone the project.

git clone https://github.com/imareef/CPD.git

Then make sure Docker is running.

    If you are on windows click on the Docker Desktop icon and wait for about a minute.

Then in the project directory run this command:

docker-compose up --build

It will create two containers: One for Django and one for PostgreSql as the database for the project. All the required packages will be installed.
Install a new package.

    Attention: If you want to install a package for django project you should run this command:

docker-compose exec web pip install <package-name>

Don't forget to add the new package to requirements.txt for further use:

docker-compose exec web pip freeze > requirements.txt
