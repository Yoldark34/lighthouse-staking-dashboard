# Lighthouse staking dashboard

Made by Yoldark from Prysm lot of keys dashboard
It is not the same as the prysm's one because lighthouse do not provide the same informations. I have adapted the dashboard to meke it works. I upgraded the dashboard and changed a lot of things making it not a 1:1 copy of the prysm dashboard.
Doc for the prysm dashboaard : https://docs.prylabs.network/docs/prysm-usage/monitoring/grafana-dashboard/#creating-and-importing-dashboards

It is my first exported dashbord, you may need to adapt it to your usage. Feel free to open issues and provide new elements improvment.

You need cryptowat to retrieve currency price Here is the tuto from prysm https://docs.prylabs.network/docs/prysm-usage/monitoring/currency-converter/  
It should run without though.  
Supports pairs: etheur,ethusd,ethgbp,ethcad,ethchf,ethjpy,ethbtc

# Features
* Handle lot of keys
* Display anualized %
* Support currency convertion thanks cryptowat
* Alway display eth gains
* Display status of validators (was very hard to do)
* Built in alerts

# Issues
* Cpu usage can't be displayed as it is not provided
* Process starting time is an educated guess as not provided, it should be enough
* The bottom node graph is supposed to display global balance for exited and withdrawable validators. This is not the case as lighthouse do not provide this info.

eth donation : 0x945DF808617bDD3753237eCF0d5D2A8EEedE76d2  
