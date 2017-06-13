# What is mining?

Mining is the process of solving math problems provided by the Monero network. These problems get more difficult if more people are trying to solve them, and they get less difficult when less people are. The problems are difficult enough to be solved about once every two minutes.

Why bother giving miners problems to solve? The person who solves the problem can determine the latest Monero transactions to be included in the blockchain. If one person can make these decisions all the time, it could lead to censorship and attacks. Mining allows anyone the chance to solve this problem, making the solver of the next problem unpredictable. If no single entity controls a large portion of the network, the network can stay secure.

Monero uses a more accessible Proof of Work algorithm called CryptoNight, which relies on a lot of memory. ASICS, or special hardware specifically for mining, have a very low amount of memory, making it extremely difficult to mine Monero with an ASIC. Monero is committed to an accessible Proof of Work and will switch to a different, more resistance algorithm if necessary.

# What are the two basic types of mining?

The two basic types are solo mining and pool mining.

With solo mining, you are contributing the hashes, or solutions to the network problems, directly. You are directly competing with every other person on the network. If others mine a block by solving the problem, then you do not get a reward. If you mine a block, you will get all the reward. Solo mining is the best way to contribute to network decentralization, but there is large variation in payouts. Professional miners typically do not solo mine.

With pool mining, you and several other miners give your hashes to a centralized server called a pool. This pool will submit all the solutions on your behalf. If any participant in the pool solves the next block, then the rewards are distributed among all members based on the contribution of each. For instance, suppose a pool has two miners. One miner is twice as fast as the other. This faster miner would get about 2/3 of the reward from the block, while the slow miner would get about 1/3. The pool itself typically keeps a small fee of 5% or less.

# How can I solo mine?

Download Monero Core or Monero CLI. Run monerod and wait for it to synchronize with the rest of the network. This may take several hours with a fast hard drive or several days with a slow one. When synchronized, you can use the command `start_mining <address> <threads>`, replacing `<address>` and `<threads>` with your Monero address and number of threads to use. If you do not already have a Monero address, use [this guide] to create one for free. You should use the number of threads equal to ½ your CPU’s cache in MB. For instance, if your CPU has 4 cores, 8 threads, and 6MB of cache, use 3 threads when mining. Example:

`start_mining 44AFFq5kSiGBoZ4NMDwYtN18obc8AemS33DBLWs3H7otXft3XjrpDtQGv7SqSsaBYBb98uNbr2VBBEt7f2wfn3RVGQBEP3A 3`

It is technically possible to solo mine with GPUs, though it is difficult. We suggest checking the Monero StackExchange for some solutions.

# How can I pool mine?

You will need additional software to pool mine, and this will vary depending on your operating system and hardware. Several of these are listed below: (maybe you can do something fancy with JS to allow a user to select their own OS and hardware?)

- CPU

  - [XMR-STAK-CPU](https://github.com/fireice-uk/xmr-stak-cpu) open-source, dev fee

  - [Monero Spelunker](https://github.com/jwinterm/monerospelunker) open-source, forked from Wolf’s with added GUI

  - [Wolf’s CPU Miner](https://github.com/OhGodAPet/cpuminer-multi) open-source

  - [YAM miner](https://mega.co.nz/#F!h0tkXSxZ!f62uoUXogkxQmP2xO8Ib-g) proprietary, dev fee

- AMD GPU

  -	[Claymore](https://bitcointalk.org/index.php?topic=638915.0) proprietary, dev fee

  -	[Wolf’s AMD Miner](https://github.com/OhGodAPet/wolf-xmr-miner/) open-source

  -	[XMR-STAK-AMD](https://github.com/fireice-uk/xmr-stak-amd) open-source, dev fee

- NVIDIA GPU

  - [XMR-STAK-NVIDIA](https://github.com/fireice-uk/xmr-stak-nvidia) open-source, dev fee

  - [Ccminer-cryptonight](https://github.com/tsiv/ccminer-cryptonight/) open-source, dev fee

Once you have the mining software downloaded, you will need to find a pool. Community members maintain some lists of pools [here](http://moneropools.com) and [here](https://www.reddit.com/r/MoneroMining/wiki/index/monero-pools). We do not endorse any pool, though we suggest choosing one with less than 10% of the total hashrate. Mining on a large pool reduces decentralization and increases the risk of a successful attack. The pool will include instructions with how to configure your mining software.

# What about overclocking, modding BIOS, etc.?

Overclocking and modifying your BIOS can provide additional hashes if done correctly. We recommend that only experts attempt this method. Using these features may void warranties and increase the risk of fires and technical failures. We recommend reading the owner’s manual and following all manufacturers’ recommendations for their hardware. Monero and Monero pools do not assume any risk for how you configure your computer.
