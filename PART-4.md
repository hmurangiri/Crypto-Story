# Part Four: How Crypto Systems Make Decisions

This part continues directly from Page 36 of **Crypto, Pole Pole**.

Amina now understands Bitcoin, wallets, exchanges, stablecoins, Ethereum, smart contracts, DeFi, NFTs, and common scams.

She has learned how to send value and how applications can run on a blockchain.

But one question remains:

**Who keeps these newer networks honest, and who decides when their rules change?**

---

## Page 37: The Election Without Ballot Papers

One Saturday, Amina attended her chama meeting.

The group needed to choose a new treasurer.

Each member wrote a name on a small piece of paper. The chairperson counted the votes while two other members watched.

The process depended on rules.

Only registered members could vote.

Each member had one vote.

The winner needed more votes than the other candidates.

The counting had to be observed.

Amina thought about blockchains.

“Bitcoin uses mining to choose who adds the next block,” she told Kamau later. “Do all blockchains use mining?”

“No,” Kamau said. “Many use a different system called proof of stake.”

**Proof of stake** is a way for a blockchain network to choose participants who help create and confirm new blocks.

Instead of proving that they used large amounts of computing work, participants lock up crypto assets as a stake.

The locked assets act like a security deposit.

A participant who follows the rules may earn rewards.

A participant who seriously breaks the rules may lose some of the stake.

Amina compared this with hiring a contractor.

A customer may ask the contractor to provide a deposit or guarantee. If the contractor completes the work honestly, the deposit is returned. If the contractor causes damage or disappears, part of the deposit may be used to cover the loss.

Proof of stake uses a similar idea, but inside a blockchain system.

The network does not simply trust a validator because the validator says, “I am honest.”

It creates an economic reason to behave honestly.

This is important because strangers on the internet may not know one another.

A proof-of-stake system usually includes:

- validators who lock assets,
- rules for choosing who proposes a block,
- other validators who check the proposal,
- rewards for correct participation,
- and penalties for serious dishonest behaviour.

Different blockchains design these rules differently.

Some require a large minimum stake.

Some allow people with small amounts to join through a pool.

Some choose validators partly at random.

Some give more selection chance to validators with larger stakes.

Amina asked the obvious question.

“Does that mean rich people control everything?”

Kamau answered carefully.

“Large holders can gain more influence in some systems. That is one of the main concerns. But the exact level of control depends on the network design, how widely tokens are distributed, how validators are organised, and whether users can move their support.”

Proof of stake does not remove power.

It distributes power according to a different rule.

Proof of work gives influence to miners who control computing equipment and electricity.

Proof of stake gives influence to participants who lock the network’s asset.

Each system has strengths and weaknesses.

Amina wrote:

> Consensus is not only a technical choice. It is also a choice about who gets power and what they must risk.

---

## Page 38: The Validators at the Gate

The following week, Amina visited a gated apartment building to deliver tea for a meeting.

A guard checked the visitor list before opening the gate.

He did not own the building.

He did not decide who lived there.

His job was to check whether visitors followed the building’s rules.

Kamau used the example to explain **validators**.

A validator is a participant in a proof-of-stake network that helps check transactions and maintain the blockchain.

A validator may:

- check whether transactions follow the rules,
- propose a new block,
- confirm blocks proposed by others,
- reject invalid information,
- and help the network agree on one shared history.

A validator does not normally decide that Amina deserves more coins.

It checks whether the transaction follows the existing rules.

For example, it may check whether:

- the sender has enough balance,
- the digital signature is valid,
- the transaction format is correct,
- the same funds were not already spent,
- and the smart contract instructions were followed.

To become a validator, a person or company may need to lock a required amount of the network’s token.

This is called **staking**.

The staked tokens are not a payment to the network.

They remain connected to the validator, but they may be temporarily locked and exposed to penalties.

In return for helping the network, validators may earn rewards.

The rewards may come from newly created tokens, transaction fees, or both.

Amina asked, “Can I stake with only a small amount?”

“Sometimes,” Kamau said. “You may delegate to a validator or join a staking pool.”

**Delegation** means allowing a validator to use the weight of your tokens without giving the validator full ownership of them.

