# Countries_world_map
![Example](https://simplewidgets.dev/wp-content/uploads/2021/07/countries_world_map.png)

Online example is available at [example.simplewidgets.dev](https://examples.simplewidgets.dev "World Map Example | simplewidgets.dev")

This package provides an easy to implement World Map (or any other country of choice) which is fully customizable. It started with only a simple world map but the goal is to create a customizable map for each country.
In this case "customizable" means the ability to change the color of a country/ state.

## About this package
This flutter package draws a map of choice using the CustomPainter. These maps can be quite big so please read "Perfomance" below.


### Available maps
| World Maps | Continents | Countries |
|--|--|--|
| <ul><li>[ ] Normal World Map </li><li>[x] Simple World Map</li> <li>[ ] Geo World Map</li></ul> | <ul><li>[ ] Africa </li><li>[ ] Asia </li> <li>[ ] Australia/Oceania </li> <li>[ ] Europe </li> <li>[ ] Middle East </li> <li>[ ] North America </li> <li>[ ] South America </li></ul> | <ul><li>[x] Netherlands </li></ul> |




### WorldMapPainter
If the WorldMap widget does not give the results you would like to see, you can also use the WorldMapPainter in your own defined CustomPainter. This will give you all the paths with the option to custom color each country.


## Tips for UI
1. Wrap the WorldMap in an InteractiveViewer widget to zoom in and out on specific countries as done in the [online example](https://examples.simplewidgets.dev "World Map Example | simplewidgets.dev"). In the example the InteractiveViewer has a maxScale of 75.
2. Set the WorldMap to 92% of the available width to make it look more centered.



## Memory usage
The map is big, so (re)building the widget can be expensive. That's why the WorldMap uses a RepaintBoundry to prevent it from unnecessary repaints. If you change a Country Color and call SetState() the widget will repaint.

#### ! Warning
On the iPad Pro 2018 there has been found some memory issues when re-painting the World Map many times in a short time period. If you have memory issues, you might want to limit the possible repaints.


## Like to contribute?
Feel free to help us improve this package by creating issues, pull request etc. Together we can make a great map for data visualization and other use cases. For any questions you can email hello@simplewidgets.dev


