# Dutch-Energy
It is a heavy Data set which consists of many sub-parts.It is based on Electricity and gas usage in that country. It can be solved using different approaches of machine learning and deep learning.

# Dataset link : https://www.kaggle.com/lucabasa/dutch-energy

# Context
Enexis, Liander, and Stedin are the three major network administrators of the Netherlands and, together, they provide energy to nearly the entire country. Every year, they release on their websites a table with the energy consumption of the areas under their administration.

The data are anonymized by aggregating the Zipcodes so that every entry describes at least 10 connections.

This market is not competitive, meaning that the zones are assigned. This means that every year they roughly provide energy to the same zipcodes. Small changes can happen from year to year either for a change of management or for a different aggregation of zipcodes.


# Content
Every file contains information about groups of zipcodes managed by one of the three companies for a specific year.

# Acknowledgements
All the data are taken from the following websites:

https://www.enexis.nl/over-ons/wat-bieden-we/andere-diensten/open-data
https://www.liander.nl/partners/datadiensten/open-data/data
https://www.stedin.net/zakelijk/open-data/verbruiksgegevens
Some processing was made with the code available at: https://github.com/lucabasa/kaggle_dutch_energy/blob/master/raw_data_cleaning.ipynb

The translation of the column names and descriptions was made by a non-native speaker.

# Inspiration
How are the smart meters spreading?
What is the trend of home-produced energy? (solar panel)
Can we see if there are many electric cars in a neighborhood?
What is going to be the energy consumption the next year?

# About this file
Every file is from a network administrator from a specific year.

The columns in each file are:

net_manager: code of the regional network manager
purchase_area: code of the area where the energy is purchased
street: Name of the street
zipcode_from and zipcode_to: 2 columns for the range of zipcodes covered, 4 numbers and 2 letters
city: Name of the city
num_connections: Number of connections in the range of zipcodes
delivery_perc: percentage of the net consumption of electricity or gas. The lower, the more energy was given back to the grid (for example if you have solar panels)
perc_of_active_connections: Percentage of active connections in the zipcode range
type_of_connection: principal type of connection in the zipcode range. For electricity is # fuses X # ampère. For gas is G4, G6, G10, G16, G25
type_conn_perc: percentage of presence of the principal type of connection in the zipcode range
annual_consume: Annual consume. Kwh for electricity, m3 for gas
annual_consume_lowtarif_perc: Percentage of consume during the low tarif hours. From 10 p.m. to 7 a.m. and during weekends.
smartmeter_perc: percentage of smartmeters in the zipcode ranges