A **staking pool** combines contributions from many users.

This can help smaller holders participate.

But it introduces risks.

The pool operator may charge fees.

The validator may perform badly.

A smart contract may contain a bug.

The platform may keep custody of the assets.

Withdrawals may take time.

The token price may fall even while the number of tokens increases.

This last point surprised Amina.

Suppose she stakes 100 tokens and earns 8 more.

She now has 108 tokens.

But if the market price falls by half, the shilling value of her holdings may still be much lower.

A high staking percentage does not guarantee profit.

It only describes token rewards.

Amina wrote another rule:

> Always separate the number of tokens earned from the real value and risk of those tokens.

---

## Page 39: When the Security Deposit Is Cut

At the tea stall, a supplier once promised to deliver flour before sunrise.

He failed to arrive.

Amina lost morning customers because she could not make enough mandazi.

The supplier later apologised, but Amina needed stronger protection.

For the next order, they agreed that he would leave a small deposit. If he failed without a good reason, he would lose part of it.

In proof-of-stake networks, a serious validator penalty is often called **slashing**.

Slashing removes part of a validator’s stake when the validator breaks important network rules.

This is not meant to punish every small technical problem.

Different networks have different rules.

But slashing may happen when a validator:

- signs two conflicting versions of a block,
- tries to approve dishonest history,
- coordinates an attack,
- or behaves in another way that threatens consensus.

A validator that goes offline may also lose rewards or face smaller penalties.

The goal is to make attacks expensive.

Imagine a validator could cheat, earn money, and lose nothing when caught.

Dishonesty would be attractive.

But if cheating risks a large locked stake, the calculation changes.

This is an example of **crypto-economic security**.

The network combines software rules with financial incentives.

It does not only say, “Do not cheat.”

It says, “Cheating may cost more than honesty earns.”

However, economic incentives are not perfect.

A rich attacker may accept a large loss for political or strategic reasons.

A software bug may punish honest validators.

A staking service may spread one mistake across many users.

If too much stake is controlled by a few companies, the network may become less decentralised.

Amina asked how she could judge a proof-of-stake network.

Kamau suggested several questions:

1. How many independent validators exist?
2. How much stake do the largest validators control?
3. Can ordinary users delegate easily?
4. What behaviour causes slashing?
5. How long are tokens locked?
6. Who writes and updates validator software?
7. What happens if many validators go offline?
8. Can the network recover from a major attack?

Amina noticed a pattern.

The simple word “staking” hid many decisions.

A platform advertisement might say, “Earn 15 percent.”

It might not explain token inflation, lock periods, slashing, custody, smart contract risk, or price volatility.

The reward was visible.

The risk was in smaller writing.

> In crypto, a reward is often payment for taking a risk. Find the risk before chasing the reward.

---

## Page 40: The Token That Came With a Vote

Amina’s chama later considered buying a delivery motorcycle.

Some members supported the idea.

Others wanted to save the money for emergencies.

The chairperson asked everyone to vote.

Kamau explained that some crypto projects also use voting.

They may issue a **governance token**.

A governance token can give holders the ability to vote on certain project decisions.

These decisions may include:

- changing fees,
- choosing how treasury money is used,
- adding new collateral assets,
- changing reward rates,
- funding developers,
- or upgrading smart contracts.

Governance sounds democratic, but the details matter.

In many systems, one token equals one vote.

A person with one million tokens may have far more voting power than a person with ten tokens.

This is different from a national election where each citizen normally receives one vote.

Token voting is closer to company shareholder voting.

Ownership brings influence.

Amina asked, “What if most people do not vote?”

“That happens often,” Kamau said.

Many token holders may ignore proposals.

Some may not understand them.

Some may keep tokens on exchanges and never participate.

A few large holders may decide the result.

Projects may try to solve this through:

- delegated voting,
- voting rewards,
- minimum participation rules,
- time delays,
- public discussion forums,
- committees,
- or special emergency powers.

Each solution creates another trade-off.

Delegation can make voting easier, but popular delegates may collect too much power.

Emergency powers can stop an attack, but they can also become central control.

Time delays give users time to react, but slow urgent fixes.

