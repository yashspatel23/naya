# NAYA

### Naya Token
Contract: 0xc8fA943b1449E8446365f16c9A40062430336C0B
BSC: https://testnet.bscscan.com/address/0xc8fa943b1449e8446365f16c9a40062430336c0b

#### Setup

1. Set Vault Address (Where the tokens are going to be minted)
    - setVault (address ADDRESS) - this method has to be called with the contract creator address

2. Mint new tokens. Remember, these tokens are with 9 decimal points and so its the number of tokens you want followed by 9x 0's.
    - Only vault owner can mint new tokens.
    - mint (address ADDRESS, uint256 AMOUNT)


#### Methods:

- pushManagement (address): set a new owner of the contract _newOwner
- pullManagement: new owner of the contract accepting the role and setting themselves as _owner
- renounceManangement: CAREFUL: give up control of the smart contract. There no longer exists an owner of the contract.

- burn (amount): Burn these number of tokens to null address.
- burnFrom

- decreaseAllowance
- increaseAllowance

- permit

- transfer (address, amount): address you want to send amount of tokens.
- transferFrom



### sNaya Token
Contract: 0x5992825b79b7A0A6e9B56c1f29f4b7ec3BA5E41D
BSC: https://testnet.bscscan.com/address/0x5992825b79b7a0a6e9b56c1f29f4b7ec3ba5e41d

#### Setup

1. Call initialize method with the staking address.
    - initialize (address STAKINGADDRESS)


#### Methods

- initialize (address): Write staking address here (0xBEDA827142D9E743687cD3C6e2ccb608d8F15160)

- approve
- decreaseAllowance
- increaseAllowance
- permit

- pushManagement (address): set a new owner of the contract _newOwner
- pullManagement: new owner of the contract accepting the role and setting themselves as _owner
- renounceManangement: CAREFUL: give up control of the smart contract. There no longer exists an owner of the contract.

- rebase
- setIndex

- transfer
- transferFrom



### Staking Contract
Contract: 0xBEDA827142D9E743687cD3C6e2ccb608d8F15160
BSC: https://testnet.bscscan.com/address/0xbeda827142d9e743687cd3c6e2ccb608d8f15160

### Deploy

address _OHM: 0xc8fA943b1449E8446365f16c9A40062430336C0B, 
address _sOHM: 0x5992825b79b7A0A6e9B56c1f29f4b7ec3BA5E41D, 
uint _epochLength: 9600,
uint _firstEpochNumber: 0,
uint _firstEpochBlock: 15755727

### Setup

1. claim first

### Methods

- claim
- forfeit
- giveLockBonus

- pushManagement (address): set a new owner of the contract _newOwner
- pullManagement: new owner of the contract accepting the role and setting themselves as _owner
- renounceManangement: CAREFUL: give up control of the smart contract. There no longer exists an owner of the contract.

- rebase

- returnLockBonus

- setContract
- setWarmup

- stake
- unstake

- toggleDepositLock



### Staking Helper Contract
Contract: 0x7e14137aD02A385a84cDB0D15261ba38417AC068
BSC: https://testnet.bscscan.com/address/0x7e14137aD02A385a84cDB0D15261ba38417AC068

#### Deploy

address _STAKING
address _OHM

#### Setup

#### Methods

- stake (amount) - amount to stake






TREASURY NOTES

ENABLE OPTIMIZATION - RUNS: 200

CONSTRUCTOR VALUES:
Naya Address: ABOVE
BUSD Address: 0xe9e7cea3dedca5984780bafc599bd69add087d56
blocksNeededForQueue: 0

