# Part Two: Meeting Bitcoin

This part continues directly from Page 12 of **Crypto, Pole Pole**.

Amina now understands why money works, how ledgers record ownership, why digital money must prevent double spending, and what problem Bitcoin tried to solve.

Now she is ready to look inside the system.

---

## Page 13: What Is a Bitcoin, Really?

The next morning, Amina opened her tea stall earlier than usual.

She had spent part of the night thinking about one sentence:

**Bitcoin is not a coin inside a phone. It is ownership recorded and protected by a network.**

But the sentence still felt strange.

When Kamau arrived for tea, she asked him the question immediately.

“What exactly is a bitcoin?”

Kamau sat on a plastic chair and placed his phone on the table.

“Let us begin with what it is not,” he said.

“A bitcoin is not a physical coin. It is not a shiny gold object with the letter B on it. Those pictures are only symbols used by websites, television stations, and advertisers.”

Amina nodded.

“So where is it?”

“It exists as part of the Bitcoin ledger.”

Kamau explained that the Bitcoin network keeps a public record of transactions. That record shows which pieces of bitcoin can be spent and what conditions must be met before they move.

Amina frowned.

“That sounds like an account balance.”

“It can look like one, but Bitcoin does not work exactly like a bank account.”

In a bank, the bank normally keeps an account under a customer’s name. The bank updates the account balance when money enters or leaves.

Bitcoin instead tracks pieces of value created by earlier transactions. These spendable pieces are commonly called **unspent transaction outputs**, or **UTXOs**.

The term sounded difficult, so Kamau used Amina’s cash tin.

Suppose she had three notes:

- one 500-shilling note,
- one 200-shilling note,
- and one 100-shilling note.

Together, she had 800 shillings.

Her total balance was 800, but it was made from separate pieces.

Bitcoin is similar in one important way. A wallet may show one total, but that total can be made from several spendable outputs created by earlier transactions.

If Amina wanted to pay 600 shillings using her physical notes, she might give the 500 note and the 200 note. The receiver would then return 100 shillings as change.

A Bitcoin transaction can also use earlier outputs and create new outputs. One output may go to the receiver. Another may return change to the sender.

“Does the network know my name?” Amina asked.

“Usually, the basic Bitcoin ledger records addresses and transaction details, not ordinary names. But that does not make every transaction completely private. People and companies can sometimes connect addresses to real identities through exchanges, payment records, repeated behaviour, or other information.”

This was Amina’s first privacy lesson.

Bitcoin is often described as anonymous, but **pseudonymous** is usually more accurate.

A pseudonym is a label that is not automatically the same as a legal name.

A Bitcoin address can act like such a label.

The ledger may show that value moved from one address to another. It may not directly show “Amina bought flour.” But if someone learns that the address belongs to Amina, they may study its history.

Amina wrote four points in her notebook:

1. Bitcoin is digital value recorded on a shared ledger.
2. A wallet balance may be made from separate spendable outputs.
3. Bitcoin addresses are not the same as bank account names.
4. Public does not always mean people immediately know who you are, but it also does not mean perfect privacy.

Then she asked, “Can I buy less than one bitcoin?”

“Yes. One bitcoin can be divided into 100 million smaller units. The smallest standard unit is called a **satoshi**, or **sat**.”

Kamau wrote:

**1 bitcoin = 100,000,000 satoshis**

Amina laughed.

“So I do not need millions of shillings before I can own Bitcoin?”

“No. A person can own a small fraction.”

This mattered because many beginners see the price of one whole bitcoin and assume they are locked out.

But the network does not require everyone to buy one full bitcoin.

Just as a person can have 50 cents without owning a full dollar, a person can own sats without owning one full bitcoin.

The amount may be small, but the safety responsibility is still real.

Amina now had a clearer answer:

> A bitcoin is not a file or a coin stored inside a phone. It is a divisible unit of value whose ownership and spending rules are recorded on the Bitcoin network.

---

## Page 14: The Wallet That Holds No Coins

That afternoon, Amina downloaded a Bitcoin wallet application for learning.

Before doing anything serious, Kamau told her to stop.

