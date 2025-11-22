# The Infrastructure Sharing Scheme: Deconstructing Blockchain as a Business Model

**Version**: 2.0  
**Date**: November 22, 2025  
**Authors**: Dhryl Anton, Michael Mcfall, Peter Jenson Haxel  
**Tools**: Manus AI, Claude AI, Typora  
**Team**: Onli Research Team  
**Organization**: The Onli Corporation

---

## Executive Summary

The prevailing critique of cryptocurrency often focuses on its technological inefficiencies—highlighting its slow transaction speeds and massive energy consumption compared to centralized systems like Visa or AWS. However, this comparison often misses the fundamental nature of the industry. A sober, logical analysis reveals that blockchain is not primarily a technological innovation in data processing, but a **business model innovation** designed to solve a specific economic problem: **Infrastructure Sharing**.

The core challenge blockchain attempts to address is: *How do you incentivize a distributed network of strangers to lend their computing power and storage infrastructure to maintain a common database without a central paymaster?* This paper argues that the cryptocurrency industry is essentially an **infrastructure sharing scheme**. Miners and validators are not merely processing transactions; they are infrastructure providers selling a specific product—**secure entries in a distributed database**. The "token" serves as the unit of account and the economic reward that motivates this provisioning of hardware. Consequently, the inefficiency of the network (e.g., Proof-of-Work energy costs) is not a technological flaw, but the necessary **security budget** required to maintain this leaderless business model.

This report deconstructs the ecosystem through this lens, examining the mechanics of "Consensus-as-a-Service," the reality of its accounting structures (double-entry vs. triple-entry), and the divergence between the utility of this infrastructure and the speculative mania that currently drives market valuations. We will demonstrate that while this model may have been a clever solution to the problem of expensive infrastructure in 2009, it is an anachronism in the age of cheap, ubiquitous cloud computing. For the vast majority of use cases, particularly internal corporate applications, paying a massive "architectural tax" to a distributed network of strangers is an economically irrational choice.

## 1. The Core Problem: Infrastructure Provisioning

To understand blockchain, one must first identify the problem it solves. It is not a problem of data speed or storage capacity; centralized relational databases (SQL) solved those issues decades ago with superior efficiency. The problem is **economic**: How to build a network where the infrastructure is owned by no one and everyone simultaneously.

### 1.1 The "Headless" Infrastructure Model

In a traditional model (e.g., Visa, Google Cloud), a central entity funds, owns, and secures the data centers. They charge fees to users to recoup these capital expenditures (CapEx) and operating expenses (OpEx). In the blockchain model, there is no central entity to buy the servers. The network must crowd-source its infrastructure from independent operators (miners/validators). This creates an "Infrastructure Sharing Scheme" where independent actors lend their compute and storage resources to the network.

### 1.2 The Economic Incentive: Selling Database Entries

To motivate these independent actors to incur real-world costs (hardware, electricity, cooling), the network must offer a product they can sell.

- **The Product**: The product is an **entry in the database** (block space).
- **The Sellers**: Miners/validators are the infrastructure providers.
- **The Buyers**: Users who wish to store a transaction record in that specific database.

Cryptocurrencies, therefore, are best understood not as "money" in the traditional sense, but as **"limited entries in a database that no one can change without fulfilling specific conditions."** The token is the coupon or unit of account that facilitates this exchange. It is the mechanism by which the infrastructure pays for itself.

## 2. Consensus-as-a-Service (CaaS)

If the business model is infrastructure sharing among untrusted parties, the critical service provided is not "payments" but **agreement**. In a centralized system, agreement is assumed because the master database is authoritative. In a distributed infrastructure scheme, agreement must be manufactured.

### 2.1 The Service of Agreement

Miners and validators are effectively selling **Consensus-as-a-Service (CaaS)**. They provide the computational work required to synchronize thousands of independent copies of the ledger.

