# Supported Local Restaurant in Manitoba
The APIs will return the list of supported restaurant in Manitoba with their name, location, city ID, city name and the list of city with ther name, ID. The APIs also support to return a list of open and closing time of supported local restaurants with name of city, city ID, name of restaurant, location and boolean that tell if that time open overnight. Moreover, the APIs return the list of restaurant within the cuisine in the city with city ID, city Name, restaurant Name, cuisin name, version.

## End points
- Restaurant
  -  Get/ restaurant (array)
  - Get/ restaurant/city (array)
- Time
  - Get/Time (array)
- Cuisin 
  - Get/Cuisin (array)
  
## Parameter
- Location(string)
- Id(int)
- version(int)
- name(string)
- overnight (boolean)