“First understand what a wallet is.”

Amina looked at the app.

“It holds bitcoin.”

“Not exactly.”

He picked up her leather purse.

“This purse holds cash. A Bitcoin wallet does not hold bitcoin in the same physical way.”

The bitcoin remains recorded on the network’s ledger.

The wallet manages the secret information needed to prove that the user is allowed to spend certain bitcoin.

This secret information includes **private keys**.

A wallet may also:

- create receiving addresses,
- show balances,
- prepare transactions,
- sign transactions,
- calculate fees,
- and help the user back up access.

Amina thought about a house.

The house stays where it is. A key does not contain the house. The key gives access to the house.

The comparison was not perfect, but it helped.

A Bitcoin wallet does not carry coins like a purse. It carries or controls the keys that allow spending.

There are many kinds of wallets.

### Mobile wallets

These run on a smartphone.

They can be convenient for small, everyday amounts. But phones can be lost, stolen, damaged, infected, or unlocked by another person.

### Desktop wallets

These run on a computer.

They may offer more features, but the computer must be protected from malware and unauthorised access.

### Hardware wallets

These are specialised devices designed to keep private keys away from ordinary internet-connected environments.

They can improve security when used correctly, especially for larger amounts. But users must still buy from trustworthy sources, protect recovery information, verify transaction details, and avoid fake support messages.

### Paper or offline backups

Some users write recovery words or key information on paper or another offline material.

This avoids some online risks, but creates physical risks. Paper can burn, fade, get wet, be photographed, or be found by someone else.

### Custodial accounts

An exchange or another service may hold the keys for the user.

The user logs in with an email, phone number, password, or other account method.

This can feel easier because the service may help with password recovery.

But the service controls the private keys.

If it freezes withdrawals, is hacked, becomes insolvent, or closes, the user may lose access.

This is the meaning behind a famous crypto phrase:

**Not your keys, not your coins.**

Kamau warned Amina that the phrase should not be treated as magic.

Self-custody gives more control, but it also gives more responsibility.

A beginner who loses a seed phrase may lose funds permanently.

A beginner who uses a reputable custodian may avoid that risk, but accepts company risk instead.

There is no option with zero risk.

The question is where the risk sits.

Amina drew two columns.

| Custodial service | Self-custody wallet |
|---|---|
| Company holds keys | User controls keys |
| Password recovery may be possible | Recovery depends on backup |
| Company can freeze or limit access | No company is needed to approve spending |
| Company can fail or be hacked | User can make irreversible mistakes |
| Easier for some beginners | More responsibility |

“What should I use?” Amina asked.

“That depends on the amount, your knowledge, your purpose, and your ability to protect backups. Start by learning with a very small amount. Do not rush into storing serious savings.”

Amina liked this answer because it did not pretend there was one perfect wallet for everybody.

A wallet is a tool.

A person must understand the tool before trusting it with value.

---

## Page 15: The Address on the Screen

The wallet showed Amina a long group of letters and numbers.

She stared at it.

“What language is this?”

“That is a Bitcoin address,” Kamau said.

A Bitcoin address is information a sender can use when creating a payment.

It is similar to a destination label.

When Amina wanted someone to send money to her mobile wallet, she gave them her phone number. In Bitcoin, she could provide an address or a QR code representing that address.

But the comparison with a phone number has limits.

A phone number is usually connected to an account managed by a company. A Bitcoin wallet can create many addresses without asking a central company for permission.

Amina tapped the receive button.

The wallet displayed a QR code.

“Can I just show this to the sender?”

“Yes, but verify the details.”

A QR code reduces typing mistakes, but it does not remove every danger.

Malware can sometimes replace an address copied on a device. A scammer may present a fake QR code. A person may choose the wrong network on an exchange.

For important payments, users should compare part of the address on both devices and confirm the correct network.

Bitcoin addresses can have different formats.

A beginner does not need to memorise every format immediately. The important lesson is that software and services must support the address type being used.

Amina asked whether one address could be used forever.

“It can sometimes receive more than once, but good wallets often create a fresh address for each payment. Reusing an address can make privacy worse because observers can more easily connect transactions.”

