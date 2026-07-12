# Part Six: Inside Advanced Crypto Systems

This part continues directly from Page 60 of **Crypto, Pole Pole**.

Amina has become a teacher, but teaching exposes a new kind of question.

Her students no longer ask only, “What is a wallet?” or “Why does Bitcoin have value?”

They now ask:

**How can a blockchain prove large amounts of information, survive disagreements, scale to millions of users, and connect safely with the wider economy?**

Amina returns to the same method that helped her at the beginning.

One idea at a time. One Kenyan example at a time. Pole pole.

---

## Page 61: The Receipt Tree

On the first Saturday of the advanced class, Amina arrived with a paper bag full of receipts.

She poured them onto the table.

There were receipts for flour, cooking oil, charcoal, sugar, rent, phone airtime, and repairs to the tea stall.

“Imagine I have ten thousand receipts,” she said. “How can I prove that one particular receipt belongs in my records without showing you every receipt?”

Njeri picked up one.

“You could number them.”

“That helps me find them,” Amina said. “But how do you know I did not replace one after making the list?”

Kamau drew a tree on the board.

At the bottom, he placed eight simple transaction records. Each record went through a **hash function**.

A hash function turns information into a fixed-length digital fingerprint.

If the information changes, even slightly, the fingerprint changes.

Two fingerprints were then combined and hashed again. The new fingerprints were paired and hashed again. The process continued until only one fingerprint remained at the top.

That final fingerprint is called a **Merkle root**.

The full structure is called a **Merkle tree**.

The name sounds difficult, but the purpose is practical.

A Merkle tree allows someone to prove that one piece of information belongs in a large set without sending the entire set.

Suppose Amina wants to prove that receipt number 436 was included in her monthly records.

She does not need to show every receipt. She can provide the receipt and a small group of neighbouring hashes. The verifier follows the path upward and calculates the final root.

If the calculated root matches the trusted root, the receipt was included in the set.

This is called a **Merkle proof**.

Amina used a market example.

Imagine a lorry carries one thousand sacks of potatoes from Nyandarua to Nairobi. The driver has a signed list represented by one fingerprint.

At the destination, the buyer wants proof that sack number 672 was on the original list.

A Merkle proof can provide that evidence without sending the details of all one thousand sacks.

Blockchains use this idea because blocks can contain many transactions.

The block header can store a compact Merkle root representing all the transactions in that block.

A lightweight wallet may then verify that a transaction was included without downloading every transaction in the blockchain’s history.

Kevin asked, “Does the proof show that the transaction was honest?”

“No,” Amina said. “It shows that the transaction was included in the committed set.”

That distinction mattered.

A cryptographic proof can show that data matches a commitment.

It cannot automatically prove that the real-world story behind the data was truthful.

A fake land transfer can be included correctly in a Merkle tree.

The tree proves inclusion, not justice.

Amina wrote three lessons:

1. A hash acts like a digital fingerprint.
2. A Merkle root represents a large set of records.
3. A Merkle proof efficiently proves that one record belongs in that set.

> Advanced cryptography often makes verification smaller, faster, and easier. It does not remove the need to ask what the verified data means.

---

## Page 62: When One Road Becomes Two

A week later, road workers closed one route near Amina’s stall.

Matatus approaching the stage had to choose between two diversions.

For a while, both roads carried passengers toward the same destination.

Kamau pointed at the traffic.

“That is a useful picture for a blockchain fork.”

A **fork** happens when a blockchain’s history or rules split into different paths.

Not all forks are the same.

Sometimes two miners or validators produce valid blocks at nearly the same time. Different parts of the network may briefly see different blocks first.

The protocol has a rule for deciding which history becomes accepted.

On Bitcoin, nodes eventually follow the valid chain with the most accumulated proof of work. The other block becomes stale, and its transactions may return to the waiting area if they were not included elsewhere.

This type of temporary split is normal.

A different kind of fork happens when people change the software rules.

