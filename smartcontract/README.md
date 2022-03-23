## HARDHAT SETUP FOR BACKEND

### Requirements
Alchemy key
Metamask key
Etherscan.io API Url

### STEPS
cd into smartcontract
install hardhat: npm i -D hardhat
setup basic project: npx hardhat   
install dependencies: npm install --save-dev "hardhat" "@nomiclabs/hardhat-waffle" "ethereum-waffle" "chai" "@nomiclabs/hardhat-ethers" "ethers" "web3 @nomiclabs/hardhat-web3" "@openzeppelin-solidity/contracts" "dotenv" "@nomiclabs/hardhat-etherscan" "@openzeppelin/contracts" 
write code
setup .env file
retrieve alchemy, metamask & etherscan keys and setup hardhat.config


### COMPILE
compile the smartcontract before deployment: npx hardhat compile

### DEPLOY
To deploy: npx hardhat run scripts/deploy.js --network rinkeby
To verify smartcontract: npx hardhat verify DEPLOYED_ADDRESS --network rinkeby


## HARDHAT SETUP FOR FRONTEND
cd into client
setup vite: npm install vite@latest
install package dependencies: npm install
install tailwind: npm install -D tailwindcss postcss autoprefixer
create tailwindcss and postcss config files: npx tailwindcss init -p