This surprised her.

She had assumed one person needed one permanent address.

But a wallet can manage many addresses that all belong to the same recovery system.

Kamau then explained another difference between an address and a private key.

An address can be shared.

A private key must remain secret.

Amina could put a receiving QR code at her tea stall if she wanted customers to pay her.

But she should never display the private key or seed phrase.

“Think of the address as the location of a locked contribution box,” Kamau said. “People can know where the box is and place value into it. The private key is what allows the value to be moved.”

Again, the comparison was not perfect, but the difference mattered.

Amina practised with a tiny test payment from Kamau.

Before he sent it, he asked her to read the first and last few characters of the address.

She did.

He checked them on his screen.

Then he sent a very small amount.

The wallet showed a pending transaction.

Amina became excited.

“It has arrived!”

“Slow down. It has been broadcast. Now let us talk about confirmations.”

Amina sighed.

Every answer seemed to open another door.

That was how learning worked.

---

## Page 16: Public Keys, Private Keys, and a Padlock

The next lesson began with two padlocks.

Kamau brought them to the tea stall and placed them on the table.

“Cryptography uses mathematics instead of metal,” he said, “but let us use these to build the idea.”

A Bitcoin wallet creates secret numbers called private keys.

From a private key, related public information can be created.

The public and private parts have different jobs.

The **private key** is used to create a digital signature.

The signature proves that the spender has the required secret without publishing the secret itself.

The **public key** helps others verify that signature.

Amina asked the obvious question.

“If the public key is public, can someone use it to calculate the private key?”

Bitcoin depends on mathematical problems designed to make that reverse calculation extremely difficult with available computing power.

It is easy for software to create a public key from a private key.

It is not practically easy to start with the public key and discover the private key.

Kamau compared this to mixing paint.

It is easy to mix several colours together. It is much harder to perfectly separate the final mixture back into the exact original drops.

The real mathematics is different, but the direction matters.

Easy one way.

Extremely difficult in reverse.

Amina then asked whether a digital signature looked like her handwritten signature.

“No. It is produced mathematically from the transaction and the private key.”

The signature is connected to the specific transaction.

If someone changes important transaction details, the old signature should no longer be valid.

This helps the network detect tampering.

Suppose Amina creates a payment sending a small amount to Kevin.

Her wallet prepares the transaction.

It uses the required private key to sign it.

Nodes can check the signature using public information.

If the signature is valid and the bitcoin has not already been spent, the transaction may be accepted according to network rules.

The private key does not need to be sent to every node.

This is crucial.

A secure system should allow proof without revealing the secret itself.

Amina wrote:

> A private key gives spending authority. A digital signature proves authority for a transaction without revealing the private key.

Kamau warned her about screenshots.

Never take a casual screenshot of a private key or seed phrase.

Screenshots may be uploaded automatically to cloud storage. Other apps may access photos. A repair technician may see them. A stolen phone may expose them.

Never send the secret words to a person claiming to be support staff.

A real wallet recovery process does not require giving the seed phrase to a stranger in a chat.

Never type the seed phrase into a website because a message says the wallet must be “verified.”

Crypto scammers often use technical language to create panic.

They may say:

- your wallet is suspended,
- your funds are at risk,
- an upgrade is required,
- a reward is waiting,
- or your account must be synchronised.

The goal is often to make the victim reveal the secret.

Amina looked at the two padlocks again.

The lock was not the main lesson.

The secret was.

Whoever controls the secret may control the funds.

---

## Page 17: The Twelve Words That Can Restore a Wallet

Amina’s wallet displayed twelve ordinary words.

The app told her to write them down in the correct order.

She recognised every word.

None looked powerful.

One was the name of an animal. Another described an object. Another was a simple action.

“How can these words control money?” she asked.

Kamau explained that many modern wallets use a **seed phrase**, also called a recovery phrase or mnemonic phrase.

The words represent secret information from which the wallet can recreate many private keys and addresses.

The phrase is therefore not just another password.

It can be the master backup for the wallet.

If Amina’s phone fell into water, she could install a compatible wallet on another device and use the seed phrase to restore access.

