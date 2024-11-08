# How to Run App 

# Note :::: Those Commands and repo is for Frontend and Cross Teams ONLY , and You should NEVER PUSH to the repo....

## Linux

#### Install docker
> sudo apt-get update

> sudo apt-get install ca-certificates curl -y

> sudo install -m 0755 -d /etc/apt/keyrings

> sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc

> sudo chmod a+r /etc/apt/keyrings/docker.asc

> echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

> sudo apt-get update

> sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin -y

> sudo chmod 777 /var/run/docker.sock

> sudo groupadd docker

> sudo gpasswd -a $USER docker

#### In terminal execute those commands to clone the repo

##### git clone http://github.com/Mazrof/app.git mazrof_app
##### cd mazrof_app
##### git submodule update --remote
#### Add .env file

#### In terminal execute ./up-linux.sh to up
#### In terminal execute ./down-linux.sh to stop

####  You should be able to access the Backend at http://localhost:3000 and the PgAdmin at http://localhost:4000 with password "mazrof" for the database server


## Windows
#### Install docker desktop
#### Run docker desktop
#### Open the powershell and execute the follwoing commands

##### git clone https://github.com/Mazrof/app.git mazrof_app
##### cd mazrof_app
##### rm back
##### git clone https://github.com/Mazrof/back.git back
#### Add .env file
##### docker compose up
#### Wait
#### You should be able to access the Backend at http://localhost:3000 and the PgAdmin at http://localhost:4000 with password "mazrof" for the database server
