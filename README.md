# Supported Local Restaurants in Manitoba
The API will return a list of supported cities within Manitoba with their Id, name, version and the list of local restaurant (restaurant name, location). Along with that, the API can return a list of opening and closing times of supported restaurant with city name, restaurant name, and a boolean for whether or not they are open at midnight. The APIs will also return list of supported restaurants within the cuisin type and the city it in.
## API documentation
Our API is a simple API, which only use get request to access the information. You can request at
```
https://app.swaggerhub.com/apis/emily96/API_resto/1.0.0
```

## End points and parameter
The API will have 3 endpoints, and the information is about the 3 endpoints within their parameters
### City
- **city**: return a list of supported countries within the local restaurants in the city
  - **parameter**
    - Id (int): Id of city. Required.
    - Name(string): Name of city. Required
    - restaurant(array) : return a list of local restaurants in supported city. Required
    - verson(int): indicate how many copy the user want to get. Optional
- **city/restaurant** : return a list of local restaurants in supported city
  - **parameter**
    - Name(string): Name of restaurant
    - Location(string): Location of restaurant

### Time
  - **time**: access the list of open and closing time for supported restaurants. You only need to input the cities Id, restaurants name and condition if the restaurants open overnight.
  - **parameter**
    - Id (string): Id of city with specific time type. Required
    > For example: "Id":"Winnipeg, Manitoba, Standard Time"
    - Name (string): Name of the restaurant. Required
    - support_overnight(boolean): boolean to check if the restaurant will be open overnight. Optional

### Cuisine
  - **cuisine**: Access the list of cuisins of supported support city. You only need to input the cuisin name, city ID, version. Required
  - **parameter**
    - Id (int): the id of the city. Required
    - Name (string): the name of the cuisin want to search. Required
    - version (int): indicate how many copy should it return. Required

## Sample requests
### Sample request direct from browser
The example below is the sample request directly from the brower when user want to check open and closing time of restaurant
```
http://swaggerhub.com/apis/emily96/API_resto/1.0.0#/Time/json?id=Winnipeg,Manitoba,StandardTime&name=KingHeadPub&support_overnight=false
http://swaggerhub.com/apis/emily96/API_resto/1.0.0#/Time/json?id=Winnipeg,Manitoba,StandardTime&name=KingHeadPub
```


### Sample request in JSON file
The example below is the sample request in JSON when the user want to check open and closing time of restaurant in Winnipeg
```
[
  {
    "Id": "Winnipeg, Manitoba Standard Time",
    "Name": "King Head Pub",
    "support_overnight": "false"
  }
]
```

## Sample response
The example below is the respose in JSON when user want to check open and closing time of restaurant in winnipeg
```
{
  "result":
  {
    "open"      : "11:00 AM",
    "closing"   : "9:00 PM",
  }
  "responses": "200"
}
```
## Response code
The "response" in the API will contain the response description of the resquest. Their are 2 values response message from the API
- "200": Sucessful operation
- "400": Invalid input

## Authors
* Emily Nguyen
* Charina Duenas
* Rajinder Singh
* Anjum Mohammed