But the same power creates danger.

If a thief obtained the words, the thief might restore the wallet elsewhere and move the funds.

The thief would not need Amina’s phone.

The thief would not need her fingerprint.

The thief might not need her wallet password.

The seed phrase could be enough.

Amina’s first idea was to save the words in her email.

Kamau stopped her.

Email accounts can be hacked. Cloud storage can be exposed. Screenshots can sync online. Notes apps may be readable by other people or services.

Her second idea was to send the words to herself through a messaging application.

That was also unsafe.

Her third idea was to write them on paper and hide them under her mattress.

“That removes some online risk,” Kamau said, “but think about fire, water, visitors, cleaners, family members, and simple forgetfulness.”

Security is not only about hiding.

It is about planning for several dangers:

- theft,
- accidental loss,
- fire,
- water,
- damage,
- memory failure,
- death or incapacity,
- and someone finding the backup too easily.

Amina realised that storing a seed phrase safely required balance.

If the backup was too easy to find, a thief could steal it.

If it was too well hidden, Amina herself might never find it.

If there was only one copy, one accident could destroy it.

If there were many careless copies, the chance of discovery increased.

For a small learning wallet, simple offline storage might be enough.

For larger value, people may consider stronger physical backups, secure locations, multisignature arrangements, or professional inheritance planning.

But complexity can also create mistakes.

A security plan should match the user’s knowledge and the amount being protected.

Amina made five rules:

1. Write recovery words offline.
2. Keep them in the correct order.
3. Do not photograph or message them.
4. Do not give them to support agents or friends.
5. Test the recovery process carefully before trusting the wallet with a large amount.

Kamau added one more rule.

“Never practise recovery with serious funds first.”

Amina could create a test wallet, deposit a tiny amount, remove the app, restore it, and confirm that she understood the process.

Learning with a tiny amount turns an expensive possible mistake into a cheap lesson.

---

## Page 18: How Amina Signed Her First Transaction

The small payment from Kamau was now visible in Amina’s wallet.

She wanted to send part of it to Kevin.

Kevin was sitting nearby and watching with great interest.

“Send it to me,” he said.

Amina entered the address from Kevin’s test wallet.

Before pressing the final button, Kamau asked her to pause.

A Bitcoin transaction has several important parts.

It refers to earlier spendable outputs.

It defines new outputs.

It includes the amount and destination conditions.

It may include a fee for miners.

It also needs valid signatures for the value being spent.

The wallet handles much of this automatically, but the user must still confirm the human details.

Is the address correct?

Is the amount correct?

Is the fee reasonable?

Is this the correct network?

Does the user trust the device?

Amina checked the first and last characters of Kevin’s address.

Then she checked the amount.

The wallet showed a network fee.

“Why must I pay a fee?” she asked.

Bitcoin blocks have limited space.

Users compete for inclusion when many transactions are waiting.

Fees give miners an economic reason to include transactions.

A transaction with a higher fee rate may be selected earlier than one with a lower fee rate, especially when the network is busy.

The fee is not normally based only on the value sent.

A large payment can sometimes cost less than a small payment if its transaction data uses less block space.

This confused Amina until Kamau returned to the cash-note example.

Imagine two people each want to pay 1,000 shillings.

One person uses one 1,000-shilling note.

The other uses fifty 20-shilling notes.

They send the same value, but one payment is more bulky.

Bitcoin fees are more closely connected to transaction data size and network demand than to the shilling value of the payment.

Amina approved the transaction.

Her wallet used the private key to create a signature.

The transaction was broadcast to nearby Bitcoin nodes.

Those nodes checked it and shared it with others.

Kevin’s wallet showed the incoming payment almost immediately.

“Done,” Kevin said.

“Broadcast,” Kamau corrected.

A transaction can be seen before it enters a block.

At that stage, it is often called **unconfirmed**.

It may be sitting in the **mempool**, a collection of valid transactions waiting for possible inclusion in a block.

Different nodes can have slightly different mempools because they receive information at different times or follow different local policies.

The transaction becomes more settled as miners include it in a block and later blocks build on top of that block.

