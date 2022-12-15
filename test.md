  Виды on-chain управления блокчейн-сетями.
  
  Mechanism
  
  To make any changes to the network, the idea is to compose active token holders and the council together to administrate a network upgrade decision.No matter whether the proposal is proposed by the public (token holders) or the council, it finally will have to go through a referendum to let all holders, weighted by stake, make the decision.
  
  Referenda are simple, inclusive, stake-based voting schemes. Each referendum has a specific proposal associated with it that takes the form of a privileged function call in the runtime (that includes the most powerful call: set_code, which can switch out the entire code of the runtime, achieving what would otherwise require a "hard fork").
Referenda are discrete events, have a fixed period where voting happens, and then are tallied and the function call is made if the vote is approved. Referenda are always binary; your only options in voting are "aye", "nay", or abstaining entirely.
Referenda can be started in one of several ways:
        Publicly submitted proposals;
        Proposals submitted by the council, either through a majority or unanimously;
        Proposals submitted as part of the enactment of a prior referendum;
        Emergency proposals submitted by the Technical Committee and approved by the Council.
All referenda have an enactment delay associated with them. This is the period between the referendum ending and, assuming the proposal was approved, the changes being enacted.


Proposing a Referendum

Public Referenda

Anyone can propose a referendum by depositing the minimum amount of tokens for a certain period (number of blocks). If someone agrees with the proposal, they may deposit the same amount of tokens to support it - this action is called endorsing. The proposal with the highest amount of bonded support will be selected to be a referendum in the next voting cycle.
Note that this may be different from the absolute number of endorsements; for instance, three accounts bonding 20 DOT each would "outweigh" ten accounts bonding a single DOT each
The bonded tokens will be released once the proposal is tabled (that is, brought to a vote).
There can be a maximum of 100 public proposals in the proposal queue.

Council Referenda

Unanimous Council - When all members of the council agree on a proposal, it can be moved to a referendum. This referendum will have a negative turnout bias (that is, the smaller the amount of stake voting, the smaller the amount necessary for it to pass - see Adaptive Quorum Biasing).
Majority Council - When agreement from only a simple majority of council members occurs, the referendum can also be voted upon, but it will be majority-carries (51% wins).
There can only be one active referendum at any given time, except when there is also an emergency referendum in progress.

Voting Timetable
Every 28 days, a new referendum will come up for a vote, assuming there is at least one proposal in one of the queues. There is a queue for Council-approved proposals and a queue for publicly submitted proposals. The referendum to be voted upon alternates between the top proposal in the two queues.
The "top" proposal is determined by the amount of stake bonded behind it. If the given queue whose turn it is to create a referendum that has no proposals (is empty), and proposals are waiting in the other queue, the top proposal in the other queue will become a referendum.
Multiple referenda cannot be voted upon in the same period, excluding emergency referenda. An emergency referendum occurring at the same time as a regular referendum (either public- or council-proposed) is the only time that multiple referenda will be able to be voted on at once.
Voting on a referendum
To vote, a voter generally must lock their tokens up for at least the enactment delay period beyond the end of the referendum. This is in order to ensure that some minimal economic buy-in to the result is needed and to dissuade vote selling.






Параметры ERC721, ERC1155, примеры программного кода.


ERC-721 is the standard interface for non-Fungible tokens (NFT).ERC-721 was first used by CryptoKitties games at the end of 2017. The popularity of CryptoKitties made people realize the important value of ERC-721.ERC-721 is a non-homogeneous token, which means that each token is different and has its own uniqueness and unique value. Of course, this means that they are inseparable and traceable at the same time.ERC-721 represents ownership of assets, provides the possibility for the tokenization of items or records, and opens up a huge market, such as real-world houses (houses are immovable, occupy a specific space of assets, unique) and unique works of art; collectible items in the virtual world, such as various unique collectibles in various collectible games on Ethereum; loan transaction records in financial transactions.


The most unique feature of ER1155 is that it uses a single smart contract to represent multiple tokens at once.This is why its balanceOf function is different fromER20 andER777.It has an additional id parameter as the token identifier to query the balance.
This is similar toER721, but the id in the table does not have the concept of balance.The balanceOf function of ER721 is associated with how many different tokens an account owns, not how many each owns.On the other hand, theER1155 account has a very clear balance for each token id.And irreplaceable through confirmation is achieved by simply casting one of them
This method will save a lot of gas fees for projects with multiple tokens.It is better than deploying different contracts for each token type.AnER1155 token contract can contain all system states, reducing deployment costs and complexity.
