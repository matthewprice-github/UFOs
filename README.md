# UFOs

## Overview 
The purpose of the analysis was to provide a comprehensive database of UFO sightings on a webpage that users could not only read but interact with themselves. Using Javascript, we can create dynamic tables that can be filtered by users based on multiple criteria.

## Results 
Depending on what the end user is interested in, they can input filters on the side bar, which will then be interpreted using a script and applied to the table on the right. For exmple, say a user remembered there was a famous UFO sighting in El Cajon on Jan 1st, 2010. They simply can input "1/1/2010" and "el cajon" in the filter fields and will be able to see there were [multiple recorded sightings](https://github.com/matthewprice-github/UFOs/blob/main/static/images/Table_screenshot.PNG) in El Cajon on that day, and all of them remark on the "three red lights" seen in the sky. A user can probably infer that all of the sightings are probably witnessing on the same UFO! 

## Summary 
This interactive table will be extremely useful for users who might want specific UFO information surround a city, country, UFO shape, time period, or some combination of the four. One drawback of this design is that the script will run whenever a user changes a single input field. Usually this is not an issue, but when a user wants to filter for multiple criteria, the script will render a new table for each new input they add. This is inefficient for the program, which could simply wait until the user has finished inputting all of their desired filters, and rendering a filtered table once. One solution could be to change the UI of the html file and create a "filter" button which the user would press when they have completed all of their inputs. This way, we can tie the event trigger to the button click, instead of having to detect a change to each input field, which would cause the updatefilters() function to fun prematurely. 