For a tiny payment between people who trust each other, waiting may not be very important.

For a large sale, the receiver may wait for several confirmations.

Risk depends on the situation.

Amina had just made her first Bitcoin transaction.

But she now understood that pressing “send” was only one step in a larger process.

---

## Page 19: The Computers That Check the Rules

Amina imagined Bitcoin as one giant computer in a hidden building.

Kamau corrected her.

The network is made from many computers communicating with one another.

Some of these computers run **Bitcoin nodes**.

A full node downloads and verifies blockchain information according to the software rules it follows.

It checks things such as:

- whether transaction formats are valid,
- whether signatures satisfy spending conditions,
- whether the same output has already been spent,
- whether blocks follow size and structure rules,
- whether miners created only the allowed block reward,
- and whether the chain’s proof of work is valid.

A node does not simply trust a miner because the miner claims a block is correct.

It verifies the block.

Amina compared this to her chama.

Imagine the treasurer announced, “I have updated the records. Trust me.”

That would be centralised trust.

Now imagine every member had the rules and could independently check the contribution list and withdrawals.

That would distribute verification.

Bitcoin nodes help make the rulebook real.

A rule written in a document has little power if nobody checks it.

Nodes enforce rules by rejecting information that does not satisfy them.

“Can anyone run a node?” Amina asked.

“In principle, yes, if they have suitable equipment, storage, internet access, electricity, and the knowledge to maintain it.”

Running a node does not automatically earn bitcoin.

This is different from mining.

A node verifies.

A miner performs proof of work and tries to produce blocks.

Miners often run nodes too, but the jobs are not identical.

Amina asked why ordinary users should care about nodes.

If everyone relies on one company’s server, that company becomes an important source of truth.

By running a node, a user can verify transactions and rules independently instead of trusting a wallet provider’s report.

However, running a node has costs and practical challenges.

Not every beginner needs to start there.

The deeper lesson is that Bitcoin’s security comes from several groups doing different jobs.

Developers write and review software.

Nodes check rules.

Miners order transactions into blocks through proof of work.

Wallets help users create and sign transactions.

Exchanges connect buyers and sellers.

Users choose which software and services to trust.

No single role is the entire network.

Amina wrote:

> Miners propose blocks. Nodes verify them. Users decide what software and rules they accept.

This sentence protected her from a common misunderstanding.

Winning the mining race does not give a miner permission to break every rule.

A miner could produce a block claiming a reward larger than allowed.

Honest nodes would reject it.

The miner would have spent electricity creating a block the network did not accept.

Rules and incentives work together.

---

## Page 20: Blocks, Hashes, and the Chain

Kamau brought a stack of receipt books to the tea stall.

Each receipt book represented a block.

A Bitcoin block contains information about a group of transactions and other data needed by the protocol.

Blocks are created one after another.

Each block points back to the previous block through a cryptographic fingerprint called a **hash**.

A hash function takes input data and produces a fixed-size output.

Even a tiny change in the input normally produces a very different output.

Amina wrote two nearly identical sentences on paper:

- Amina paid Kevin 500 sats.
- Amina paid Kevin 501 sats.

Only one number changed.

But if software hashed the two messages, the outputs would be very different.

This makes hashes useful for detecting changes.

Kamau stamped each receipt book with a code connected to the previous one.

“If someone changes an old book, its fingerprint changes. The next book still points to the old fingerprint. The chain no longer matches.”

In Bitcoin, changing an old block would affect its hash and the links after it.

But noticing the change is not enough.

The system also uses proof of work, which makes rebuilding the chain expensive.

The attacker would need to redo work for the changed block and catch up with work added by honest miners.

The deeper a transaction sits under later blocks, the more work protects its history.

This is why confirmations matter.

Amina asked whether a blockchain was simply any database with linked pages.

“No. The word is used too broadly. A chain of blocks is one structure, but a serious blockchain system also needs rules about who can add data, how participants agree, how conflicts are resolved, and what security assumptions users accept.”

A private company could create a chain of blocks controlled by one administrator.

That may still be useful for record keeping, but its trust model would be different from Bitcoin.

