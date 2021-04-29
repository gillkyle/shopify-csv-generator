shopify-csv-generator
===================

A faker-based generator for Shopify sample data, forked from [@davefreiman](https://github.com/davefreiman/shopify-sample-data). Created for use with [gatsby-source-shopify](https://github.com/gatsbyjs/gatsby-source-shopify).

Images are randomly requested from [Unsplash](https://source.unsplash.com/) and are copyright the individual photographers.

## Installation

Make sure you have the Faker gem installed:

    gem install faker

Run the script with an argument specifying how many products you want. It will generate three variants per product, so if you request 20 products it will generate 60 SKUs:

    ruby faker_script.rb 20

The `shopify_data.csv` file will be generated in the project root directory. All you have to do is navigate to https://<shopifystore.com>/admin/products and find the "Import" button. Then select the generated file and boom - Your store now has dummy data.

## Examples

The [`examples` directory](./examples) includes pre-generated files for 100 and 30,000 SKUs. These are not the direct output from the script, but have been imported and then re-exported from a Shopify store. This means that all images are pre-imported and have `cdn.shopify.com` URLs.