A **soft fork** makes the rules stricter while trying to remain compatible with older software.

Imagine a chama rule that previously allowed withdrawals up to KSh 100,000 with one signature. A new rule allows only KSh 20,000 with one signature.

Members following the stricter rule reject some actions that older members might accept. However, actions accepted under the new rule can still fit inside the old rule.

A **hard fork** changes the rules in a way that older software may not accept.

Imagine half the chama decides that contributions can now be made in goats, while the other half recognises only shillings.

The groups may no longer share one valid record.

If both communities continue supporting their versions, two networks and two assets can exist.

Amina asked who decides whether an upgrade happens.

“There is rarely one simple answer,” Kamau said.

Developers may write code.

Node operators decide what software they run.

Miners or validators decide what blocks they produce and support.

Exchanges decide which assets they list.

Wallets and businesses decide which networks they recognise.

Users decide where they place attention, money, and activity.

Governments may also influence outcomes through law and access.

This is why blockchain governance can be messy.

Code matters, but so do people, institutions, communication, and economic power.

Amina told the students about a disagreement in their chama.

Some members wanted to invest the group’s savings in a delivery motorbike. Others wanted to preserve cash for emergencies.

The written rules explained how to vote, but they could not make everyone agree.

A blockchain protocol can define how valid blocks are selected. It cannot remove political disagreement about what the rules should become.

Before using a network after a major fork, Amina advised checking:

- which chain major wallets support,
- which chain exchanges recognise,
- whether replay protection exists,
- whether the asset symbol has changed,
- where developers and validators have moved,
- and whether scammers are using the confusion.

A fork can create duplicate-looking balances on two chains. That does not mean free wealth has appeared without risk.

Prices can collapse. Wallets can send transactions on the wrong chain. Fake support accounts can target confused users.

> A blockchain fork is not only a technical split. It is a public argument about rules, ownership, and which history a community will recognise.

---

## Page 63: When Is a Payment Truly Final?

A customer paid Amina with cash.

She checked the note and placed it in her tin.

The payment felt final.

Another customer paid through mobile money.

Amina saw the confirmation message, but she knew that mistakes, fraud investigations, court orders, or system corrections could sometimes affect financial records.

A third customer paid with Bitcoin.

The transaction appeared quickly, but it had zero confirmations.

“Which payment is final?” Njeri asked.

Amina smiled.

“That depends on what we mean by final.”

**Finality** means confidence that a transaction will not be reversed or replaced.

Different systems provide different forms of finality.

Bitcoin uses what is often called **probabilistic finality**.

When a transaction enters a block, it has one confirmation. Each additional block built on top of it makes reversal less likely.

There is no magical moment when mathematics changes from “possibly reversible” to “absolutely impossible.”

Instead, confidence grows.

For a cup of tea, a merchant may accept a small risk after seeing a valid transaction.

For the sale of a house, the parties may wait for more confirmations because the value is much larger.

Some proof-of-stake networks use **economic finality**.

Validators vote on blocks. After enough stake supports a checkpoint under the protocol’s rules, reversing it may require validators to violate the rules and lose valuable stake.

The transaction is treated as final because a conflicting history would be extremely costly and may trigger penalties.

Other networks use rapid finality through smaller validator groups or specialised consensus systems.

That can improve speed, but users must examine who the validators are and what happens if many fail or cooperate dishonestly.

Amina compared finality to selling a cow.

A buyer may first send a deposit.

Later, both sides sign documents.

The cow is transported.

Ownership records are updated.

Each step increases confidence, but the legal system still defines how disputes are handled.

Blockchain finality is also shaped by rules and assumptions.

A transaction may be final on the chain while still being disputed in the real world.

Suppose someone steals Amina’s private key and sends her funds away.

The blockchain can finalise the transfer correctly according to its rules.

That does not make the theft morally or legally acceptable.

It means the network recognised a valid signature.

Users should ask:

1. How does this network define finality?
2. How long does finality normally take?
3. Can the chain reorganise?
4. What economic cost would reversal require?
5. Who can halt or restart the network?
6. Has the network changed history before?
7. How much finality is appropriate for this transaction?

Amina wrote a rule for merchants:

> The larger the payment and the harder the refund, the more carefully you should understand settlement and finality.

Fast appearance is not always final settlement.

A transaction can appear in a wallet before the network has reached strong agreement.

---

## Page 64: When Consensus Breaks

During one chama meeting, ten members had to approve the month’s accounts.

Four members lost network access during a storm.

Three members disagreed with the treasurer.

The remaining three could not reach the required number of approvals.

No money was stolen.

Nothing moved at all.

“This is a **liveness failure**,” Kamau explained.

A consensus system has two important goals.

**Safety** means honest participants do not accept conflicting histories as final.

**Liveness** means the system continues making progress and processing valid activity.

A network can protect safety by stopping when it is uncertain.

That is like the chama refusing to approve a withdrawal when too few officials are available.

The money remains safe, but urgent payments may be delayed.

A network can protect liveness by continuing with fewer participants.

That may keep transactions moving, but it can increase the danger of conflicting decisions.

Consensus design balances these risks.

Failures can happen for many reasons:

- internet outages,
- software bugs,
- power failures,
- incompatible upgrades,
- validators going offline,
- attacks on network communication,
- dishonest majorities,
- or cloud service failures affecting many validators at once.

A **chain reorganisation** happens when the network replaces recent blocks with another valid history.

Small reorganisations may be part of normal operation on some chains.

Large or repeated reorganisations can reduce confidence and expose merchants to double spending.

A **double-signing** failure happens when a validator signs conflicting blocks or votes.

Proof-of-stake systems may punish this through slashing.

A **51 percent attack** generally describes a situation where one party or cooperating group controls enough mining power or stake to influence block production and transaction ordering.

Such an attacker may be able to censor transactions or attempt to reverse recent payments.

They cannot normally create coins from nothing or spend coins without valid keys.

That is an important limit.

Amina compared it to controlling most matatus on a route.

The owners could refuse to carry certain passengers or delay competitors.

They could not use that control to open every passenger’s locked house.

Power over transaction ordering is serious, but it is not unlimited power over all cryptography.

Networks may respond to failures through:

- automatic penalties,
- backup communication paths,
- client diversity,
- emergency upgrades,
- social agreement,
- or temporary halts.

Each response adds trade-offs.

An emergency committee can act quickly, but it becomes a point of trust.

Automatic rules reduce discretion, but software may react badly to an unexpected event.

Social recovery can save a network, but it shows that humans remain part of the final decision.

Amina told the students to study outages rather than only marketing claims.

A project’s behaviour during stress reveals:

- who has emergency power,
- whether users receive honest information,
- how decentralised infrastructure really is,
- whether funds remain safe,
- and how quickly developers learn from failure.

> A network is not proven by operating smoothly on an ordinary day. Its design becomes visible when machines fail, participants disagree, and money is at risk.

---

## Page 65: A Rollup Is Like a Busy Matatu

Amina’s class tried a popular blockchain application during a busy evening.

The base network fee was higher than the amount Njeri wanted to send.

“This cannot serve ordinary people,” Njeri complained.

Kamau drew a matatu.

“If twenty passengers travel from Thika to Nairobi, they do not each need a separate vehicle,” he said. “They can share one journey.”

A **rollup** applies a similar idea to blockchain transactions.

It processes or groups many transactions outside the main chain, then publishes compressed information or proofs back to the main chain.

The main chain becomes the settlement and security layer.

The rollup handles much of the activity.

This can increase capacity and reduce fees.

There are two broad families.

### Optimistic rollups

An optimistic rollup assumes submitted transaction results are valid unless someone challenges them.

The word “optimistic” means the system accepts the result first and allows a period for fraud proofs.