Amina learned that a governance token may have several sources of value.

It may provide voting rights.

It may receive part of protocol fees.

It may be required for staking.

It may only be used for speculation.

A project calling a token “governance” does not automatically make it useful.

Amina wrote five questions:

1. What decisions can token holders actually make?
2. Who owns most of the tokens?
3. How many holders normally vote?
4. Can developers ignore the vote?
5. Does the token have any purpose beyond creating demand for itself?

She underlined the final question.

A vote is meaningful only when it can change something real.

---

## Page 41: The Organisation With No Office

Kevin showed Amina an online community that called itself a DAO.

“It has members in many countries,” he said. “They manage money together, but there is no main office.”

DAO stands for **decentralised autonomous organisation**.

The name can sound more advanced than the reality.

A DAO is usually a group that coordinates decisions using online tools, blockchain wallets, smart contracts, and tokens.

A DAO may manage:

- a shared treasury,
- a software protocol,
- an investment club,
- a grant programme,
- an online community,
- digital art,
- or a public project.

The word **decentralised** means control is spread among participants to some degree.

The word **autonomous** suggests that some rules can run automatically through smart contracts.

But most DAOs are not fully automatic.

People still write proposals.

People debate.

People vote.

Developers write code.

Signers approve transactions.

Lawyers may advise the group.

Community members may disagree.

Amina compared a DAO with her chama.

Both could collect money from members.

Both could vote.

Both could fund projects.

Both needed records and rules.

The difference was that a DAO could operate across borders and use blockchain tools to hold funds and execute approved actions.

For example, a DAO treasury might use a multi-signature wallet.

A **multi-signature wallet** requires several approved people to sign before funds can move.

Three out of five signers may need to approve a payment.

This reduces dependence on one treasurer.

But a DAO still faces difficult questions.

Who can join?

Who can propose an idea?

Who can vote?

How are conflicts solved?

What legal responsibilities exist?

What happens if the smart contract is hacked?

What if token holders approve something harmful?

What if a small group quietly controls most votes?

A DAO can distribute decision-making.

It cannot remove human politics.

Amina smiled.

“Even on blockchain, meetings are still meetings.”

Kamau laughed.

“Yes. Technology can change the tools. It does not change human nature.”

---

## Page 42: How a Smart Contract Learns the Price of Maize

Amina understood that smart contracts could follow blockchain data.

A contract could see token balances and transactions.

But she wondered how it could know something outside the blockchain.

“How can a lending app know the price of the collateral?” she asked.

“How can an insurance contract know whether rain fell in Kitui?”

Kamau introduced **oracles**.

An oracle is a service or system that brings outside information into a blockchain application.

A blockchain cannot automatically know the weather, the shilling-dollar exchange rate, a football result, or the price of maize.

Someone or something must provide that information.

Oracles may provide:

- market prices,
- weather data,
- election results,
- sports scores,
- shipping information,
- interest rates,
- and proof that an event happened.

Amina imagined a crop insurance contract.

Farmers pay a small premium.

If rainfall in a certain area falls below a defined level, the contract pays them automatically.

The smart contract needs reliable rainfall data.

If the data is wrong, the payment will also be wrong.

This creates the **oracle problem**.

A blockchain may execute code perfectly, but the result can still fail if the outside data is false or manipulated.

One oracle provider creates a central point of failure.

A dishonest provider could report a fake price.

A technical problem could send old data.

A hacked account could affect millions of shillings in smart contracts.

Decentralised oracle systems try to reduce this risk by collecting information from several independent sources.

They may compare results and ignore unusual answers.

But decentralisation does not guarantee truth.

Several sources may all depend on the same original data.

A fast market crash may make prices change before the oracle updates.

Attackers may manipulate a small exchange used as a price source.

Amina learned to ask:

1. Where does the data come from?
2. How many independent sources provide it?
3. How often is it updated?
4. What happens when sources disagree?
5. Can one company change the result?
6. What happens if the oracle stops working?

She wrote:

> A smart contract is only as reliable as its code, its data, and the systems around it.

---

## Page 43: The Token Cake

For Kevin’s birthday, Amina baked a cake.

