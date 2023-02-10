# RTrade
*API Wrapper for Roblox Trading*

⚠️ **STILL IN DEVELOPEMENT** (Updates to follow)

**RTrade** is the successor of <a href="https://github.com/wa1ker38552/RoTrade-PY">RoTrade.py</a> which is a poorly written library from a long time ago. I kinda gave up on that project and decided to restart its entire development as RTrade. Hopefully RTrade will be used as a library to aid learning developers trying to create a trade bot. Since most trade bots on Roblox either 1. don't work, 2. are just token loggers, or 3. impossible to get as you have to be whitelisted. 

**Quick Example**
```py
import rtrade

client = rtrade.client('cookie')

@client.on_ready()
def on_ready():
  print(client.user.id)

@client.on_trade_recieved()
def on_trade_received(trade):
  print(f'New inbound trade: {trade.id}')

client.run()
```