If a dishonest result is submitted, a watcher can challenge it.

A correct challenge causes the invalid claim to be rejected and may punish the dishonest party.

This design needs:

- enough time for challenges,
- honest watchers,
- available transaction data,
- and working fraud-proof software.

Withdrawing to the main chain can take time because users may need to wait for the challenge period.

### Zero-knowledge rollups

A zero-knowledge rollup, often called a ZK rollup, submits a cryptographic validity proof.

The proof shows that the new state follows the rules without the main chain redoing every calculation.

The main chain verifies the proof.

This can provide faster finality, but generating proofs can require complex technology and heavy computation.

Both designs can still have centralised parts.

A **sequencer** usually orders transactions inside the rollup.

If one company controls the sequencer, it may delay or censor users, even if it cannot steal funds directly.

Users should ask whether they can force a transaction through the main chain when the sequencer fails.

A rollup can also have upgrade keys.

An administrator may be able to change the contract.

That can help fix bugs, but it creates trust.

Amina returned to the matatu example.

The base chain is the highway authority that recognises the completed journey.

The rollup is the matatu operator grouping passengers.

The sequencer is the conductor deciding boarding order.

The proof or transaction data is the trip record.

The bridge contract is the stage where passengers enter and leave.

If the conductor disappears, passengers need an emergency way to exit.

If the stage records are wrong, funds may be trapped.

Amina’s rollup checklist included:

1. Who controls the sequencer?
2. Can users withdraw without the operator’s permission?
3. Where is transaction data published?
4. Who controls upgrades?
5. Is there a delay before upgrades take effect?
6. Has the proof system been audited?
7. What happens if the rollup stops?
8. Is the bridge protected?

> Layer 2 does not mean risk disappears. It means part of the work and part of the trust move to a new system.

---

## Page 66: The Missing Exercise Book

A teacher can mark a student’s answer only if the work is available.

One afternoon, Kevin claimed that he had completed twenty mathematics questions correctly.

“Show me the exercise book,” Amina said.

“I left it at school.”

“Then I cannot verify your claim.”

This simple problem explains **data availability**.

A blockchain network may receive a claim that the system moved from one valid state to another.

But verifiers need access to enough underlying data to check transactions, reconstruct balances, or challenge fraud.

If the data is hidden, users may know that someone announced a new result but cannot independently verify how the result was produced.

For a rollup, transaction data must be available so that others can reconstruct the rollup state.

This matters especially when the main operator disappears or behaves dishonestly.

A system can publish full transaction data on the main chain.

That provides strong security, but it can be expensive.

Other systems publish data to specialised data availability networks.

This can reduce cost, but it introduces another network and another set of assumptions.

Amina compared it to land records.

Suppose a county office publishes only one sentence:

“Ownership records were updated correctly.”

Citizens cannot verify the change unless the supporting documents are available.

A hash of the documents proves commitment to specific information, but the hash does not reveal the documents.

Data commitment and data availability are different.

A **data availability sampling** system lets many light participants check small random pieces of a larger data set.

If enough random samples are available, participants gain confidence that the full data was published.

Imagine one thousand sacks of maize arranged in a warehouse.

Inspectors randomly check many positions.

If an owner hides a large part of the stock, random sampling has a good chance of discovering the missing sections.

The comparison is not perfect, but it shows how small checks can provide confidence about a large set.

Amina taught the class four separate questions:

1. Was the data committed?
2. Is the data available?
3. Is the data valid?
4. Does the data describe a truthful real-world event?

These questions are related, but not identical.

A blockchain may prove that a specific set of bytes was published.

A validity proof may prove that calculations followed rules.

Neither automatically proves that a farmer delivered real maize or that a person owns the land described.

Oracles and legal institutions still matter when blockchains touch the physical world.

> A proof cannot help a verifier when the information needed to check the proof has been hidden.

---

## Page 67: Proving Without Revealing

Njeri wanted to enter an event limited to people over eighteen.

