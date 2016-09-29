# Rails Elasticsearch Autocomplete

[Frontend: Elasticsearch Angular Autocomplete](https://github.com/EricLondon/Elasticsearch-Angular-Autocomplete)

Setup:
```

# install/run elasticsearch
brew install elasticsearch
brew services start elasticsearch

# checkout project
git clone git@github.com:EricLondon/Rails-Elasticsearch-Autocomplete.git
cd Rails-Elasticsearch-Autocomplete

# install gems
bundle install

# setup database
rake db:create && rake db:migrate

# create elasticsearch index via rails console
rails c
> Person.__elasticsearch__.create_index! force: true

# create sample data
rake import:people

```
