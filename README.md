## Getting started

The dependencies for the project can be installed using

    $ pip install -r requirements.txt

To initialize the database you need to download the data

    $ wget https://s3.amazonaws.com/open_data/csv/opendata_projects.zip && unzip opendata_projects.zip

and import it

    $ mongoimport -d donorschoose -c projects --type csv --file /vagrant/opendata_projects.csv -headerline