The organiser asked for a copy of her identity card.

She felt uncomfortable.

The card showed more than her age. It showed her full name, date of birth, photograph, and identification number.

“Why must I reveal everything to prove one fact?” she asked.

This question introduces **zero-knowledge proofs**.

A zero-knowledge proof allows one party to prove that a statement is true without revealing the secret information behind it.

In a simplified example, Njeri could prove that her age is above eighteen without revealing her exact birth date.

A borrower might prove that income exceeds a required level without publishing the full salary statement.

A user might prove membership in an approved group without revealing which member they are.

A blockchain transaction system might prove that balances and calculations follow the rules while hiding specific amounts or participants.

The proof has three important goals:

- a true statement should be provable,
- a false statement should be extremely difficult to prove,
- and the verifier should learn nothing beyond the intended fact.

Real zero-knowledge systems use advanced mathematics.

A beginner does not need to calculate the equations to understand the purpose.

The purpose is selective proof.

Amina used a box with a locked door.

She placed a red bead or a blue bead inside.

Njeri wanted to prove that she knew the bead’s colour without showing the bead.

Through repeated challenges, she could convince the class that she knew the secret while keeping the colour hidden.

This classroom game was only an analogy. Real proofs are cryptographic and non-interactive in many blockchain systems.

Zero-knowledge technology can support:

- private payments,
- identity proofs,
- rollup scaling,
- proof of asset ownership,
- voting systems,
- compliance checks,
- and verification of complex calculations.

It also creates risks.

The proving software may contain bugs.

A trusted setup, where used, may be compromised.

Complex circuits may enforce the wrong rule.

Private systems can be abused for crime as well as used for legitimate privacy.

Governments and businesses may disagree about how much privacy is acceptable.

Amina reminded the class that privacy is not the same as secrecy for wrongdoing.

People need privacy when discussing health, protecting salaries, voting, trading, or escaping abuse.

At the same time, financial institutions have legal duties to manage fraud and money laundering.

The difficult task is designing systems that protect ordinary people while supporting legitimate accountability.

> Good privacy allows a person to reveal what is necessary for a purpose, not every detail they possess.

---

## Page 68: The Invisible Tax of Transaction Order

Two customers reached Amina’s stall at the same moment.

Both wanted the last samosa.

One had arrived first, but the second customer offered Amina more money.

Who should receive it?

The order of actions can create value.

On a blockchain, block producers or sequencers decide the order in which transactions appear.

That ordering power creates **maximum extractable value**, commonly called MEV.

MEV is value that can be gained by including, excluding, or rearranging transactions.

Suppose a large buyer submits an order on a decentralised exchange.

The order will push the token price upward.

A bot sees the pending transaction.

It buys first, lets the large order raise the price, then sells immediately after.

This is called **front-running** when a transaction is placed before another to profit from its expected effect.

A **sandwich attack** places one trade before the user and another after the user.

The user receives a worse price.

The bot keeps the difference, minus fees.

MEV can also come from useful activity.

A liquidator may close an unhealthy loan and protect a lending protocol from bad debt.

An arbitrage trader may correct price differences between exchanges.

The problem is not that every form of MEV is dishonest.

The problem is that transaction ordering creates hidden competition and can harm users.

On a busy Nairobi route, matatu operators may compete for the first position because the first vehicle gets passengers.

On a blockchain, bots compete to place profitable transactions in the best position.

They may pay higher priority fees or make private agreements with block builders.

This competition can raise costs and centralise infrastructure.

Amina showed the students how users can reduce exposure:

- set reasonable slippage limits,
- avoid trading illiquid tokens,
- split very large trades carefully,
- use protected transaction services where trustworthy,
- compare expected output before approving,
- and avoid broadcasting obvious profitable opportunities.

Decentralised exchange interfaces may offer MEV protection, but users should understand what the protection trusts.

A private relay may hide the transaction from the public waiting area.

That can reduce front-running, but the relay itself may see the order.