The important question is not only, “Does it use blockchain?”

Better questions include:

- Who writes the blocks?
- Who verifies them?
- Who can change the rules?
- Can users leave?
- Is the history public?
- What makes rewriting records difficult?
- What happens when participants disagree?

Amina noticed that the word blockchain often attracted attention, but the design details determined what the system actually did.

A blockchain is not automatically honest.

It records what its rules and participants accept.

If bad information enters through a trusted person, a blockchain may preserve bad information very efficiently.

Technology can protect records after entry.

It cannot magically prove that every real-world statement was true before entry.

This is sometimes called the **oracle problem**, which Amina would study later.

For now, she understood the chain itself.

Each block linked to the previous one.

Hashes made changes visible.

Proof of work made accepted history expensive to rewrite.

Nodes checked the result.

---

## Page 21: The Mining Competition

Kevin had seen videos of noisy buildings filled with machines.

“Those are Bitcoin mines,” he said. “They dig coins from computers.”

The name mining creates that picture, but Bitcoin miners do not dig through soil.

They use specialised computers to perform repeated calculations.

Their goal is to find a valid block hash under the network’s current target.

The process involves changing a value and hashing block information again and again.

Most attempts fail.

A successful result proves that the miner performed a large amount of computational work.

This is called **proof of work**.

Kamau turned it into a simple game.

He wrote a secret condition on paper.

Then he gave Kevin and Amina dice.

“Keep rolling. The first person to roll the required pattern wins.”

Kevin could verify Amina’s winning roll quickly.

But producing the lucky pattern might take many attempts.

Proof of work has a similar useful difference.

Finding a valid result is difficult and costly.

Checking the result is much easier.

A winning miner broadcasts the proposed block.

Nodes verify the block and its proof of work.

If it follows the rules, nodes may add it to their accepted chain.

The miner can receive two main forms of reward:

1. newly issued bitcoin through the block subsidy,
2. transaction fees included in the block.

The reward gives miners a reason to spend money on machines, electricity, buildings, cooling, staff, and maintenance.

Amina asked why miners would not simply lie and award themselves more bitcoin.

Because nodes enforce the issuance rules.

A dishonest reward would make the block invalid.

The miner could spend real electricity producing a block that honest nodes reject.

Mining is also competitive.

A miner’s chance of finding the next block is connected to its share of total computing power, called **hashrate**.

A small miner may work for a long time without finding a block.

For this reason, many miners join **mining pools**.

A pool combines work from many miners and shares rewards according to contributed work.

Pools reduce income uncertainty, but they can also concentrate coordination power.

This led Amina back to decentralisation.

Bitcoin mining may involve thousands of machines, yet a smaller number of pools may coordinate much of the hashrate.

Decentralisation must be studied carefully, not assumed from a slogan.

Mining also uses energy.

Supporters argue that energy use secures a global monetary network and can use varied energy sources, including otherwise wasted energy in some settings.

Critics argue that the consumption and environmental effects can be too large or poorly justified.

Both the source of electricity and the value society places on the network matter to the debate.

Amina did not reduce the issue to “good” or “bad.”

She asked:

- How much energy is used?
- Where does it come from?
- What service does the network provide?
- What alternatives exist?
- Who bears the costs?
- Who receives the benefits?

Clear thinking required more than repeating a side’s favourite sentence.

---

## Page 22: Why the Difficulty Changes

In the dice game, Kamau could make winning easier or harder.

If any roll of six won, a winner would appear quickly.

If six sixes in a row were required, winning would take longer.

Bitcoin also adjusts the difficulty of mining.

The network aims for blocks to be found, on average, about every ten minutes.

But miners can add or remove computing power.

If much more hashrate joins and difficulty stays unchanged, blocks may appear too quickly.

If miners leave, blocks may appear too slowly.

Bitcoin periodically adjusts the mining target based on how long earlier blocks took.

When blocks came too quickly, mining becomes harder.

When they came too slowly, it becomes easier.

This adjustment helps keep issuance roughly on schedule even as total mining power changes.

Amina asked whether a block always arrives exactly ten minutes after the previous one.

