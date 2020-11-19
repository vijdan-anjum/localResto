# Supported Local Restaurant in Manitoba
The APIs will return a list of supported cities within Manitoba with their ID, name, version and the list of local restaurant (restaurant name, location). Along with that, the API can return a list of opening and closing times of restaurants with city name, city ID, restaurant name, location, and a boolean for whether or not they are open at midnight. The APIs will also return cuisine types in the city with city ID, city Name, restaurant Name, cuisine name.

## End points
- City
  -  Get/ City (array)
  - Get/ City/Restaurant (array)
- Time
  - Get/Time (array)
- Cuisine 
  - Get/Cuisine (array)
  
## Parameter
- Location(string)
- Id(int)
- version(int)
- name(string)
- overnight (boolean)