Before cutting it, she decided how many slices there would be.

Some slices went to family.

Some went to neighbours.

One large slice was kept for visitors arriving later.

Kamau used the cake to explain **tokenomics**.

Tokenomics means the economic design of a crypto token.

It studies how tokens are created, distributed, used, and removed from circulation.

Important tokenomics questions include:

- What is the maximum supply?
- How many tokens exist today?
- How many are available for trading?
- Who received the first tokens?
- How quickly will new tokens enter the market?
- What is the token used for?
- Can tokens be burned?
- Can the rules change?

A token may have a maximum supply of one billion units.

But perhaps only one hundred million are currently circulating.

The other nine hundred million may belong to founders, investors, a treasury, or future reward programmes.

This difference matters.

A token can look scarce today while a large future supply waits to enter the market.

When locked tokens become available, this is called an **unlock**.

A **vesting schedule** controls when founders, workers, or investors may receive or sell their tokens.

Vesting can prevent everyone from selling immediately after launch.

For example, an investor’s tokens may be locked for one year, then released slowly over three years.

But unlocks can still create selling pressure.

Amina learned three supply terms:

**Circulating supply** is the amount generally available in the market.

**Total supply** is the number that exists after subtracting tokens permanently destroyed.

**Maximum supply** is the highest amount allowed by the rules, if a maximum exists.

She also learned about market value.

A token’s **market capitalisation** is often calculated as:

**Price multiplied by circulating supply.**

A token costing only 10 shillings is not automatically cheap.

If ten billion tokens circulate, the project may already have a very large market value.

The price of one unit tells only part of the story.

Amina wrote:

> Do not ask only, “What is the token price?” Ask, “How many tokens exist, who owns them, and how many are coming?”

---

## Page 44: The Fast Road Built Beside the Main Road

Amina travelled upcountry during a holiday weekend.

The main highway was crowded.

Cars moved slowly because too many people were using the same road.

A new side road allowed some vehicles to move faster, then return to the main highway later.

This helped her understand blockchain scaling.

A **Layer 1** is the main blockchain network.

Bitcoin and Ethereum are examples of Layer 1 networks.

They maintain their own consensus and transaction history.

A **Layer 2** is a system built on top of a Layer 1 to process activity more efficiently.

It may handle many transactions away from the main chain, then send a summary or proof back to the Layer 1.

The main goal is to improve speed, cost, or capacity while still using the security of the underlying chain.

On Ethereum, some Layer 2 systems group many transactions into one package.

This is called a **rollup**.

Instead of every small action taking full space on the main chain, the Layer 2 compresses the information.

Users may pay lower fees.

Applications may feel faster.

But Layer 2 networks introduce new questions.

How do users move money in and out?

Who runs the transaction sequencer?

Can withdrawals be delayed?

What happens if the Layer 2 software fails?

Are fraud proofs or validity proofs working correctly?

Can the team upgrade the contracts?

Amina learned that different scaling methods make different trade-offs.

Some prioritise speed.

Some prioritise low fees.

Some prioritise privacy.

Some depend on a small group of operators.

A cheap transaction is useful, but cost is not the only measure.

A road may be fast because it has no traffic police, poor lighting, and weak construction.

Speed alone does not make it safe.

Amina wrote:

> When a network says it is faster and cheaper, ask what it gives up and who you must trust.

---

## Page 45: The Public Window and the Curtains

Amina once believed crypto transactions were anonymous.

Then Kamau opened a blockchain explorer.

He showed her a public address and its transaction history.

The explorer displayed money entering and leaving the address.

It showed dates, amounts, fees, and connected addresses.

“Can everyone see this?” she asked.

“On many public blockchains, yes.”

Public blockchains are often **pseudonymous**, not fully anonymous.

A wallet address may not show a person’s legal name.

But activity connected to the address is public.

If an exchange, merchant, social media post, or investigation connects the address to Amina, other transactions may also become easier to study.

**Blockchain analysis** uses public transaction data to identify patterns and connections.

Analysts may follow funds after a hack.

Exchanges may check whether deposits came from risky addresses.

Law enforcement may investigate fraud.

