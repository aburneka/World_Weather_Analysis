# World Weather Analysis

## Project Overview 

For this project we have created an app, PlanMyTrip. The app helps travelers pick cities where they would like to visit based on weather data. The app asks for temperature ranges and then gathers any city, as well as hotel information, that falls within the applicable range. 

From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, we have created a travel route between the four cities as well as a marker layer map. 

## Resources

Data Source: Open Weather Map API, Google Maps API, WeatherPy_database.csv, WeatherPy_vacation.csv

Software: Python 3.7.6, Jupyter Notebook, Matplotlib, Numpy, Pandas, Citipy,


## PlanMyTip App Output 

Using Open Weather Map's API we attributed the current weather of the cities found by the citipy module and placed the data in a dataframe and exported to a csv file.

After the dataframe was created we then imported the csv file and then isolated the cities that fell within the users temperature range after they completed the input statements. In this example we used a temperature range of 65 - 85 degrees farenheit. 

Using the Google Maps API we then pulled in the closest hotel within 5000m of the longitude and latitude coordinates for cities that fall within the temperature range. Using the gmaps module we plotted the cities with hotels in the temperature range on a map. See the example below: 

<img width="989" alt="World Map Vacation Search" src="https://user-images.githubusercontent.com/79999761/116018475-ef48de00-a5f6-11eb-99c2-c7199d42ce1a.png">


### Mock Travel Itinerary 

The last step in this project was to pick four cities that fall into the temperature data range that are in somewhat close proximity to one another as the options for travel were limited to walking, driving and biking.  Using Gmaps directions layer we plotted driving directions to create a round trip itinerary to the four identified cities: 
<img width="784" alt="Cities" src="https://user-images.githubusercontent.com/79999761/116018787-a47b9600-a5f7-11eb-933c-97db1d481473.png">

Driving Route: <img width="981" alt="Driving Route" src="https://user-images.githubusercontent.com/79999761/116018831-b9582980-a5f7-11eb-90d9-9aadd5aaf7f1.png">

Chosen Cities with Information: 
<img width="988" alt="Cities with Markers" src="https://user-images.githubusercontent.com/79999761/116018881-d8ef5200-a5f7-11eb-94fc-4828cae34a5b.png">


