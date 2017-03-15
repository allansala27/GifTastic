# HW - {GifTastic}

## Live Link 
- https://allansala27.github.io/GifTastic/

## Description on how to use the app
- Click on one of the buttons on the top to load 10 gifs of that topic or input your own topic to add a button.

## Requirements
- Use the Giphy API to retrieve gifs of a specific topic
- Append new topic buttons to the end of the topics list

## Technologies Used
- Jquery for Dom Manipulation
- AJAX for API GET requests

## Code Explaination
- I first created an array of topics as instructed to.
- In a for loop, I created buttons and assigned them a data attribute corresponding to their topic.
	- Once the button is created, I used .append() to created a list of buttons at the top of the page
- Using jQuery, I created an anonymous on click function to make the AJAX call to the giphy API.
	- I stored the data attribute of the button in a variable using $(this).
	- I stored a URL template into a variable to use in the AJAX call which sets the query parameters and narrows the retreival to 10 objects.
	- I used a for loop to loop through the JSON objects retrieved in the AJAX call and display them to the HTML along with their rating i.e. suitability for different age groups.
- Using jQuery, I created an anonymous on click function to add functionality to the "Add Topic" button.
	- The button takes the value from the text input and uses that as a data attribute and text for the button.
	- I appended the button at the end of the button list at the top of the page.	