A batch auction may execute many trades together at one price.

That can reduce ordering games, but it changes how quickly trades settle.

> Whenever transaction order affects profit, someone will compete to control the order.

MEV is an advanced example of a simple lesson Amina learned long ago.

Rules create incentives.

Incentives shape behaviour.

---

## Page 69: When DeFi Risks Join Hands

Amina studied a DeFi strategy advertising a high return.

The strategy looked simple:

1. Deposit a stablecoin.
2. The protocol lends it.
3. The receipt token is deposited elsewhere.
4. Another protocol borrows against it.
5. Rewards are sold and reinvested.

Each step seemed reasonable.

Together, they created a chain of dependence.

This is called **composability**.

DeFi applications can connect like building blocks.

Composability allows rapid innovation.

It also allows risk to travel from one protocol to another.

Suppose the stablecoin loses its peg.

The lending protocol may experience withdrawals.

The receipt token may fall in value.

Borrowers may be liquidated.

The automated strategy may fail to exit.

A bridge used by one part of the system may pause.

An oracle may report a delayed price.

A governance vote may change collateral rules during the crisis.

One failure can trigger several others.

This is **systemic risk**.

Amina compared it to several businesses in one shopping centre.

The restaurant depends on the water company.

The water company depends on electricity.

The electricity system depends on fuel.

The fuel supplier depends on a bank.

The bank depends on a communication network.

A problem in one place can reach businesses that appeared unrelated.

Advanced DeFi risks include:

### Smart contract risk

Code may contain a bug or unsafe upgrade.

### Oracle risk

The protocol may use an incorrect or manipulated price.

### Liquidity risk

Users may be unable to sell or withdraw without a large loss.

### Stablecoin risk

The stablecoin may lose its peg or reserves may fail.

### Leverage risk

Borrowing can multiply both gains and losses.

### Governance risk

A small group may pass harmful changes.

### Bridge risk

Assets may depend on a vulnerable cross-chain system.

### Liquidation risk

A temporary price movement may force a sale at the worst time.

### Counterparty risk

A supposedly decentralised product may depend on a company, market maker, or custodian.

### Regulatory risk

Access, token treatment, or business operations may change under law.

Amina created a dependency map before depositing money.

At the centre, she wrote the product name.

Around it, she added every token, oracle, bridge, administrator, exchange, and contract the strategy used.

The attractive return now looked different.

It was payment for accepting several connected risks.

A high annual percentage yield is not free money.

It may be compensation for risk, token inflation, temporary rewards, leverage, or an unsustainable subsidy.

> In DeFi, study not only the product you touch. Study the systems that product depends on.

---

## Page 70: An Identity You Carry

At a clinic, Amina filled in the same personal details she had written at another clinic.

At a training centre, she carried paper certificates to prove her qualifications.

At a new financial service, she submitted identification again.

“Why can I not carry trusted proofs about myself?” she asked.

This question leads to **decentralised identity**.

Traditional identity systems often store user information inside separate organisations.

Each organisation creates an account and controls its own database.

A decentralised identity approach tries to let a person hold reusable digital credentials.

A school could issue a **verifiable credential** showing that Njeri completed a course.

The credential would contain a cryptographic signature.

A future employer could verify that signature without calling the school for every application.

A government could issue a proof of age.

A professional body could issue a licence.

A cooperative could issue membership proof.

The user stores credentials in a wallet and presents only what is needed.

A **decentralised identifier**, often shortened to DID, is an identifier that can be connected to cryptographic keys and documents without depending entirely on one website username.

The system still needs trusted issuers.

A fake school can issue a perfectly signed fake qualification.

Cryptography proves who signed the credential.

Society must decide whether the signer is credible.

Amina described three roles:

1. **Issuer:** the organisation creating the credential.
2. **Holder:** the person receiving and storing it.
3. **Verifier:** the person or service checking it.

Good identity design must consider recovery.

