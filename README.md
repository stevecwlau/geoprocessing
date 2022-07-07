# Geoprocessing with Python
The purpose of this repository is to present applications of Python in automating geoprocessing solutions.

## [1) Geocoding using the LandsD Location Search API and Python](https://github.com/stevecwlau/geoprocessing/blob/742ace2da2cda18d6e4d30c91fdfd4f8e3ee73d2/geocode_api.ipynb)
This Python script allows geocoding of large numbers of string addresses to x and y coordinate values using the [Location Search API](https://geodata.gov.hk/gs/locationSearchAPI). The existing [Geotagging tool](https://geodata.gov.hk/gt/) offers the same geocoding capability, but is limited to a hundred requests per dataset.

The script expects an input CSV file with a column that contains addresses. The default column name is “address”, but you can specify a different name in the configuration section of the script.

The script will take each address, combine it with other parameters such as district, and then 
geocode it using the Lands Department’s Location Search API. The script will then return:
- the matching x and y coordinates,
- the formatted name and address from the LandsD database
