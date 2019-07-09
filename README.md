# CordaLearning
![](https://i.ibb.co/KDnsFhW/687474703a2f2f7777772e636f7264612e6e65742f696d672f636f7264616c6f676f2e706e67.png)

# SongTrack
The proprietors of SongTrack approached Debut Infotech to create an entirely new decentralized system that could feature completely transparent transmission of artist loyalties, instant royalty payouts for artists & fans, real-time payments, and clarity of ownership. Our team of zealous Blockchain adepts went ahead and built a Corda-integrated DApp which gave investors full control of their digital assets without having to rely on third parties, middlemen or intermediaries, thereby reducing costs and increasing visibility. 

## Read case study
[click here](https://www.debutinfotech.com/pages/corda/images/SongTrack.pdf)


# Top View of Corda system 

![](https://i.ibb.co/j60hgLN/node-diagram.png)


# SongTrack Network structure
   - There are 3 Parties (Nodes maintaining DLT) and 1 Notary.
   - Node Artist and Node Fan to store information for Artist, Fan and trade related data.
   - Notary to verify uniquness or validate transactions.
     
     
 # System overview 
 ![](https://www.debutinfotech.com/pages/corda/images/sound-study.png)

 
 # SongTrack flow
  - step 1: Register Artist (localhost:10006/users/register-artist)
  - step 2: Register Fan (localhost:10009/users/register-artist)
  - step 3: Add song information (localhost:10006/artist/add-song)
  - step 4: Artist will issue royalty certificate for song (localhost:10006/issue-royaltyCertificate)
  - step 5: Fan will purchase royalty certificate(localhost:10009/purchase-royaltyCertificate)
  - step 6- Check currently available royalty certificate for investor. (localhost:10006/get-issued-royaltyCertificates)
    
 # Minimum System Requirements
    - 16 GB RAM preferably
    - Latest version of JAVA 8 java 8u181 (Preferably, Corda and kotlin support latest version of java 8)
    - http://docs.corda.r3.com/sizing-and-performance.html
    
 # Corda Background
    - States
    - Transactions
    - Contracts
    - Flows
    - Consensus
    - Notaries
    - Vault
    - Nodes
    
    
# Instructions for setting up

#### To download the application, execute the following commands
   ##### $ git clone https://github.com/debutdeveloper/SongTrack.git
 
### To set up the Corda application, it is needed to compile via Gradle
   - $ ./gradlew clean deployNodes
   - $ build/nodes/runnodes

### To set up and run the web servers 
   - $ cd clients
   - $ gradle clean build
   - $ java -jar build/libs/clients.jar
 
# Interacting with the nodes: 
##### To verify that client  live and running, navigate to the following URL:
####  http://localhost:8080/swagger-ui.html#/client-rest-controller

# RPC endpoints

|       Node     |        Url         |
| -------------- | -----------------  |
|     Artist     |  localhost:10006   |
|      Fan       |  localhost:10009   |
|    Notary      |  localhost:10003   |

    
    
    
    


    
    

