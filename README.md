# Bank_of_Tz

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

Bank_of_Tz is a web scrapper which scapes data from bot.go.tz the data its scapes includes

  - Treasury Bill Prices from previous Actions (available in JSON)
  - Treasury Bond Prices from previous Actions
  - Currency Rates 
 
### Installation
Using pip

```$
$ pip install Bank_of_Tz --upgrade
```
or for Those with both python2 and python3
```$
$ pip3 install Bank_of_Tz --upgrade
```

using Git and pip

```sh
$ pip install git+https://github.com/Mbonea-Mjema/Bank-of-Tz.git
```
### Examples

- Get rates
```python
import Bank_of_Tz as B
obj=B.Bank_of_Tz()
data=obj.get_rates()
'''output >>{'USD': ['225,505.94', '227,761.00'], 'Euro': ['262,331.06', '264,999.92'], 'GBP': ['295,954.00', '298,959.09'], 'KES': ['2,240.50', '2,258.41'], 'ZAR': ['16,330.83', '16,487.34']} '''
```

- Get Treasury Bond Prices
```python
import Bank_of_Tz as B
obj=B.Bank_of_Tz()
data=obj.get_All_bond_prices('15') # requires one argument (Number of Years)
```
- Get Treasury Bill Prices 
```python
import Bank_of_Tz as B
obj=B.Bank_of_Tz()
data=obj.get_All_bond_prices('1') # requires one argument (Number of results)
```

### Todos

 - Price Predictions
 - Add graphs

License
----

MIT



[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
