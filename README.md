# Capstone Project - The Battle of Neighborhoods
[TOC]
## Section 1: Introduction
    In this section I will clearly define the idea of my choosing, where I leverage the Foursquare location data to solve the imagined business opportunity.
### Business Problem
    As an Asian who is planning to move to Toronto from another city, how can I find the most Asian-friendly neighborhoods to settle down in Toronto?

### Interest
    Asians who are planning to move to Toronto but are not familiar with Toronto.

## Section 2: Data
### Get Postcode, Borough and Neighborhood information of Toronto from Wikipedia
requests.get('https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M')

        Postcode   Borough          Neighborhood
    0   M3A        North York       Parkwoods
    1   M4A        North York       Victoria Village
    2   M5A        Downtown Toronto Harbourfront , Regent Park
    3   M6A        North York       Lawrence Manor, Lawrence Heights
    4   M7A        Queen's Park     Queen's Park
    5   M9A        Etobicoke        Islington Avenue
    6   M1B        Scarborough      Malvern, Rouge
    7   M3B        North York       Don Mills North
    8   M4B        East York        Woodbine Gardens, Parkview Hill
    9   M5B        Downtown Toronto Ryerson, Garden District
### Add Geo-spatial data
        Postcode    Borough           Neighborhood                      Latitude    Longitude
    0   M3A         North York        Parkwoods	                        43.753259   -79.329656
    1   M4A         North York        Victoria Village                  43.725882   -79.315572
    2   M5A         Downtown Toronto  Harbourfront , Regent Park        43.654260   -79.360636
    3   M6A         North York        Lawrence Manor, Lawrence Heights  43.718518   -79.464763
    4   M7A         Queen's Park      Queen's Park                      43.662301   -79.389494
    5   M9A         Etobicoke         Islington Avenue                  43.667856   -79.532242
    6   M1B         Scarborough       Malvern, Rouge                    43.806686   -79.194353
    7   M3B         North York        Don Mills North                   43.745906   -79.352188
    8   M4B         East York         Woodbine Gardens, Parkview Hill   43.706397   -79.309937
    9   M5B         Downtown Toronto  Ryerson, Garden District          43.657162   -79.378937
### Get venues information of Toronto from FourSquare

        Neighborhood        Neighborhood Latitude   Neighborhood Longitude  Venue                   Venue Latitude  Venue Longitude Venue Category
    0   Parkwoods           43.753259               -79.329656              Brookbanks Park         43.751976       -79.332140      Park
    1   Parkwoods           43.753259               -79.329656              PetSmart                43.748639       -79.333488      Pet Store
    2   Parkwoods           43.753259               -79.329656              KFC                     43.754387       -79.333021      Fast Food Restaurant
    3   Parkwoods           43.753259               -79.329656              Variety Store           43.751974       -79.333114      Food & Drink Shop
    4   Parkwoods           43.753259               -79.329656              Ranchdale Park          43.751388       -79.322138      Park
    5   Parkwoods           43.753259               -79.329656              Joey                    43.753441       -79.321640      Burger Joint
    6   Parkwoods           43.753259               -79.329656              Three Valleys Park      43.751195       -79.337356      Park
    7   Victoria Village    43.725882               -79.315572              Victoria Village Arena  43.723481       -79.315635      Hockey Arena
    8   Victoria Village    43.725882               -79.315572              Tim Hortons             43.725517       -79.313103      Coffee Shop
    9   Victoria Village    43.725882               -79.315572              Portugril               43.725819       -79.312785      Portuguese Restaurant





