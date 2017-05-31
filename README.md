# Blockchain Trials
Sample Code to get started with Blockchain


# Sample App using STRATO

Create STRATO instance on Azure
    https://azuremarketplace.microsoft.com/en-us/marketplace/apps/blockapps.strato-blockchain-lts-vm?tab=Overview

OR install the developer trial edition
    https://github.com/blockapps/strato-getting-started

Install blockapps-bloc
    https://www.npmjs.com/package/blockapps-bloc
		
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
    