- **Business Logic**: The latency and low throughput of blockchains are not "bugs"; they are the constraints of the CaaS business model. To ensure that a collection of strangers agrees on the state of the database, the network must deliberately slow down to allow for propagation and verification.
- **The Offering**: New enterprise models are explicitly marketing this as "Consensus-as-a-Service," allowing private networks to offload the difficulty of maintaining trust to a decentralized layer of infrastructure providers.

### 2.2 Security as a Cost Center

In this business model, security is the primary operational constraint. If the infrastructure is shared by anonymous actors, the risk of malicious updates (double-spending, history rewriting) is existential.

- **The Security Budget**: The massive energy consumption of Bitcoin (Proof-of-Work) is the **security budget** of the business model. It is the cost of physically securing the shared infrastructure against hostile takeover. While often compared to Visa’s energy use per transaction (where Bitcoin is millions of times less efficient), the proper comparison is to the cost of maintaining a physical vault or a military force to defend a gold reserve. The energy is the "moat" that protects the integrity of the purchased database entries.

## 3. The Accounting Reality: Double-Entry, Not Triple-Entry

A common narrative in the "innovation" argument is that blockchain introduces "Triple-Entry Accounting." A sober analysis of the accounting logic reveals this to be a misnomer.

### 3.1 Distributed Double-Entry

The system operates on a standard **double-entry bookkeeping** system. Every transaction consists of a debit from one address and a credit to another.

- **The "Third" Entry**: Proponents argue that the cryptographic signature or the blockchain record itself constitutes a "third entry" that verifies the transaction.
- **The Reality**: This is a control mechanism, not an accounting entry. It is simply **distributed double-entry accounting**. The innovation lies in the *replication* of the double-entry ledger across the shared infrastructure, ensuring that all providers hold the same copy of the debit/credit records. The fundamental logic of the accounting remains unchanged; only the verification mechanism (consensus) has shifted.

## 4. The Trust Paradox in Infrastructure Sharing

While the business model is designed to be "trustless" (relying on code and incentives), the practical implementation has led to massive re-intermediation and centralization.

### 4.1 Re-Intermediation

Because interacting directly with the raw infrastructure (running a node, managing keys) is technically complex, an entire industry of intermediaries—exchanges and custodians—has emerged.

- **The Irony**: Users trust these centralized intermediaries (Binance, Coinbase) to manage their access to the "trustless" infrastructure. This reintroduces the very counterparty risks the model was designed to eliminate.
- **Centralization of Code**: The development of the infrastructure software itself is highly centralized. For example, the Geth client is used by a supermajority of Ethereum validators, creating a single point of failure. Similarly, Bitcoin Core development is maintained by a small group of committers.

### 4.2 Infrastructure Centralization

The economics of mining (infrastructure provisioning) favor economies of scale, leading to the formation of large mining pools. This has resulted in a level of centralization that is antithetical to the stated goals of the ecosystem.

- **Cartelization of Mining**: A handful of mining pools consistently control over 51% of the hashrate for major networks like Bitcoin and Ethereum Classic. This gives them the theoretical ability to collude and perform a 51% attack, rewriting the ledger or censoring transactions. While overt attacks are rare due to the long-term economic disincentive (destroying the value of the network they mine), the *power* to do so still resides in the hands of a few. This is not a decentralized system; it is an oligopoly of infrastructure providers.

- **Staking Centralization**: In Proof-of-Stake systems, the same dynamic occurs. Large, centralized exchanges (like Coinbase, Binance) and staking services (like Lido) have become the dominant validators. A significant portion of users delegate their staking power to these entities for convenience, creating massive central points of control and failure. The top few staking pools control a sufficient percentage of the stake to halt the network or censor transactions if they were to collude or be compelled by a state actor.

## 5. Economic Reality: Utility vs. Speculation

There is a profound disconnect between the utility of the infrastructure sharing model (selling database entries) and the market valuation of the tokens.

### 5.1 The Token as a Speculative Asset

