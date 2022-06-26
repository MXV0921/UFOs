# UFOs
## An Excercise in Utilizing JavaScript, Bootstrap and CSS

## Purpose of the Project
This project we were given a JavaScript file with an array of dictionaries that contained information of "UFO sightings".  We created an app file in Java that would help us to filter this data in a user interface HTML file.

## Results of Project

![webpage](webpage_image_address)

This is our final webpage, it contains a working javascript table that has multiple filters such as date, state, and country.  Once published our page will be a user friendly site to sort through all of this information.

We created the table using the following code:

![create_table_image](githubaddress_create_table)

By utilizing a module called 'D3' we are able to write code in our app.js file that builds visual tables on our html page.  The following block of code references the line in the html where the table will be placed("td" abbreviates 'table data':

```    Object.values(dataRow).forEach((val) => {
      let cell = row.append("td");
      cell.text(val);
    });
  });
}
```

We used our app.js file to create filters in the following code block:

![filter_table_image](github_filter_table)

When a user enters a filter in any of these boxes, the table will accordingly filter on the users request.  Here is an example of the table being filtered to show only sightings that took place in ca(California):

![filter_table_california](github_california_filter)


## Summary of Project

This project is very useful in creating a basic filter for data.  There is so much more that we would be able to do make this professional and more user friendly:
1. We need to perform further data cleaning on the duration column of our table.  To make this more usable, there needs to be a clear and consisent format for the duration of the events.  This will make a filter easier to use, rather than having the data as strings vs a number.
2. The formatting of the locations should also be adjusted.  With addtional lines of code we can automatically capitalize the states and countries that the events happened.  As an additional plus, we can write lines of code in the filter to allow the user to enter either lowercase or uppercase letters when sorting.  Currently the filter does not work if capitalization does not match.
3. A third solve for the capitalization issue would be to write code that would change the filter box to a drop down menu.  This dropdown box would allow users to sort by only items contained in the table. 
