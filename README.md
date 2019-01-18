# Trading-Algorithms

Over the past 15+ years, I have written dozens of algorithmic trading strategies for both myself and a few clients.  Thus far, I have only used a trading platform called TradeStation.  TradeStation utilizes its' own native language (EasyLanguage) to code these tools.

I coded my primary system as a collection of 25 "virtual" strategies running only in the background.  At the end of each user-defined interval, each virtual system is evaluated on its' performace and ranked in relation to the performance of the other 24 virtual strategies over the same interval.  Then, the best performing virtual strategy is selected to execute real trades during the next interval.  This system of virtual strategy selection and switching is known as "walking forward in the backtest", and could also be described as automated variable optimization.  

I have coded many proprietary calculations and features into this system.  To name a few:
- "mirroring" -- entering and exiting trades exactly opposite to what the normal system has calculated
- "agreeing"  -- only entering trades when multiple virtual strategies agree on a given entry point
- "dynamic momentum" -- automatically updating momentum settings based on market patterns
- "anchored momentum" -- updating momentum continuously based on 2-dimensional 'distance' from an anchor point
- "momentum derivatives" -- utilizing rates of change of momentum, i.e. momentum is increasing at an increasing or decreasing rate

In addition, I have developed many more features and conditions to filter trades.

In conclusion, I have developed my system based on the theory that most of the time the market has a tendency to balance itself out, and my goal is to identify and exploit market imbalances.

