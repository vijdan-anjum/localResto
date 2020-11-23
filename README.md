# Supported Local Restaurants in Manitoba
The API will return a list of supported cities within Manitoba with their Id, name, version and the list of local restaurant (restaurant name, location). Along with that, the API can return a list of opening and closing times of restaurants with city name, restaurant name, and a boolean for whether or not they are open at midnight. The APIs will also return cuisine types in the city with their name, city it in and city code
## API documentation
Our API is a simple API, which only use get request to access the information

## End points
- City
  - city: return a list of supported countries within the local restaurants in the city
  - city/restaurant(array): return a list of local restaurants in supported city
- Time
  - time (array): access the list of open and closing time for supported restaurants. You only need to input the cities Id, restaurants name and condition if the restaurants open overnight.
- Cuisine 
  - cuisine (array): Access the list of cuisins of supported support city. You only need to input the cuisin name, city name, city ID
  
## Parameter
- Location(string): the location of restaurant. Required
- Id(int): the Id of specific city of manitoba. Required
- Id(string): the Id of city for to check for open/closing time. Required
- version(int): indicate how many copy the user want to get. Optional (the default will be 1)
- name(string): Name of city, restaurant or cuisin. Required
- overnight (boolean): indicate if the restaurant open overnight or not 

## Sample response
For City end point
```
