# where did josé serrano's donors go?

From [wikipedia](https://en.wikipedia.org/wiki/José_E._Serrano)

>José Enrique Serrano (born October 24, 1943) is an American politician who has been a member of the United States House of Representatives since 1990. Serrano, a Democrat from New York, represents a district that is **one of the smallest in the country geographically, consisting of a few square miles of the heavily populated South Bronx in New York City**. His district is also one of the most densely populated and one of the few majority Hispanic districts in the country. The district was numbered the 18th from 1990 to 1993 and the 16th from 1993 to 2013; it has been the 15th district since 2013. He is currently the longest-serving Hispanic-American in the House. **He is not running for re-election in 2020 due to a diagnosis of Parkinson's disease.**

data is sourced from [fec.gov](https://www.fec.gov/data/receipts) based on receipts to the [Serrano for Congress campaign committee](https://www.fec.gov/data/committee/C00240986/)

## development

clone the repo
```sh
$ git clone git@github.com:noslouch/serrano.git
```

setup a virtual environment
```sh
$ python -m venv .venv
$ pip install -r requirements.txt
```

download a data source:
- go to: https://www.fec.gov/data/receipts/?data_type=processed&committee_id=C00240986
- click "Export" and then "Download"
- move it into the `data` directory under the name `serrano.csv`

run the jupyter notebook
```sh
$ . ./venv/bin/activate
(.venv) $ jupyter notebook serrano-donors.ipynb
```
