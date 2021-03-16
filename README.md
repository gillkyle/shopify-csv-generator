shopify-csv-generator
===================

A Faker-inspired generator for shopify sample data, forked from [@davefreiman](https://github.com/davefreiman/shopify-sample-data) to tweak some values and defaults

## Installation

Make sure you have the Faker gem installed:

    gem install faker

Run the script with an argument specifying how many products you want:

    ruby faker_script.rb 15

The `shopify_data.csv` file will be generated in the project root directory. All you have to do is navigate to https://<shopifystore.com>/admin/products and find the "Import" button. Then select the generated file and boom - Your store now has dummy data.