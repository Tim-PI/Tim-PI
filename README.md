# pyredictit
=======

pyredictit is a wrapper for the public PredictIt API (https://predictit.freshdesk.com/support/solutions/articles/12000001878-does-predictit-make-market-data-available-via-an-api-).  Running this module requires mechanicalsoup and <b>Python 3.6</b>.

**this can buy or sell shares using the money currently in your account. i am not responsible for any awful (or brilliant) trades you may accidentally or purposefully make with this wrapper. don't risk more than you can afford to lose. **

Things you can do with this currently are:
- Buy or sell shares of contracts that you already own.
- Check your current balance
- Find out how much you'd make if you sold all of your shares in a market
- Find out what you would make (or lose) depending on how the contract resolves
- Summarize all of your current contracts.
- Look up & purchase shares of contracts you don't currently own

UPDATE 1/26/2017 - the number 1 question I've been getting about this is "will it steal my login and password," and the answer is *of course not*, <b>but don't take my word for it!</b> Lines 202-213 are the parts where authentication is handled specifically, and I suspect that even people who don't fully understand Python's syntax will be able to see and verify for themselves that this information isn't transmitted anywhere beyond PI's server.

INSTALLATION:

1. Go to https://www.python.org/downloads/

2. Click "Download Python 3.6.0"

3. Install it and check "Add Python to PATH"  box in setup options.

4. Open up Powershell/Terminal and type: python -m pip install mechanicalsoup

5. Clone this repo

6. Use it like a Python module!

TODO:
* stop loss and buy-at functionality
* C O M M E N T S
* UNIT TESTS
* DOC TESTS
* Check volumes and current prices
* Custom Exception classes
* setup.py script
* Adding to pip
* <s>Look up & purchase shares of contracts you don't currently own</s> - added 1/25/2017!

HOW YOU CAN HELP:

report all exceptions!  Include as much info as possible and please check to make sure that you are using valid login info and whatnot if you're copying over from the examples.  Also, *any* feedback is useful! 

WARNINGS:

I've been posting about this over on PredictIt and a few people there have informed me that this kind of stuff isn't allowed by their TOS. Frankly, because everything in the API is done the same way it would be on the site, I really doubt that they could ever figure it out - also, I've been using it to buy/sell on my account frequently and haven't been banned - but I thought I should mention that it is possible according to their TOS that this is not allowed.  I'm still going to develop it and they can send all the C&Ds they want, but I would feel pretty bad if I got someone else's account banned when they thought they were safe using something I wrote.

