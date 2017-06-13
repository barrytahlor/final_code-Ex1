Remote Server

1) Add mongo

 add the key: (without the key, the repository will not load)

	>sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv EA312927

Now, create a new MongoDB repository list file:
	
	>sudo bash -c 'echo "deb http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.2 multiverse" > /etc/apt/sources.list.d/mongodb-org-3.2.list'

Complete the installation with update of repositories then install: update the packages list.

	>sudo apt update

install themongodb-org meta-package, which includes the daemon, configuration and init scripts, shell, and management tools on the server.
	
	>sudo apt install mongodb-org


	>sudo systemctl start mongod
	
check the status to verify that the service has started properly.


	>sudo systemctl status mongod

ensure that it restarts automatically at boot:

	>sudo systemctl enable mongod

 Start momgo

	>mongo


start the Mongo daemon:# learn-fullstack-javascript
Learning Fullstack JavaScript Development: MongoDB, Node.js, React.js
