CORONA@HOME (CORO) integration/staging repository
======================================

CORONA@HOME is a cutting edge cryptocurrency, with many features not available in most other cryptocurrencies.
- 100% Proof of Stake 3.0 Consensus protocol, allowing very low transaction fees and energy expenditure, and staking rewards to all participants in the network.
- Masternode technology used to secure the network and provide additional features. Each Masternode is secured with collateral of 1000 CORO.
- Decentralized blockchain voting utilizing Masternode technology. The blockchain will distribute monthly treasury funds based on successful proposals submitted by the community and voted on by the Masternodes.


Quick installation of the CORONA@HOME daemon under linux.

Installation of libraries (using root user):

    add-apt-repository ppa:bitcoin/bitcoin -y
    apt-get update
    apt-get install -y build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
    apt-get install -y libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    apt-get install -y libdb4.8-dev libdb4.8++-dev

Cloning the repository and compiling (use any user with the sudo group):

    cd
    git clone https://github.com/Coronahome/CORO.git
    cd CORO
    ./autogen.sh
    ./configure
    sudo make install
    cd src
    sudo strip coronaathomed
    sudo strip coronaathome-cli
    sudo strip coronaathome-tx
    cd ..

Running the daemon:

    coronaathomed 

Stopping the daemon:

    coronaathome-cli stop

Demon status:

    coronaathome-cli getinfo
    coronaathome-cli mnsync status



## Coin Specs ##
<table>
<tr><td>Algo</td><td>Quark</td></tr>
<tr><td>Block Time</td><td>60 Seconds</td></tr>
<tr><td>Difficulty Retargeting</td><td>Every Block</td></tr>
<tr><td>Max Coin Supply</td><td>8,888,888 CORO</td></tr>
</table>

## PoS Rewards Breakdown ##

<table>
<th>Block Height</th><th>Reward</th><th>Masternodes</th><th>Stakers</th>
<tr><td>< 172,800</td><td>0.1 CORO</td><td>0.08 CORO</td><td>0.02 CORO</td></tr>
<tr><td>172,800-345,600</td><td>0.12 CORO</td><td>0.096 CORO</td><td>0.024 CORO</td></tr>
<tr><td>345,600-518,400</td><td>0.14 CORO</td><td>0.112 CORO</td><td>0.028 CORO</td></tr>
<tr><td>518,400-691,200</td><td>0.16 CORO</td><td>0.128 CORO</td><td>0.032 CORO</td></tr>
<tr><td>691,200-864,000</td><td>0.18 CORO</td><td>0.144 CORO</td><td>0.036 CORO</td></tr>
<tr><td>864,000-1,036,800</td><td>0.20 CORO</td><td>0.16 CORO</td><td>0.04 CORO</td></tr>
<tr><td>1,036,800-1,209,600</td><td>0.22 CORO</td><td>0.176 CORO</td><td>0.044 CORO</td></tr>
<tr><td>1,209,600-1,382,400</td><td>0.24 CORO</td><td>0.192 CORO</td><td>0.048 CORO</td></tr>
<tr><td>1,382,400-1,555,200</td><td>0.25 CORO</td><td>0.2 CORO</td><td>0.05 CORO</td></tr>
<tr><td>1,555,200-1,814,400</td><td>0.28 CORO</td><td>0.224 CORO</td><td>0.056 CORO</td></tr>
<tr><td>1,814,400-2,073,600</td><td>0.32 CORO</td><td>0.256 CORO</td><td>0.064 CORO</td></tr>
<tr><td>2,073,600-2,332,800</td><td>0.38 CORO</td><td>0.304 CORO</td><td>0.076 CORO</td></tr>
<tr><td>2,332,800-2,592,000</td><td>0.48 CORO</td><td>0.384 CORO</td><td>0.096 CORO</td></tr>
<tr><td>2,592,000-3,110,400</td><td>0.60 CORO</td><td>0.48 CORO</td><td>0.12 CORO</td></tr>
<tr><td>3,110,400-3,628,800</td><td>0.76 CORO</td><td>0.608 CORO</td><td>0.152 CORO</td></tr>
<tr><td>3,628,800-4,147,200</td><td>1 CORO</td><td>0.8 CORO</td><td>0.2 CORO</td></tr>
<tr><td>4,147,200+</td><td>0.8 CORO</td><td>0.64 CORO</td><td>0.16 CORO</td></tr>

</table>

There is NO budget as development, governance, owner or any other hidden budget. 
All genareted CORO rewards are transparent split among mastrernodes and stakers.


More information at [CORONA@HOME](https://coronahome.org/)