If Njeri loses her phone, does she lose every credential?

Can an abusive partner control her recovery contact?

Can an issuer revoke a credential?

Can a verifier secretly track every place the credential is used?

Can a blockchain expose permanent personal information?

Putting raw identity data on a public blockchain can be dangerous because public records may remain visible for years.

Many identity systems store only identifiers, revocation records, or proofs on-chain while keeping sensitive details off-chain.

Amina warned against using “decentralised” as a marketing word.

If one company controls the wallet, issuer list, recovery process, and verification server, the user may still depend heavily on that company.

> Digital identity should give people useful control over proof, but it must also protect privacy, recovery, consent, and the right not to be tracked.

---

## Page 71: How Institutions Hold Crypto

Amina kept a small learning balance in a self-custody wallet.

A pension fund or large company could not manage billions of shillings in the same way.

It needed policies, audits, several approvals, insurance arrangements, legal responsibility, and controls that survive staff changes.

This is **institutional custody**.

A custodian holds crypto assets or controls the keys on behalf of another organisation.

Institutions may choose custody because they need:

- separation of duties,
- transaction approval policies,
- reporting,
- compliance checks,
- secure key storage,
- insurance,
- recovery procedures,
- and legal accountability.

Amina visited a fictional company treasury office.

No employee knew the complete private key.

The system used several key shares.

A transfer required approval from people in different departments.

Large withdrawals had a waiting period.

Destination addresses were approved in advance.

Keys were stored in protected devices.

Every action produced an audit record.

This is very different from writing a seed phrase in one manager’s notebook.

Common custody approaches include:

### Cold storage

Keys remain offline for stronger protection from internet attacks.

Cold storage is safer for long-term holdings but slower for daily transactions.

### Multi-signature custody

Several keys must approve a transaction.

This reduces dependence on one person or device.

### Multi-party computation

Different parties hold secret shares and jointly create a signature without reconstructing one complete private key in one place.

### Qualified or regulated custody

A licensed entity holds assets under specific legal and operational requirements.

Regulation can improve accountability, but it does not remove operational or financial risk.

Institutions also need to understand **rehypothecation**.

A custodian or trading platform may lend or reuse customer assets.

The customer may believe coins are sitting untouched in a wallet while the company has created additional obligations.

This introduces counterparty and liquidity risk.

Proof-of-reserves can help show that a company controls certain assets.

It does not by itself prove that all liabilities are disclosed, that assets are unencumbered, or that the company is solvent.

A complete assessment needs both assets and obligations.

Amina’s institutional checklist included:

1. Who legally owns the assets?
2. Who controls each key share?
3. How are employees removed from access?
4. What happens after a death or disaster?
5. Are customer assets segregated?
6. Can the custodian lend the assets?
7. What insurance exists, and what does it exclude?
8. How are transactions audited?
9. Which country’s laws apply?
10. What happens if the custodian fails?

> Institutional security is not one strong password. It is a system of technology, people, law, process, and accountability.

---

## Page 72: Crypto Meets the Wider Economy

For the final class of Part Six, Amina drew five circles on the board.

She labelled them:

- households,
- businesses,
- banks,
- governments,
- crypto networks.

Then she connected the circles.

Crypto does not exist in a separate universe.

A Kenyan user may earn shillings, buy a stablecoin through an exchange, transfer it across a blockchain, use a DeFi application, sell it through an off-ramp, and pay rent in shillings.

Every step touches the wider economy.

Banks may provide accounts to exchanges.

Payment companies may connect merchants to stablecoin settlement.

Governments may tax gains and regulate service providers.

Telecommunication companies provide the internet and mobile access.

Courts decide disputes.

Developers maintain software.

Auditors examine reserves and contracts.

Ordinary users provide the final demand.

Amina explained several possible connections.

### Payments and remittances

Stablecoins may reduce settlement time across borders.

Their real value depends on reliable reserves, affordable on-ramps, safe wallets, legal access, and useful off-ramps.

