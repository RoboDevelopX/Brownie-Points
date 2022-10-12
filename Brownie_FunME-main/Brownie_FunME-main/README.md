# Brownie_FunME
Smart Contract "FUND ME"

Es un sistema de contrato inteligente desplegado y desarrolado en python
Lenguajes: Ethereum Python & Solidity
Framework: Brownie
Otras Dependencias: Infura, Alchemy, Ganache, Chainlink, Git, 


Install pip3: 
	web3
	Brownie
	py-solc-x 
	pytest

1 brownie Compile

2 brownie run scripts/deploy.py --network rinkeby
	
	EtherScan: contract > virify and publish 

	 	- Crear  API ETHERSCAN TOKEN
	 	- Crear API INFURA TOKEN
	 	- Crear Cuenta en alchemy.io (...) crear una nueva APP: 
			** En view key: HTTP, wEBSOCKETS **
	
	 
3 brownie run scripts/deploy.py --network rinkeby
 
4. deploying to Ganache

 brownie compile
 
 - brownie networks list
 
 - brownie networks add Ethereum ganache-local host=https://0.0.0.0:8545 chainId=1337
 - brownie networks list
 - brownie run scripts/deploy.py networks ganache-local
 - brownie run scripts/fund_and_withdraw.py networks ganache-local
 
 - brownie test
 - brownie test --network development
 
 - brownie test -k test_only_owner_can_withdraw --network rinkeby
 - brownie networks add development mainnet-fork-dev cmd=ganache-cli host=https://127.0.0.1 fork='https://{alchemyapi.io - view key: HTTP}' accounts=10 mnemonic=brownie port=8545
 - brownie run scripts/deploy.py --network mainnet-fork


Crear Cuenta en alchemy.io (...) crear una nueva APP 
	- En view key: HTTP, wEBSOCKETS
	
- brownie test --network mainnet-fork-dev
