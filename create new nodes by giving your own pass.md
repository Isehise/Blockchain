create new nodes by giving your own password: geth --datadir node1 account new geth --datadir node2 account new
make a note of the two public keys: node1: 0xD965Cc8ab09fAdB25bb039556a03A089550b794 node 2: 0xbe9F9a2499E9afBD7c92B5d0656b207dF002912

![GenesisConfiguration.PNG](https://github.com/Isehise/Blockchain/blob/main/GenesisConfiguration.PNG)


run puppeth under the tool directory to generate your genesis block

![Puppeth_complete.JPG](https://github.com/Isehise/Blockchain/blob/main/Puppeth_complete.JPG)


initilize nodes geth --datadir node1 init ./anyware.json geth --datadir node2 init ./anyware.json

begin mining by opening two terminals. type in password. ../geth --datadir node1 --unlock 0xD965Cc8ab09fAdB25bb039556a03A089550b794 --mine --rpc --allow-insecure-unlock
../geth --datadir node2 --unlock  0xbe9F9a2499E9afBD7c92B5d0656b207dF002912 --mine --port 30304 --bootnodes "enode://""
open mycrypto, change network to customized one With network name: anyware; chain ID=50599

![NodeTransaction.PNG](https://github.com/Isehise/Blockchain/blob/main/NodeTransaction.PNG)

Send test transactions

![SuccessfulTransaction.PNG](https://github.com/Isehise/Blockchain/blob/main/SuccessfulTransaction.PNG)