### Savings and investment

Bitcoin and other crypto assets may form part of some portfolios.

They remain volatile and can lose significant value.

A responsible saver separates essential money from high-risk assets.

### Capital markets

Tokens may represent funds, bonds, shares, invoices, or real estate interests.

Tokenisation can improve transfer and settlement, but legal ownership must match the digital record.

A token saying “one share” is not enough if company law does not recognise the holder’s rights.

### Banking

Banks may offer custody, settlement, tokenised deposits, or blockchain infrastructure.

Public blockchains may compete with some banking services while supporting others.

### Government

Public institutions may explore digital identity, payments, records, or central bank digital currency.

Technology can improve administration, but public accountability, privacy, and due process remain essential.

### Business operations

Companies may use smart contracts for settlement, supply chains, loyalty programmes, or shared records.

A normal database may still be cheaper and simpler when one trusted organisation controls the process.

The students asked whether crypto would replace banks and governments.

Amina answered carefully.

“Some services may change. Some middlemen may disappear. New middlemen may appear. Banks and governments may adopt parts of the technology. Public networks may grow beside them. The future will probably be mixed.”

The strongest question was not, “Will crypto win?”

It was:

**Which system serves people better for this particular purpose, under these particular risks and rules?**

Amina returned to her first lesson.

Money is a shared agreement.

Crypto changes how some agreements can be recorded, verified, and enforced.

It does not remove human needs.

People still need food, shelter, trust, fair laws, secure technology, education, and ways to correct harm.

Kevin looked at the five circles.

“So this is the end?”

“Not yet,” Amina said.

They had entered advanced territory, but several important subjects remained.

The next stage would examine privacy systems, governance attacks, tokenised real-world assets, economic design, security failures, regulation, and how to evaluate the future without falling for hype.

Amina closed her notebook.

On the last page she wrote:

> Crypto becomes useful when technical possibility meets human reality.

---

# Learning Checkpoint Six

### 1. What does a Merkle proof show?

It efficiently shows that a piece of data was included in a larger committed set.

### 2. What is a blockchain fork?

It is a split in blockchain history or rules that can be temporary or can create separate networks.

### 3. What is finality?

Finality is confidence that a transaction will not be reversed or replaced.

### 4. What are safety and liveness?

Safety protects the network from accepting conflicting histories. Liveness allows the network to continue processing valid activity.

### 5. What is a rollup?

A rollup groups or processes transactions outside a base chain and posts data or proofs back to it for settlement.

### 6. Why does data availability matter?

Verifiers need access to transaction data so they can reconstruct the state, check claims, or challenge fraud.

### 7. What is a zero-knowledge proof?

It proves that a statement is true without revealing the secret information behind the statement.

### 8. What is MEV?

MEV is value gained by including, excluding, or changing the order of blockchain transactions.

### 9. Why can DeFi risk spread?

Protocols depend on shared stablecoins, oracles, bridges, liquidity, governance, and smart contracts. A failure in one system can affect many others.

### 10. What is a verifiable credential?

It is a digitally signed claim issued by a trusted organisation that a holder can present to a verifier.

### 11. What does institutional custody require?

It requires secure key management, multiple approvals, audits, legal responsibility, recovery plans, and clear control of assets.

### 12. Does crypto operate separately from the economy?

No. It connects with banks, payment systems, businesses, governments, telecommunications, courts, and ordinary users.

---

# What Comes Next

## Part Seven: Power, Privacy, and Real-World Assets

The next installment will continue with Pages 73–84 and cover:

1. Privacy coins and transaction privacy
2. Governance attacks and vote buying
3. Real-world asset tokenisation
4. Stablecoin reserve design
5. Token incentives and reflexive markets
6. Protocol treasuries
7. Smart contract security and audits
8. Economic attacks
9. Regulation and enforcement
10. Crypto taxation and record keeping
11. Building responsible crypto products
12. A framework for judging crypto’s future
