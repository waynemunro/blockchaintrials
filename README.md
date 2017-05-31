# Blockchain Trials
Sample Code to get started with Blockchain


# Sample App using STRATO

Create STRATO instance on Azure
    https://azuremarketplace.microsoft.com/en-us/marketplace/apps/blockapps.strato-blockchain-lts-vm?tab=Overview

OR install the developer trial edition
    https://github.com/blockapps/strato-getting-started

Install blockapps-bloc
    https://www.npmjs.com/package/blockapps-bloc
		
Create Sample App 

    $ npm install -g blockapps-bloc
	
    $ bloc init  (set app name "firstapp")
    
    ## Change the config.yaml with the correct API url from the test drive
    
    $ npm install

    ## npm install -g solc
	
    $ bloc genkey  
    
    ## Make sure to enter entropy password and remember it. It creates admin account first, see "admin" folder under app/users and inside it a json file with all the details
    
    ## Use bloc genkey testuser  (this creates an account with name "testuser")

    $ bloc compile SimpleStorage

    $ bloc upload SimpleStorage   (use the entropy password to retrieve private key)

    ## See the updated files in the app/meta/SimpleStorage folder

    $ bloc start

    ## Use Post Man or Fiddler to brower through various API's
    ## GET http://localhost:8000/users
    
# STRATO Pizza Demo

    https://github.com/blockapps/pizza-demo

    ## Deploy it in the same VM instances as STRATO

    $ git clone https://github.com/blockapps/pizza-demo.git

    ## Change Port 9001 to 9011 in DockerFile, docker-compose.yml and Gruntfile.js

    $ sudo docker build -t pizza --build-arg STRATO=ubuntudev.westus.cloudapp.azure.com .

    $ sudo docker-compose up

    ## Open http://ubuntudev.westus.cloudapp.azure.com:9011/

    





