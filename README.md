munin-finance
=============

Creates Munin graphs from the data at [Yahoo! Finance](http://finance.yahoo.com/) which are extracted
via their [CSV-based API](http://download.finance.yahoo.com/) providing the last trade price data.

Note: The data is delayed depending on the stock exchange backing the symbol.

Install
-------

Clone this repository or download the finance_ file and create a
symlink as *root* in /etc/munin/plugins by using e.g.:

	cd /etc/munin/plugins; ln -s /path/to/finance_ finance_<symbol>

where <symbol> is a stock symbol known to the http://finance.yahoo.com/ API
like "FB" (Facebook) or "AAPL" (Apple). Use their search form to find the concrete
symbol names.

**Don't forget to restart your munin-node deamon.**
