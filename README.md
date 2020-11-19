# Supported Local Restaurants in Manitoba
The API will return a list of supported cities within Manitoba with their ID, name, version and the list of local restaurant (restaurant name, location). Along with that, the API can return a list of opening and closing times of restaurants with city name, city ID, restaurant name, location, and a boolean for whether or not they are open at midnight. The APIs will also return cuisine types in the city with city ID, city Name, restaurant Name, cuisine Name.

## End points
- Restaurant
  - Get/restaurant (array)
  - Get/restaurant/city (array)
- Time
  - Get/time (array)
- Cuisine 
  - Get/cuisine (array)
  
## Parameter
- Location(string)
- id(int)
- version(int)
- name(string)
- overnight (boolean)