“No. Ten minutes is an average, not an appointment.”

One block may arrive after a few seconds.

Another may take much longer.

Over many blocks, the average tends toward the target because of the difficulty system.

This reminded Amina of matatus.

A route may have an average travel time, but one trip can be fast and another slow because of traffic, rain, police checks, passengers, or road conditions.

An average describes a pattern, not a promise for each event.

The difficulty adjustment also helps protect the known supply schedule.

Miners cannot create unlimited bitcoin simply by buying more machines.

More machines increase competition.

Then the network adjusts.

The protocol still limits the reward per block.

This is an important separation of powers.

Miners provide work, but the protocol rules define the allowed issuance.

Nodes check those rules.

Users decide which rules they recognise.

Amina asked what would happen if most miners suddenly stopped.

Blocks could become slower until difficulty adjusted.

Transactions might wait longer.

The network would not necessarily disappear immediately, but its security and speed could be affected.

Bitcoin therefore depends on economic participation.

Its technology cannot be separated from incentives.

Miners continue because they expect rewards to justify costs.

Users transact because they believe the network is useful.

Markets give bitcoin a price.

Developers maintain software.

Node operators verify.

The system is technical, social, and economic at the same time.

---

## Page 23: Confirmations and the Meaning of Final

Kevin’s incoming payment had now entered a block.

His wallet displayed one confirmation.

Amina expected a large green message saying FINAL.

Instead, the confirmation number slowly increased as new blocks appeared.

In Bitcoin, a transaction receives its first confirmation when miners include it in a block accepted by the network.

Each later block adds another confirmation.

Why wait?

Sometimes two miners find valid blocks at nearly the same time.

Different parts of the network may briefly see different tips of the chain.

As more work is added, one branch becomes the accepted chain with the most accumulated proof of work under Bitcoin’s rules.

A transaction in the other branch may return to the mempool or be included later.

This temporary reorganisation is usually small, but it explains why a newly mined transaction is less settled than one buried under several blocks.

For low-value payments, a merchant may accept little or no confirmation depending on the risk.

For a house purchase or another very large transfer, parties may wait longer.

There is no single confirmation number that fits every situation.

Amina compared it to accepting a mobile money message.

If a stranger showed her a screenshot saying “payment sent,” she should not trust the screenshot.

She should check her own account.

For Bitcoin, a receiver should rely on trusted wallet information or independent verification, not only on a sender’s screen.

A fake transaction can be displayed in an edited image.

A transaction on the wrong network may look similar.

An unconfirmed transaction may be replaced in some situations.

Amina also learned that Bitcoin settlement is not the same as legal settlement.

The blockchain may show that bitcoin moved.

A court may still consider questions about fraud, contracts, theft, taxes, or ownership.

Technology records the transaction according to protocol rules.

Human society still applies laws and agreements around it.

Finality can therefore have several meanings:

- technical finality,
- economic finality,
- business acceptance,
- and legal finality.

Bitcoin gives **probabilistic finality**.

As more proof of work builds on a transaction, reversing it generally becomes less likely and more expensive.

It does not create a magical moment when the laws of mathematics declare that reversal is absolutely impossible under every imaginable condition.

Amina wrote:

> More confirmations usually mean stronger settlement, but the number needed depends on the value and risk of the transaction.

---

## Page 24: The Supply Schedule and Amina’s First Safety Rules

Amina now understood how transactions moved.

Her final question for this part was about supply.

“How are new bitcoins created?”

New bitcoin enters circulation through the block subsidy paid to miners who produce valid blocks.

The subsidy does not stay the same forever.

Roughly every 210,000 blocks, it is cut in half.

This event is called the **halving**.

The original block subsidy was 50 bitcoin.

It later fell to 25, then 12.5, then 6.25, and then lower again according to the rule.

Because the subsidy keeps shrinking, the total supply approaches a maximum of 21 million bitcoin.

The final amount is released gradually over a very long period.

Amina asked whether 21 million was too small for the whole world.

One bitcoin can be divided into 100 million sats.

That creates 2.1 quadrillion satoshis across the full maximum supply.