While the token has utility as a "coupon" to pay for infrastructure services (transaction fees), its market price is driven largely by speculation rather than the demand for block space.

- **Greater Fool Theory**: Academic research suggests that the pricing models for cryptocurrencies do not follow Discounted Cash Flow (DCF) logic, as there are no cash flows. Instead, they rely on the "Greater Fool Theory"—the expectation that someone else will pay more for the entry in the future.
- **Wash Trading**: The illusion of high demand is often manufactured. Studies indicate that up to 70% of volume on unregulated exchanges—and significant percentages on DEXs—is wash trading, designed to lure investors into the infrastructure scheme.

### 5.2 The Divergence

If the token were priced strictly on its utility (the cost to buy a database entry), volatility would likely be lower and prices would align with the cost of compute/energy. The current trillions in market capitalization reflect a **financialization of the infrastructure coupons**, treating them as "digital gold" rather than utility tokens.

## 6. The Architectural Tax: A Quantitative Analysis

The business model of infrastructure sharing imposes a significant and often overlooked "architectural tax" on its users. This tax is the premium paid for the service of decentralized consensus, a service that is increasingly unnecessary in an era of cheap, centralized infrastructure. A quantitative comparison reveals the staggering inefficiency of this model.

### 6.1 The Cost of a Single Transaction

Let us compare the cost of a single transaction across different systems as of late 2025:

| System | Energy Consumption (per transaction) | Financial Cost (per transaction) |
| :--- | :--- | :--- |
| **Bitcoin** | ~1,272 kWh | ~$5.00 - $50.00+ |
| **Ethereum** | ~0.03 kWh | ~$0.50 - $5.00+ |
| **Visa** | ~0.001 kWh | ~$0.15 - $0.25 (interchange fee) |
| **AWS (DynamoDB)** | Negligible | ~$0.00000025 (for a 1KB item write) |

*Sources: Digiconomist, YCharts, AWS Pricing Calculator*

As the data shows, a single Bitcoin transaction consumes enough energy to power an average U.S. household for over a month. Even with the move to Proof-of-Stake, an Ethereum transaction is orders of magnitude more expensive and energy-intensive than its centralized counterparts. The cost of writing a small record to a globally distributed, highly available database like Amazon DynamoDB is effectively zero for most practical purposes.

### 6.2 The Corporate Use Case: An Irrational Choice

The absurdity of the architectural tax becomes most apparent when considering the corporate use case. A corporation seeking to maintain a ledger of its internal activities (e.g., supply chain tracking, internal asset transfers) has two options:

1.  **Centralized Database (e.g., AWS RDS)**: Host a secure, private database on a cloud provider. **Cost: ~$15-50/month** for a small, highly available instance.
2.  **Private Blockchain**: Pay transaction fees to a public network of anonymous miners/validators to process and store these same transactions.

Why would a rational economic actor choose to pay external, anonymous parties a significant fee to process transactions that are internal to their own organization? The infrastructure sharing model was conceived in a world where setting up a secure, globally accessible server was a complex and expensive proposition. In the modern cloud era, it is a solved problem that costs less than a monthly coffee budget.

This is the crux of the argument: the infrastructure sharing scheme forces users to pay a massive premium for a service (decentralized consensus) that they often do not need, to solve a problem (expensive infrastructure) that no longer exists.

## 7. The Alternative: Escaping the Infrastructure Tax

The infrastructure sharing scheme is not an inevitability; it is a consequence of attempting to build a system of ownership on top of a distributed ledger. If one abandons the ledger, one abandons the need for shared infrastructure and its associated tax. This is the approach taken by the Onli architecture.

### 7.1 No Ledger, No Processing Bottleneck

Onli has no distributed ledger. There is no global state that must be synchronized across thousands of nodes. Every digital asset (a **Genome**) is a self-contained object, and every transaction is a peer-to-peer interaction between the sender and the receiver. This has profound implications for the infrastructure requirements:

