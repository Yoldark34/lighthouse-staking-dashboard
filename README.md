# Lighthouse staking dashboard

Made by Yoldark from Prysm lot of keys dashboard
It is not the same as the prysm's one because lighthouse do not provide the same information. I have adapted the dashboard to make it works. I upgraded the dashboard and changed a lot of things making it not a 1:1 copy of the prysm dashboard.  
Doc for the prysm dashboard : https://docs.prylabs.network/docs/prysm-usage/monitoring/grafana-dashboard/#creating-and-importing-dashboards

It is my first exported dashboard, you may need to adapt it to your usage. Feel free to open issues and provide new elements improvement.

You need cryptowat to retrieve currency price Here is the doc from prysm https://docs.prylabs.network/docs/prysm-usage/monitoring/currency-converter/  
It should run without though.  
Supports pairs: etheur,ethusd,ethgbp,ethcad,ethchf,ethjpy,ethbtc

This graph is gain and running monitoring oriented, you should use another graph if you want system monitoring oriented graphs 
<img src=preview.PNG>

# Requirement
* Grafana
* Prometheus
* Cryptowat (optionnal)
* Lighthouse "Dr. Wong" version with metrics enabled (bn et vc)  and validator monitor on bc 

# Features
* Handle lot of keys
* Display annualized %
* Support currency conversion thanks cryptowat
* Always display eth gains
* Display status of validators (was very hard to do)
* Built in alerts
* Display attestation, aggregate and proposed count per validators
* Keep tracks of daily and monthly income

# TODO
* ~Add aggregated and proposed blocks in the validator table (there is only attestation right now)~

# Issues
* ~Cpu usage can't be displayed as it is not provided~ Load avg added which should be a suitable solution.
* Process starting time is an educated guess as not provided, it should be enough
* The bottom node graph is supposed to display global balance for exited and withdrawable validators. This is not the case as lighthouse do not provide this info.
* ~Log types counter are merged, need warning and error counter~ It is because there is no error logs

eth donation : 0x945DF808617bDD3753237eCF0d5D2A8EEedE76d2  
