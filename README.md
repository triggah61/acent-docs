
# ACENT BLOCKCHAIN TECHNICAL PAPER

## INTRODUCTION

The current Web 2.0 technology is meant to allow users to generate, collaborate, and share content over the internet and enables interactions such as peer-to-peer (P2P), business to consumer (B2C), and business to business (B2B). However, the current system ultimately favors entities that track and take advantage of users by collecting private data and providing unsecure systems subject to reckless profiteering and information manipulation.

ACENT offers a solution that favors and protects users in the form of the Osiris Web 3.0 browser that prioritizes user privacy and security, and speed.

The ACENT Blockchain empowers the Osiris web 3.0 browser, a decentralized net-neutral browser that can render web 2.0 and blockchain technologies. ACENT (ACE) is the native utility token of the Osiris browser and it provides a secure and convenient way to settle payments and other economic activities in the ACENT ecosystem.

ACENT ACE is currently in the format of ERC20 utility token in the Ethereum chain but will soon be migrated to the ACENT blockchain. It is a functional utility cryptocurrency that serves as the medium of exchange between participants using Osiris browser and its built-in multi-cryptocurrency wallet by supporting decentralized applications on the ACENT blockchain. ACENT also distributes economic incentives to encourage user contribution, governance participation, and maintenance of the ACENT ecosystem on Osiris through the proliferation of decentralized internet infrastructure (hereon referred to as decenternet).

ACENT blockchain is determined to improve the blockchain ecosystem by solving known problems and implementing the following improvements:

1. **Acent is 100% compatible with Ethereum developer environment tools**
 All Ethereum DApps can be migrated as-is into the Acent ecosystem. DApps such as Cryptokitties or Uniswap can easily be migrated or be created with their own deployment version in the Acent chain.
2. **Acent fosters blockchain mass adoption by lowering the financial entry barrier**
 Users can enjoy earning through farming or harvesting transaction fees collected on the Acent chain and distributed through the Acent Substance Accumulation Pool (ASAP).
3. A **cent fosters blockchain mass adoption by lowering the technical entry barrier**
 Users may receive network node hosting fees by handling complex procedures through the browser-MetaWallet integration.
4. **Acent resolves the Ethereum gas fee issue**
 Ethereum gas prices are too high but Nitro gas will remain cheap and within a reasonable value. (More details provided below)
5. **Acent alleviates scalability Issues**
 Acent mainnet maintains a practical higher number of transactions per second (TPS) at around 1,000 TPS compared to the Ethereum chain (version 1.0).

Here we outline the mechanisms at work in the ACENT blockchain.

## ACENT FUNCTIONALITIES

### Architecture

![ACENT ARCHITECTURE](images/architecture.png)

### Consensus

#### POSA (Proof of Staked Authority)

ACENT uses Proof of Staked Authority (POSA) Consensus which has evolved from the old decenternet POR (Proof-of-Reliability) algorithm. The ACE POSA is a hybrid form of consensus that enhances the Clique Proof of Authority Consensus with built-in DeFi-like staking rewards to all participants.