- **No Consensus Required**: Since there is no shared database, there is no need for a complex and energy-intensive consensus mechanism to ensure agreement among strangers.
- **No Third-Party Infrastructure**: The processing for a transaction is handled by the devices of the two participants. You do not need to pay a network of miners or validators to execute your transaction.

### 7.2 The Power in Your Pocket

The computational requirements for an Onli transaction are minimal. A Genome, even one with elaborate use policies, is typically under 50KB. Any modern digital device—a smartphone, a tablet, a laptop—has more than enough processing power to handle the cryptographic calculations required for a transaction. In a world where billions of people carry a supercomputer in their pocket, the idea of outsourcing computation to a global network of specialized hardware is an anachronism.

### 7.3 Infinite Scalability at Millisecond Speed

Because each transaction is a peer-to-peer event, the Onli network can scale infinitely. A billion simultaneous transactions are simply a billion pairs of devices interacting directly. There is no central bottleneck, no network congestion, and no concept of a "block size" to limit throughput. Every transaction settles in milliseconds, regardless of how many other transactions are occurring on the network. This is a level of performance that is simply unattainable in any system based on a distributed ledger.

By eliminating the ledger, Onli eliminates the need for the infrastructure sharing scheme. It provides a model for digital ownership that is not only more secure and efficient, but also economically rational in the modern technological landscape of 2025.

## 8. The Counter-Argument: Is the Tax Worth It for Censorship Resistance and Immutability?

The most sophisticated defense of the infrastructure sharing scheme concedes its economic inefficiency but argues that the architectural tax is a necessary price for two essential properties: **censorship resistance** and **immutability**. The argument posits that only a massively distributed, economically incentivized network of anonymous actors can guarantee that transactions cannot be blocked and that the historical record cannot be altered. While compelling on the surface, this argument fails on two fronts: first, it overstates the practical reality of blockchain's guarantees, and second, it fails to recognize that these properties can be achieved more efficiently through a different architecture.

### 8.1 The Illusion of Censorship Resistance

The claim of censorship resistance is severely undermined by the economic realities of infrastructure centralization, as discussed in Section 4.2. When a handful of mining pools or staking entities control the majority of the network's processing power, they become central points of failure and control.

- **OFAC Compliance and Censorship**: In 2022, following the U.S. Treasury's sanctioning of Tornado Cash, a significant percentage of Ethereum validators began actively censoring transactions associated with sanctioned addresses. This was not a theoretical attack; it was a real-world demonstration that the supposedly censorship-resistant infrastructure is, in fact, beholden to the geopolitical and regulatory pressures placed upon its largest operators. The architectural tax did not buy immunity from state-level influence; it merely obfuscated the points of control.

In the Onli architecture, censorship resistance is achieved not through a global network of intermediaries, but by **eliminating the intermediary entirely**. A transaction is a private, peer-to-peer exchange of information between two parties. As long as those two parties can communicate—via the internet, Bluetooth, a messaging app, or even by saving a file to a USB drive—they can transact. There is no miner or validator to petition, and therefore no one to censor the transaction. Resistance is an intrinsic property of the peer-to-peer model, not a service purchased at great expense.

### 8.2 Immutability: Global vs. Object-Level

The concept of immutability is often conflated with the blockchain itself, but it is a property of any chained-hash data structure. The architectural tax is paid not for immutability itself, but for achieving **global consensus** on a single, immutable history.

- **The Cost of Global State**: Blockchain's approach is to make a single, universal history of all transactions immutable. This requires immense coordination and energy because every node must agree on the entire history of everything.

Onli achieves a more practical and efficient form of immutability at the object level. 

- **Object-Level Immutability**: The history of a Genome is immutable because each new state is a cryptographic function of its previous state plus the unique events it has experienced. To alter a past event in a Genome's history would require re-computing every subsequent state, which would invalidate its current state and render it useless. This creates a tamper-evident chain of custody for a *specific asset*, not for the entire universe of assets.

