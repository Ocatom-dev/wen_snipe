
# Table of contents
* [Important Notes](#IMPORTANT-NOTES-BEFORE-RUNNING-THE-BOT)
* [New Update](#NEW-UPDATES)
* [Advanced Bot](#NOW-LAUNCH-ADVANCED-BOT)
* [Setup](#HOW-TO-RUN)
* [TroubleShoot](#TROUBLESHOOT)

## NEW UPDATES
1. In this new update you can use BNB instead WBNB. it will make you easier to snipe :)


## HOW TO RUN
1. Open your terminal/command prompt
2. clone this repository by typing <code> git clone https://github.com/Ocatom-dev/wen_snipe </code>
3. Navigate to your wen_snipe folder
4. Type <code>npm install</code> and wait for it to finish installing
5. copy your <code>.env.example</code> to <code>.env</code> or simply rename your <code>.env.example</code> file to <code>.env</code>
6. set up your <code>.env</code> to with this explanation : 

```
WBNB_CONTRACT=0xbb4cdb9cbd36b01bd1cbaebf2de08d9173bc095c
~ WBNB contract for buy the token

FACTORY=0xcA143Ce32Fe78f1f7019d7d551a6402fC5350c73
~ Pancake Factory contract to get function of buy

ROUTER=0x10ED43C718714eb63d5aA57B78B54704E256024E
~ Pancake Factory contract to process function of buy

YOUR_ADDRESS=
~ Your BSC (BEP20) address from trustwallet or another wallet.

SLIPPAGE=1
~ Customize your slippage here, cannot decimal. (eg : 1, 5, 10). if you buy early token recommended 30+ Slippage

GWEI=5
~ Customize your GWEI (gas fee) here, cannot decimal. (eg : 5, 10, 25). if you buy early token recommended 15+ GWEI

GAS_LIMIT=345684
~ Minimul limit is 210000, more much more better.

MIN_LIQUIDITY_ADDED=3
~ Set how much minimum liquidity added in pair address that you want to buy. set in BNB. (eg : 2, 4, 7).
  2 mean 2 BNB liquidity added.

YOUR_MNEMONIC=
~ Input your private Key here, that you get from your wallet privacy.

AMOUNT_OF_WBNB=0.002
~ Amount how much you want buy the token in WBNB.

TO_PURCHASE=0xe9e7cea3dedca5984780bafc599bd69add087d56
~ Token address that you want to buy.


```

6. run with <code>npm run snipe </code>.

7. Wait the bot do his job, if success, you will see like this picture. <br>
   <img src="./assets/botimg.PNG">
   
8. Close bot with <code>ctrl + C</code>.

## WARNING
All this bot feature are free, I'm never sell this bot, and I'm never share my TG account. Please be careful and DWYOR!. Only this bot is free, not advanced bot.

## TROUBLESHOOT
* some possible reasons for failed tx:
- you haven't approved your WBNB
- your gas price is too small
- your GWEI is too small (use 15+ for early token)
- your slippage is too small (use 30+ for early token)

* Error with node :
  
 <img src="./assets/wss-error.png"

 You can use provided node <code>wss://bsc-ws-node.nariox.org:443</code>  or you can use a private node or build your own node. It's faster than public node.
Recommended node providers for private node : 
  1. https://getblock.io/en/
  2. https://www.quicknode.com/
  3. https://www.ankr.com/ <br>
   
