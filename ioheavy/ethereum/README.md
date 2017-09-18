# Experiment Setup

* Requirments:  sudo apt-get install npm & npm install web3@0.19 
* Modify the deploy.js to give the password for eth.account[0]
* use `node deploy.js` to deploy the smart contract into blockchain(ethereum). It will output the deployed smart contract address
into `stdout`.

# Run

* Write: `node write.js start_key total_key_num sig contract_address` write `total_key_num` key-value pairs starting with key `start_key` sequentially.
  `sig` is a id stamp of this request used for distinguish this request from the others (due to some web3.js library bugs, this is needed). `contract_address`
  is the deployed smart contract address returned by `deploy.js`.
* Scan: `node scan.js star_key total_key_num sig contract_address` scan `total_key_num` key-value pairs starting with key `start_key` sequentially.
  `sig` is a id stamp of this request used for distinguish this request from the others (due to some web3.js library bugs, this is needed). `contract_address`
  is the deployed smart contract address returned by `deploy.js`.

 
