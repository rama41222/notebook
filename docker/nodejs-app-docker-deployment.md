### NodeJS EC2 docker deployment

###### Provision an EC2 Instance


- Create an EC2 instance
- SSH into the EC2 instance
```
$ ssh -i "sshkeyfile.pem" ubuntu@hostname
```

###### Installing Docker on ubuntu 18.04


1. First, update the packages index and upgrade your system 
    ```
    sudo apt update
    sudo apt upgrade
    ```
2. Install the dependencies necessary to enable a new repository over HTTPS.
    ```
    sudo apt install apt-transport-https ca-certificates curl software-properties-common
    ```
3. Import the repository’s GPG key 
    ```
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
    ```
4. Add the Docker APT repository
    ```
    sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
    ```
5. Now that the Docker repository is enabled, update the apt package list and install the latest version of Docker CE
    ```
    sudo apt update
    ```
6. Install Docker CE
    ```
    sudo apt install docker-ce
    ```
7. Check the Docker Status
    ```
    sudo systemctl status docker
    ```
    
### Docker Compose

1. Import the repository
    ```
    sudo curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
    ```
2. Set the permissions
    ```
    sudo chmod +x /usr/local/bin/docker-compose
    ```
3. Now **docker-compose** should be working. Use the following command to check the version
    ```
    docker-compose --version
    ```
    
### API      
 
1. Create the .env file and input all the env variables
    ```
    touch .env
    ```
    
### Run      

1.  Use the docker compose file to run the api
    ```
    docker-compose build && docker-compose up
    ```

#### Further
*  `docker-compose down` # Remove a Service 
*  `docker-compose start` # Start a Service
*  `docker-compose stop` # Stop a Service
*  `docker-compose run <service_name>` # Run Specific Service