Units can be displayed in smaller forms if needed.

Scarcity is not about the number of whole coins alone.

It is about the supply rule and divisibility.

A fixed maximum does not guarantee a rising price.

Demand can increase or fall.

Governments can regulate access.

Technology can face risks.

Competing systems can develop.

Investors can change their minds.

A scarce thing can still be unwanted.

Bitcoin’s supply rule is one part of its value story, not proof of guaranteed profit.

As the block subsidy falls, transaction fees are expected to become a more important part of miner revenue.

This creates a long-term question.

Will fees be high enough to support strong security after subsidies become small?

Bitcoin supporters believe network use and value can create a sustainable fee market.

Critics question whether that will happen smoothly.

The future is not fully known.

Amina appreciated that honest education includes unanswered questions.

Before ending the lesson, Kamau asked her to write her first Bitcoin safety rules.

She wrote:

### Amina’s first twelve safety rules

1. Never invest money needed for rent, food, school fees, debt, or emergencies.
2. Begin with a tiny test amount.
3. Learn the difference between an address, a private key, and a seed phrase.
4. Never share a seed phrase or private key.
5. Do not keep recovery words in screenshots, email, or ordinary online notes.
6. Verify addresses and networks before sending.
7. Use a test transaction before moving a large amount.
8. Do not trust payment screenshots.
9. Download wallet software only from carefully verified sources.
10. Treat urgent support messages as suspicious.
11. Understand whether a service is custodial or self-custodial.
12. Slow down. Most expensive mistakes begin with hurry, greed, fear, or confusion.

Kevin read the rules.

“They sound serious.”

“They are,” Amina said. “This money has no undo button.”

That statement was almost correct, but Kamau refined it.

Some services may help before a withdrawal completes. Some transactions can be replaced under specific conditions. Courts may act against identifiable thieves. Exchanges may freeze stolen funds.

But a properly confirmed Bitcoin transaction cannot simply be reversed by calling Bitcoin customer care.

There is no central Bitcoin office.

Amina closed her notebook.

She could now explain:

- what a bitcoin is,
- what wallets really manage,
- how addresses receive value,
- how private keys authorise spending,
- why seed phrases matter,
- how transactions are signed and broadcast,
- what nodes verify,
- how blocks link together,
- what miners do,
- why proof of work is costly,
- why confirmations matter,
- and how Bitcoin’s supply schedule works.

She had moved beyond the door.

But Bitcoin was only the first room in a much larger building.

Other networks would introduce smart contracts, stablecoins, tokens, decentralised finance, and new forms of risk.

Before going there, she needed to compare Bitcoin with other blockchains and understand why people built them.

---

# Learning Checkpoint Two

### 1. Does a Bitcoin wallet hold physical or digital coins inside the phone?

No. The Bitcoin ledger records spendable value. The wallet manages keys and helps the user receive, view, and spend that value.

### 2. What is a private key?

It is secret information used to create valid digital signatures and authorise spending.

### 3. What is a seed phrase?

It is a human-readable recovery backup that can recreate a wallet’s keys. Anyone who obtains it may be able to control the funds.

### 4. What does a node do?

A node checks transactions and blocks against the Bitcoin rules it follows.

### 5. What does a miner do?

A miner performs proof of work and tries to produce a valid block containing transactions.

### 6. Why do confirmations matter?

Each later block adds more proof of work after the block containing a transaction, making reversal generally more difficult.

### 7. Does Bitcoin’s limited supply guarantee profit?

No. Price depends on demand, risk, regulation, market behaviour, technology, and many other factors.

### 8. What is the safest amount for a beginner’s first test?

An amount small enough that losing it would not affect the beginner’s life.

---

# What Comes Next

## Part Three: Beyond Bitcoin

The next installment will cover:

1. Why other blockchains were created
2. Ethereum and programmable money
3. Smart contracts
4. Gas fees
5. Tokens and token standards
6. Stablecoins
7. Centralised and decentralised exchanges
8. Liquidity pools
9. Decentralised finance
10. Oracles
11. Bridges and wrapped assets
12. Common smart-contract risks
