# Exploring the Enforcement of Cookie Banners across Continents: An Empirical Study

The directory `./crawler` contains details concerning our crawler and the cookie consent banner detection code and how to run it. 

Use `./crawler/demo.py` to run the crawler, but ensure the the following are in order:
1 - the right Firefox profile, we use different Firefox profiles: 
  . `accept` - `./data/cookie-accept`
  . `no interaction` - `./data/cookie-reject`

Ensure to set the right profile (here)[https://github.com/intumwa/cookie-prevalence/blob/929238c6326b4e9c41666ab0a96df2f2886faad5/crawler/openwpm/deploy_browsers/deploy_firefox.py#L146C80-L146C80]: 

For acceptance: `driver.install_addon('/path/to/extension/idcac.xpi')`
For rejection: `driver.install_addon('/path/to/extension/consent_o_matic.xpi')`

`./data/websites.txt` is the list of domains that we have repeatedly crawled, each 6 times from five countries.

When everything is ready, run the cookie consent banner detector at `./crawler/popup.py`

## Below is a summary of the results of our experimentation