Researchers may study how networks are used.

But analysis can also affect privacy.

A business may not want competitors to see supplier payments.

A worker may not want the public to estimate her salary.

A family may not want strangers studying its savings.

Some crypto systems use privacy tools.

These may hide amounts, mix transaction paths, or use cryptographic proofs that reveal less information.

One advanced tool is a **zero-knowledge proof**.

It can allow someone to prove a statement without revealing all the private information behind it.

For example, a person might prove that she is over eighteen without showing her full date of birth.

In crypto, zero-knowledge technology can support private transactions or help Layer 2 networks prove that many transactions were processed correctly.

Privacy tools also create debate.

Ordinary users need privacy.

Criminals may also try to hide stolen funds.

Governments and companies must balance privacy, security, and legal duties.

Amina wrote:

> Public does not always mean identified. Private does not always mean criminal.

The important question was what information the system revealed, to whom, and under what conditions.

---

## Page 46: When Crypto Meets the Law

One morning, a customer asked Amina whether crypto was legal in Kenya.

She almost answered quickly.

Then she remembered Kamau’s warning about simple answers.

Crypto regulation can cover many different activities.

A country may treat buying crypto differently from running an exchange.

Holding a token may be allowed while advertising an investment without permission is restricted.

Tax rules may apply even when no special crypto law exists.

Different authorities may oversee different parts of the market.

Regulation may address:

- customer identity checks,
- anti-money-laundering controls,
- consumer protection,
- exchange licensing,
- custody of customer assets,
- stablecoin issuance,
- securities and investment products,
- taxes,
- data protection,
- and cross-border payments.

Amina learned the term **KYC**, which means Know Your Customer.

A regulated platform may ask for identification, a photograph, an address, or information about the source of funds.

The purpose is to reduce fraud, money laundering, and misuse of the financial system.

She also learned **AML**, which means anti-money laundering.

AML controls may include transaction monitoring, record keeping, and reporting suspicious activity.

Some crypto users dislike these checks because they value privacy and open access.

But businesses that connect crypto with banks and national currencies often have legal responsibilities.

Regulation can provide useful protection.

It may require companies to keep customer assets separate, explain risks, maintain security, and respond to complaints.

Poor regulation can also create problems.

Rules may be unclear.

Small businesses may face costs they cannot afford.

Innovation may move elsewhere.

Bad actors may continue operating outside the rules.

A licence is not a guarantee that a company will never fail.

Amina created a careful answer for customers:

“Do not ask only whether crypto is legal. Ask what activity you want to perform, which platform you plan to use, what current Kenyan rules apply, and what tax or reporting duties you may have.”

Laws can change.

Before acting, a person should check current information from official authorities or a qualified professional.

---

## Page 47: Amina Investigates a New Coin

A stranger sent Kevin a message about a new token called HarakaCoin.

The message promised that the price would increase one hundred times.

It claimed the project would “bank every African by next month.”

Kevin was excited.

Amina was not convinced.

She decided to investigate.

First, she studied the problem.

What problem did HarakaCoin claim to solve?

Was the problem real?

Did the solution need a blockchain or token?

Second, she studied the team.

Were the founders real people?

Did they have relevant experience?

Could their history be checked?

Had they built anything before?

Third, she studied the product.

Was there a working application?

Could ordinary people use it?

Were users active, or did the project only have social media followers?

Fourth, she studied the token.

What was it used for?

How many tokens existed?

Who owned most of them?

When would locked tokens become available?

Could the team create more?

Fifth, she studied the code and security.

Was the code public?

Had independent experts reviewed it?

Did administrators have special powers?

Could the smart contract be changed?

Sixth, she studied the community.

Did people ask serious questions?

Were critics insulted or blocked?

Did every discussion focus only on price?

Seventh, she studied the money.

How was the project funded?

Did it have real revenue?

Was the treasury transparent?

How long could the team continue operating?

Eighth, she studied the legal and market risks.

Could regulators treat the token as an investment product?

Was trading concentrated on one small exchange?

Was liquidity deep enough for holders to sell?

Amina discovered that two anonymous wallets controlled most of the token supply.

The project had no working product.

The founders used stock photographs.