Clique POA consensus protocol has a unique feature wherein only designated signer nodes can seal/mine the blocks. This means there is no energy and time-consuming hash mining involve in contrast to Ethash (Ethereum&#39;s PoW algorithm). Only nodes that are in the list of signers can seal the blocks. In the absence of hash mining, Clique creates a block in a predefined period of time. In ACENT POSA, we set it to 3 seconds. This significantly speeds up transaction processing time by 5X as compared to Ethereum.

We modified the Clique POA consensus that instead of the signers getting the transaction fees, the said fees will go to a reward pool called Acent Substance Accumulation Pool (ASAP). A built-in staking smart contract called Acent Rewards Smart Contract (ARSC) will enable users of Acent blockchain to participate by staking ACENT into ARSC and get proportionate ACE rewards from ASAP.

The hybrid consensus enables the ACENT network to speed up transactions while keeping fees low and minimizes the network&#39;s carbon footprint. Furthermore, it also enables users to participate in decentralized fees farming.

#### Signers/Validators

Initially the signers/validators that would validate and seal/mine the blocks will be defined in the genesis.json. The signers will be updated dynamically via Clique POA protocol of Acent blockchain.

#### Staking Process

The POSA consensus works the same way as Clique POA consensus with additional staking feature via smart contracts. The staking feature will be administered by Acent Governance Smart Contract (AGSC) and Acent Rewards Smart Contract (ARSC) that will allow for the distribution of network fees as participation rewards called Acent Rewards Program (ARP)

When ACENT blockchain is released, all mined Nitro transaction fees are programmed to be sent to a specific ACENT blockchain address called the Acent Substance Accumulation Pool (ASAP). Since all the collected network fees are sent to the ASAP address, it will securely contain the accumulated ACE tokens for rewards use.

A specific-use smart contract, Acent Rewards Smart Contract (ARSC), is created to allow people to participate in a rewards distribution program.

ARSC will give participants entitlement to withdraw a percentage of the ASAP pool that is proportional to the amount of ACE tokens they deposited/staked.

The more ACE a participant deposits to ARSC, the more ACE from the ASAP they are entitled to withdraw. Similar to Uniswap, participants are also able to check their increasing withdrawable balance from the ASAP in real-time. Since balances are not locked in, participants may also withdraw their principal deposit at any time.

To better illustrate, consider the following example:

Alice buys Ethereum ACE from the exchange to participate in ARP. Alice will need to convert her Ethereum ACE to ACENT ACE via Acent Token Bridge (ATB) DApp. Alice will then get her ACENT ACE. Once Alice deposits the ACE tokens she converted, she will be able to see how much ACE she has deposited at all times as well as her share of ACE in the ASAP. Should she need to withdraw her ACE tokens, Alice will be able to choose between withdrawing her principal deposit or her earnings from the ARSC.

### Tokenomics

#### Token Distribution

ACE is the native token Acent Blockchain. Initially, 2 billion ACE (Eth ACE) are issued as an ERC20 token in the Ethereum blockchain. Once Acent blockchain is deployed, Eth ACE holders will have the option to transfer their Eth ACE tokens to Acent blockchain to participate in POSA staking and get more ACE as rewards, as explained in the Token Governance section.

#### Token Governance

Once the Acent blockchain is deployed, holders of Eth ACE will be able to convert their Ethereum ACE to Acent blockchain&#39;s ACE via the Ethereum Bridge Smart Contract (EBSC). EBSM will lock in the smart contract the Eth ACE to be converted. The Crypto Bridge Oracle (CBO) will pick-up the event in Ethereum and submit the conversion request to Acent Bridge Smart Contract (ABSC). ABSC will credit the holder&#39;s address in the Acent blockchain with the same amount of Ethereum ACE locked. The address used to call EBSM should be authorized address and defined via the Acent Governance DApp.

ABSC will initially hold the corresponding 2,000,000 ACE which will be needed to convert all the Eth ACE.

To manage future enhancements and settings of EBSC, CBO, and ABSC smart contracts, Acent Governance Smart Contract (AGSC) will facilitate approval of these changes via staked voting of ACE holders.

### Ascended Tokens

The Acent blockchain has it own version of wrapping called &quot;Ascending&quot; which allows users to convert BTC, ETH, or another wrapped contract as Acent-wrapped versions of their selected cryptocurrency. For instance, an ascended ETH will become AETH and WBTC to ABTC and will be sent to the user&#39;s Metawallet. The ETH or WBTC will then be held in custody within smart contracts to maintain a 1:1 value between the original and ascended tokens.

ETH and ERC20 tokens are will be equally transferable as ascended tokens on the Acent chain.

The Ethereum Bridge Smart Contract (EBSC), Crypto Bridge Oracle (CBO), and Acent Bridge Smart Contract (ABSC) via Acent Token Bridge (ATB) will facilitate the wrapping and ascending of corresponding tokens, similar to Eth ACE to ACE swap/conversion process.

The Acent Governance Smart Contract facilitates the nomination, approval, and listing of wrapped/ascended tokens in the Acent Blockchain.

## DAppS, SMART CONTRACTS AND INTERFACES

### Acent Rewards (AR) DApp

AR DApp will enable ACE holders to participate in Acent Rewards Program (ARP). AR DApp facilitates the staking, and withdrawal of the ACE of participants. AR DApp communicates with the Acent Rewards Smart Contract (ARSC) to process the participants&#39; requests.

Acent Rewards Smart Contract (ARSC) handles processing of Acent Rewards Program (ARP). It accepts and stores the staked ACE of participants. It computes the corresponding rewards of the participant based on the balance of ASAP and number of participants of the ARP. It is also responsible for transferring ACE staked and ACE rewards to participants.

### Acent Token Bridge (ATB) DApp

Acent Token Bridge (ATB) DApp will enable holder of ACE in Ethereum to convert their Eth ACE to ACE, the native token of Acent blockchain. ATB also facilitates conversion/bridging of ETH and ERC20 tokens from Ethereum to its Ascended token equivalent in Acent Blockchain. ATB handles both direction when converting/bridging tokens (i.e. from Ethereum blockchain to Acent blockchain and vice versa)

To process holder&#39;s conversion/bridge request from EThereum blockchain to Acent Blockchain, ATB communicates with Ethereum Bridge Smart Contract (EBSC). EBSC will accept any of the defined Eth ACE, ETH or ERC20 Tokens from the request, locks the specific token/coin and register the bridge event in Ethereum events. Crypto Bridge Oracle (CBO) will listen for conversion/bridge events in Ethereum events and will send the requests to Acent Bridge Smart Contract (ABSC). ABSC will facilitate conversion/bridge requests and will send corresponding Ascended tokens/coins to the holder&#39;s address in Acent blockchain.

To process holder&#39;s conversion/bridge request from Acent blockchain to Ethereum Blockchain, ATB communicates with Acent Bridge Smart Contract (ABSC). ABSC will accept any of the defined Eth ACE, ETH or ERC20 Tokens from the request, locks the specific token/coin and register the bridge event in Acent blockchain events. Crypto Bridge Oracle (CBO) will listen for conversion/bridge events in Acent blockchain events and will send the requests to Ethereum Bridge Smart Contract (EBSC). EBSC will facilitate conversion/bridge requests and will send corresponding Ethereum tokens/coins to the holder&#39;s address in Ethereum blockchain.

See [Appendix: DApps - Smart Contract Flows](#dapps---smart-contracts-flow)

### Acent Governance DApp

Acent Governance DApp will enable ACENT admins to facilitate voting on enhancements/forks of Acent blockchain, nomination, creation and support of tokens to be ascended (i.e. wrapped) in Acent blockchain, and upgrades/settings updates of the smart contracts in Acent blockchain ecosystem.

### Osiris Metawallet

Osiris Metawallet is the native crypto wallet of Osiris browser. Osiris Metawallet will facilitate the wallet interface for swap/conversion of Eth ACE and token swaps of wrapped tokens in Acent blockchain.

## APPENDIX

### DAppS - SMART CONTRACTS FLOW

#### ACENT REWARDS DAPP (Acent ACE Staking)

![ACENT STAKING](images/acent-staking.png)

#### ACENT REWARDS DAPP (Acent ACE/Rewards Withdrawal)

![ACENT WITHDRAWAL](images/acent-withdrawal.png)

#### ACENT TOKEN BRIDGE (Ethereum ACE to Acent ACE Bridge)

![ETHEREUM ACE TO ACENT ACE ](images/ea2aa.png)

#### ACENT TOKEN BRIDGE (Acent ACE To Ethereum ACE Bridge)

![ACENT ACE TO ETHEREUM ACE SWAP](images/aa2ea.png)

#### ACENT TOKEN BRIDGE (Ethereum ETH to Acent AETH Bridge)

![ETHEREUM ETH TO ACENT AETH](images/ee2ae.png)

#### ACENT TOKEN BRIDGE (Acent AETH To Ethereum ETH Bridge)

![ACENT AETH TO ETHEREUM ETH](images/ae2ee.png)

#### ACENT TOKEN BRIDGE (Ethereum WBTC to Acent ABTC Bridge)

![ETHEREUM WBTC TO ACENT ABTC](images/eb2ab.png)

#### ACENT TOKEN BRIDGE (Acent ABTC To Ethereum WBTC Bridge)

![ACENT ABTC TO ETHEREUM WBTC](images/ab2eb.png)


### Wrapped Smart Contract Samples


***WBTC within Open Zeppelin***

```
pragma solidity 0.4.24;
import "openzeppelin-solidity/contracts/token/ERC20/StandardToken.sol";
import "openzeppelin-solidity/contracts/token/ERC20/DetailedERC20.sol";
import "openzeppelin-solidity/contracts/token/ERC20/MintableToken.sol";
import "openzeppelin-solidity/contracts/token/ERC20/BurnableToken.sol";
import "openzeppelin-solidity/contracts/token/ERC20/PausableToken.sol";
import "../token/WrappedToken.sol";
contract WBTC is WrappedToken, DetailedERC20("Wrapped BTC", "WBTC", 8) {}
---- skip
```

***WETH within Open Zeppelin library***

```WETH within Open Zeppelin library
pragma solidity 0.4.24;
import "openzeppelin-solidity/contracts/token/ERC20/StandardToken.sol";
import "openzeppelin-solidity/contracts/token/ERC20/DetailedERC20.sol";
import "openzeppelin-solidity/contracts/token/ERC20/MintableToken.sol";
import "openzeppelin-solidity/contracts/token/ERC20/BurnableToken.sol";
import "openzeppelin-solidity/contracts/token/ERC20/PausableToken.sol";
import "../token/WrappedToken.sol";
contract WBTC is WrappedToken, DetailedERC20("Wrapped BTC", "WETH", 8) {}
---- skip
```



***AETH within Open Zeppelin library***

```AETH within Open Zeppelin library
pragma solidity =0.5.16;
import './interfaces/AETHerc20.sol';
import './libraries/AETHswap.sol';
contract PancakeERC20 is Acent ERC20 {
	using SwapToken for uint;

	string public constant name = 'Acent LPs';
	string public constant symbol = 'Acent-LP';
	uint8 public constant decimals = 18;
	uint  public totalSupply;
	mapping(address => uint) public balanceOf;
	mapping(address => mapping(address => uint)) public allowance;

	bytes32 public DOMAIN_SEPARATOR;
	// keccak256("Permit(address owner,address spender,uint256 value,uint256 nonce,uint256 deadline)");
	bytes32 public constant PERMIT_TYPEHASH = 0x6e71edae12b1b97f4d1f60370fef10105fa2faae0126114a169c64845d6126c9;
	mapping(address => uint) public nonces;

	event Approval(address indexed owner, address indexed spender, uint value);
	event Transfer(address indexed from, address indexed to, uint value);

	constructor() public {
    	uint chainId;
    	assembly {
        	chainId := chainid
    	}
    	DOMAIN_SEPARATOR = keccak256(
        	abi.encode(
            	keccak256('EIP712Domain(string name,string version,uint256 chainId,address verifyingContract)'),
            	keccak256(bytes(name)),
            	keccak256(bytes('1')),
            	chainId,
            	address(this)
        	)
    	);
	}
-------skip----------------------------
```



## ACENT Network Architecture
Acent is not just a product but an ecosystem that is built on a set of modular, adaptable, and interchangeable tools. It is a rewards based ecosystem that aims to surpass both the current internet ecosystems and the work of existing blockchains like Ethereum. 

Acent aims to expand into the mainstream by incentivizing net-neutral browsing and introducing DApps that use the play-to-earn model, among others. Developers are encouraged to join the effort to improve existing tools and create new ones in order to make the promise of blockchain technology a reality. 


### Acent mainnet
![ACENT MAINNET](images/1.%20MAINNET.png)

### Acent testnet
![ACENT TESTNET](images/2.%20TESTNET.png)

### Acent blockchain main infrastructure
![ACENT BLOCKCHAIN MAIN INFRASTRUCTURE](images/3.%20INFRA.png)

### Future Network Enhancements



### Network URLs

#### Main Net
Mainnet will be released according to the roadmap.
