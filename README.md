# UFOs - The table is out there

# Overview
The purpose of this application is display information from Dana's js file of UFO sighting data as a table in a webpage.  Moreover, the quantity of data necessitates that we make the results table filterable by any one or more of five criteria from the data file.  We will add a navbar, jumbotron, and a row with article title, subtile and content above the filter list and table.


# How to Guide
### Load the Page
Begin by loading the <a href="index.html">index.html<a/> page.  This will display the main page and application.  You will find the list of filters in the lower left corner of the page and the table of data immediately to the right.  Example searches for each filter appear as grey text. Initially the table will be unfiltered, displaying every record in the data set, as seen below:<br> 
![Unfiltered Table](/Static/images/table_unfiltered.png)<br> 

### Filter the Results
Searching the data is simple, just type a search term in the corresponding box.  To perform the search and refresh the table, press `Enter` or simply exit the box by clicking or tabbing out.  This will display all results matching your search.  The search is a simple `AND` search, meaning that the results will comprise the records that match all of the specified criteria.  In the example below, two filters are used to show only the sightings which occurred on 1/11/2010 in fl.<br>
![Filtered Table](/Static/images/table_filtered.png)<br>

### Refresh the Page
To clear all existing filters, you can refresh the page, manually clear the search terms or click the `UFO Sightings` button at the top left, in the navbar.
![Page Refresh](/Static/images/refresh.png)<br>
 
# Summary and Next Steps
This tool does serviceable work, delivering relevant results to a user's query.  However it is somewhat limited and one of the most glaring issues is the want of a record count.  It is rather difficult to determine the number or results in a search or even the relative size of two different searches.  The size of each row varies with the length of the comments field, compounding the problem.  

### Future Development
- In addition to the matching record count, we could add a count of results by group using one of the filters.  For example if the table is filtered by state, we could display a count of the results grouped by date or shape.

- It may prove helpful to the user if the date field were searchable for a period of time in addition to what is currently a single data.  This could be accomplished by first adding an endDate field to the filter list and then filtering the data for a range from the original date field to the endDate field.

- Providing the user with the ability to create bar line graphs with the filtered data would be a powerful feature.  A quick glance at the table suggests that sightings spike on Jan 1st, but a line or bar graph clearly show the magnitude of the spike.
  
# Tools used
- js
- html
- bootstrap
- d3