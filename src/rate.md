# > $ curl rate.sx

![Example](img/rate-thumbnail.png =600x)

## Description
A really cool tool for tracking cryptocurrency exchange rates, conversions, historical data updating every 5 minutes.

## Usage
Represent the values in currency other than dollars(Euro in this case):

```
curl eur.rate.sx
```

Customise the timespan and the currency:

```
curl rate.sx/eth@30d                # Ethereum to USD rate for the last 30 days
curl eur.rate.sx/btc@february       # How Bitcoin (BTC) price in EUR changed in February
```

Convert currencies:

```
curl eur.rate.sx/1BTC+1BCH+1BTG       # convert sum of the Bitcoins (BTC, BCH and BTG) into Euro (EUR)
curl rub.rate.sx/100ETH               # convert 100 ETH into Russian ruble (RUB)
```

I strongly suggest checking the [Github](https://github.com/chubin/rate.sx) page fo the project to fully explore the features it provides. 

## Tips
I tried to put it in a watch command but it seems to have a lot of issues with the special characters. So here a one-liner 
that will update the graph every 60 seconds until you press CTRL+C. You can easily customise the curl command and "watch" whatever graph you want.

```
while true; do curl -s rate.sx; sleep 60; done
```

## Links
- [Github](https://github.com/chubin/rate.sx)