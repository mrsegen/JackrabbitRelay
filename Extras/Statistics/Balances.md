# JackrabbitRelay Balance Logging System

These modules record and chart the balances of all your accounts for
statistical analysis.

## Disclaimer

Please note RAPMD Crypto, LLC ("the Company"), does not provide financial
advice. The Company, and any associated companies, owners, employees,
agents or volunteers, do not hold  themselves out as Commodity Trading
Advisors (“CTAs”) or Authorized Financial Advisors  (“AFAs”). The owners,
publishers, employees and agents are not licensed under securities laws 
to address particular investment situations. No information presented
constitutes a  recommendation to buy, sell or hold any security,
financial product or instrument discussed  therein or to engage in any
specific investment strategy.

All content is for informational purposes only. The content provided
herein is not intended to replace or serve as a substitute for any
legal, tax, investment or other professional advice,  consultation or
service. It is important to do your own analysis before making any
investment  based on your own financial circumstances, investment
objectives, risk tolerance and liquidity needs.

All investments are speculative in nature and involve substantial risk of
loss. The Company does not in any way warrant or guarantee the success of
any action you take in reliance on the  statements, recommendations or
materials. The Company, owners, publishers, employees and  agents are not
liable for any losses or damages, monetary or other that may result from
the  application of information contained within any statements,
recommendations or materials.  Individuals must use their own due
diligence in analyzing featured trading indicators, other trading  tools,
webinars and other educational materials to determine if they represent
suitable and  useable features and capabilities for the individual.

Use this Software at your own risk. It is provided AS IS. The Company
accepts no responsibility or liability for losses incurred through using
this software. While The Company has gone to great lengths to test the
software, if you do find any bugs, please report them to us in the
[Jackrabbit Support Server](https://discord.gg/g93TpbV) or on Github, and
we will sort them out. Remember that risk management is your
responsibility. If you lose your account, that's entirely on you.

Past performance is not indicative of future results. Investments involve
substantial risk. Any past  results provided are intended as examples
only and are in no way a reflection of what an individual  could have
made or lost in the same situation.

## Installation and Usage

This is an automated process that runs nightly and automatically. The
only step required is to install the below line into your crontab.

You can run them more frequently then once a day, but its really not
beneficial. 

**IMPORTANT**: The order of these lines is significant and need to be as
listed for proper functionality.

```crontab
0 5 * * * /home/JackrabbitRelay/Extras/Statistics/GetExchangeBalances > /dev/null 2>&1
0 7 * * * /home/JackrabbitRelay/Extras/Statistics/ChartExchangeBalances > /dev/null 2>&1
```

## Testing

Run the below command lines. The output will be very minimal, but the
results will be in the `/home/JackrabbitRelay/Statistics/Balances` and
`/home/JackrabbitRelay/Statistics/Charts` folders.

```bash
/home/JackrabbitRelay/Extras/Statistics/GetExchangeBalances
/home/JackrabbitRelay/Extras/Statistics/ChartExchangeBalances
```

## Donations

If you would like to help support this project financially, please use
any of the below addresses. Anything donated goes to the costs of
sustaining Jackrabbit Relay. Thank you.

You can subscribe to the Jackrabbit Relay tier for recurring monthly
support:

    https://www.patreon.com/RD3277

If you perfer crypto or just a one time donation, please use any of the
below:
| | |
| :--- | :--- |
| BCH | bitcoincash:qzw5h5ccfz6v7zzh0vf5pl0eqp3zjmp5us07l72nvv|
| BTC | 3JUbL3Vsj61VBAmyHtQhyiFJcizEfxAvzV |
| ETH | 0x3c6C06150B2f24b3179a50b618aD3c0f58CF74FD |
| LINK | 0xd8Fd4fA3b489861ad6Eb95a0617B4DA7c78123F8 |
| LTC | MHj8nQcRdJWVVNeHUemSQgzBw3cPrZEtRU |
| USDT | 0xd8Fd4fA3b489861ad6Eb95a0617B4DA7c78123F8 |