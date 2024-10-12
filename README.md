python-restcountries is a simple Python wrapper for the REST Countries API. It allows users to retrieve country data by name or other filters, and provides access to various country attributes such as name, capital, currencies, population, and more.
Installation:

To install:

shell

pip install python-restcountries

Usage:

To use the API wrapper:

python

from restcountries import RestCountryApiV2 as rapi
country_list = rapi.get_countries_by_name('France')

Response Filtering:

Filters can be applied to limit the data returned. For example:

python

country_list = rapi.get_countries_by_name("France", filters=["name","currencies","capital"])

Available Attributes:

Attributes include name, currencies, capital, languages, region, population, flag, and many more.
Country Object:

The API returns a Country object or a list of Country objects, which provides access to all relevant country details like name, capital, area, etc.

This wrapper simplifies interactions with the REST Countries API, offering flexibility with filtering and detailed access to country information.