The promised partnership could not be confirmed.

The smart contract allowed the creator to block selling.

Kevin slowly put down his phone.

“The logo looked professional,” he said.

Amina replied, “A good logo is not due diligence.”

---

## Page 48: Utility, Hype, and the Question That Matters

Amina had now studied many crypto projects.

Some moved real value across borders.

Some provided useful financial tools.

Some helped creators build digital communities.

Some were experiments that might become useful later.

Others existed mainly to create excitement and sell tokens.

Kamau asked her to imagine two businesses.

The first business had a loud launch.

Influencers promoted it.

The token price rose quickly.

The website used words such as revolutionary, unstoppable, and guaranteed.

But the product had almost no users.

The second business had a small community.

Its product solved one clear problem.

Users paid modest fees because the service was helpful.

The team published regular reports and admitted its weaknesses.

“Which one has more utility?” Kamau asked.

“The second one,” Amina said.

**Utility** means practical usefulness.

A crypto network or token may have utility if it helps people do something valuable.

Examples include:

- transferring value,
- paying network fees,
- securing a blockchain,
- accessing a service,
- representing ownership,
- coordinating a community,
- or providing collateral.

But utility does not guarantee a token will rise in price.

A useful network may have a poorly designed token.

A useless token may rise for a while because of speculation.

Price and usefulness can move separately.

Amina learned to separate four questions:

1. Is the problem real?
2. Is the product useful?
3. Is blockchain necessary?
4. Does the token capture any value from the product?

A project can succeed while its token disappoints.

A token can rise while the project fails to create lasting value.

This distinction was one of the most advanced lessons Amina had learned.

Crypto research is not about finding certainty.

Certainty does not exist.

It is about reducing ignorance.

It is about understanding what could go right, what could go wrong, and whether the possible reward justifies the risk.

Amina looked at the first page of her notebook.

Months earlier she had written one question:

**What is money?**

Now she understood money as trust, records, rules, power, technology, incentives, and human behaviour.

She had travelled far.

But the journey was not finished.

The next part would explore advanced ideas about cryptography, zero-knowledge systems, restaking, interoperability, real-world assets, central bank digital currencies, decentralised identity, protocol revenue, attacks, governance failures, and how crypto may fit into Africa’s future.

Before closing her notebook, she wrote:

> Do not ask whether crypto is good or bad. Ask which system, for which purpose, under which rules, with which risks.

---

# Learning Checkpoint Four

### 1. What is proof of stake?

A consensus method where participants lock crypto assets and help verify the network, earning rewards for honest behaviour and risking penalties for serious rule breaking.

### 2. What is a validator?

A network participant that checks transactions and helps propose or confirm blocks on a proof-of-stake blockchain.

### 3. What is slashing?

A penalty that removes part of a validator’s stake after serious dishonest or dangerous behaviour.

### 4. What is a governance token?

A token that may give holders voting power over certain project or protocol decisions.

### 5. What is a DAO?

A group that coordinates decisions and shared resources using online communities, tokens, wallets, and smart contracts.

### 6. What is an oracle?

A system that supplies a blockchain application with information from outside the blockchain.

### 7. What is tokenomics?

The design of a token’s supply, distribution, uses, incentives, unlocks, and economic rules.

### 8. What is a Layer 2?

A system built on top of a main blockchain to process transactions more efficiently while using the main chain for settlement or security.

### 9. Are public blockchain transactions anonymous?

Usually not fully. They are often pseudonymous, meaning addresses are public even when legal names are not directly shown.

### 10. What is the first question to ask about a crypto project?

What real problem does it solve, and does that problem need blockchain or a token?

---

# What Comes Next

## Part Five: Advanced Crypto Without the Confusion

The next installment will cover:

1. Cryptography beyond passwords
2. Zero-knowledge proofs
3. Restaking and shared security
4. Interoperability and cross-chain messaging
5. Real-world assets on blockchain
6. Central bank digital currencies
7. Decentralised identity
8. Protocol revenue and value capture
9. Common blockchain attacks
10. Governance failures and emergency powers
11. Crypto’s possible role in Africa
12. Building a personal crypto risk framework
