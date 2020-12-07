# UFOs
 
# Overview Of Project
 
In this project we created a dynamic HTML webpage which renders a table holding UFO sighting data categorized by
date, city, state, country, shape, duration, and a section for comments/descriptions. The page utilizes bootstrap and css to add aesthetic modifications and images to the page. The HTML document also utilizes the object oriented programming language JavaScript to take inputs from the page and modify/build the HTML table based on the values received from these user inputs. For this Challenge we will be adding filters for each category so that the user can filter the data from the data.js to render the HTML table according to the values for each category.
 
 
# Results
 
## Filtering the Table
We have five different input boxes  on our webpage to filter the adjacent table so that it only contains data with categories holding the same values placed in the input boxes by the user.
 
### Filters
![alt text](https://github.com/sebcampos/UFOs/blob/master/resources/input_boxes.png?raw=True)
 
If one or more values are added to any of these input boxes a javascript function will iterate over the `<li>` html object which contains the all the input fields; then collect (if any) input information placed by the user. After collecting the inputs from the user our script will iterate over the data object within our data.js file and filter the categories to only contain info related to the input fields then save this data as a new object. After which a table will be built out of the newly filtered data object. If no inputs are given the data rendered in the table will the original data content.
 
### Example
![alt text](https://github.com/sebcampos/UFOs/blob/master/resources/example.png?raw=True)
 
In the above example, we can see a user filter the table for the state "ca" and the shape "light" resulting in a table containing data where every value in the table columns state and shape are equal to "ca" and "light" respectively.
 
 
# Summary
 
## Draw Backs
- The values in the filter must match exactly with the values in our table, ie if the user was to enter "California" into the country input box nothing would be returned as "California" is not equal to "ca". No where do we specify on this page that our inputs must be exact.   
- All out data is being held in one JavaScript array within a data.js file, adding/updating a large amount of new data might prove tedious or unreasonable
- The Data on the page can not be downloaded or saved from our page in any format.
## Recommendations
- Add a way for the user to print or save the currently displayed table as a file: csv, xlsx, sql etc.
-  Create a sql database for our JavaScript script to query instead of the data.js file
- Create a Python or JavaScript script to automate adding new data to the sql file or data.js file
- Create a Python or JavaScript function to attempt to add more leniency when reading inputs. ie a function that would allow the user to input "California" and return the values for "ca".

 