This is the crucial distinction: Onli provides **verifiable, object-level immutability** without the massive overhead of enforcing a single, global immutable state. Each asset carries its own immutable history within its mathematical structure. You do not need to pay a global network to verify the history of your specific asset; the asset verifies itself.

In conclusion, the architectural tax does not purchase the absolute guarantees it promises. The censorship resistance is conditional, and the global immutability is an inefficient and over-engineered solution for most use cases. Onli demonstrates that both properties can be achieved with greater integrity and near-zero marginal cost by shifting the architecture from a distributed ledger to a system of distributed, self-verifying objects.

## 9. Conclusion: An Anachronism in the Age of Cheap Infrastructure

Viewing blockchain through the lens of the Infrastructure Sharing Scheme clarifies the disconnect between the industry's narrative and its technological reality. The core innovation of cryptocurrency was not the distributed ledger—an old technology—but the creation of a business model to incentivize the provisioning of a "headless," shared infrastructure. This model, while clever, is a product of its time: a solution to the problem of expensive and inaccessible infrastructure that was relevant in 2009.

In 2025, in a world of ubiquitous, on-demand, and extraordinarily cheap cloud computing, this model is an anachronism. The "architectural tax" required to pay a global network of strangers to perform computations that can be handled by a smartphone is no longer justifiable. For corporations, the idea of paying external parties to manage internal records is economically irrational.

The market's speculative frenzy has obscured this fundamental reality, financializing the infrastructure coupons (tokens) into a new asset class. But the underlying utility remains that of a cumbersome and inefficient distributed database. As the cost of centralized infrastructure continues to plummet and the efficiency of peer-to-peer computation on personal devices grows, the economic foundation of the infrastructure sharing scheme will inevitably erode.

The future of digital assets will not be built on a model that manufactures scarcity and agreement at immense cost. It will be built on architectures that leverage the power of the devices already in our pockets, eliminating the need for a costly and inefficient intermediary layer. The question for the rational economic actor is simple: Why pay an architectural tax for a service you no longer need?

## References

[1] Anton, D., Mcfall, M., & Haxel, P. J. (2025). *The Physics of Finance*. The Onli Corporation.

[2] Anton, D., Mcfall, M., & Haxel, P. J. (2025). *The Ledger Fallacy: Why Blockchain is Not a System of Ownership*. The Onli Corporation.

[3] Merrill, T. W. (1998). Property and the Right to Exclude. *Nebraska Law Review*, 77(4), 730-755.

[4] Neward, T. (2004). The Vietnam of Computer Science. *TheServerSide.com*.

[5] Digiconomist. (2025). *Bitcoin Energy Consumption Index*. Retrieved from https://digiconomist.net/bitcoin-energy-consumption/

[6] YCharts. (2025). *Ethereum Average Transaction Fee*. Retrieved from https://ycharts.com/indicators/ethereum_average_transaction_fee

[7] Amazon Web Services. (2025). *AWS Pricing Calculator*. Retrieved from https://calculator.aws/

[8] European Commission. (2023). *Ethereum Merge Trend Report*. EU Blockchain Observatory and Forum.

[9] Costan, V., & Devadas, S. (2016). *Intel SGX Explained*. MIT Computer Science and Artificial Intelligence Laboratory.

[10] Lamport, L., Shostak, R., & Pease, M. (1982). The Byzantine Generals Problem. *ACM Transactions on Programming Languages and Systems*, 4(3), 382-401.

[11] Nakamoto, S. (2008). *Bitcoin: A Peer-to-Peer Electronic Cash System*.

[12] Buterin, V. (2013). *Ethereum White Paper*.

[13] Cowles Foundation. (2025). *Crypto Wash Trading*. Yale University.

[14] Rapid Innovation. (2025). *Blockchain Consensus-as-a-Service*.

[15] Alden, L. (2025). *Bitcoin Security Modeling*.

[16] Brookings Institution. (2025). *Debunking the Narratives About Cryptocurrency*atives about Cryptocurrency*.
