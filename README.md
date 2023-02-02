# UFOs
## Overview of Project:


## Results:

### Instructions for Using the Search Function: 

To apply the filter search options on the UFO sightings table, reference the empty fields available on the left navigation panel on the page.

<img width="1289" alt="image" src="https://user-images.githubusercontent.com/114873837/216457558-bf2e07d8-0cae-4ca7-94a3-b7dc0a9e12ee.png">

Click the curser into the field of interest. Then, type the value you'd like to see within the field. Then hit the "Enter" key to apply the filter.

<img width="1495" alt="image" src="https://user-images.githubusercontent.com/114873837/216458152-31b1a6bd-0dc2-4c04-b43f-0ee53c0609bc.png">

Please note that the values for the search are case sensitive, and the value must be an exact match for what is displayed in the table. To use the example above, a search within the state of "va" will return the value(s) for Virginia-based sightings, but "VA" or "Virginia" will not.

<img width="1499" alt="image" src="https://user-images.githubusercontent.com/114873837/216458444-0a968ed0-6090-45bc-bc96-e7a471a35677.png">

Similarly, date formats must be typed in M/D/YYYY format without leading zeros for months or dates. Values matching "1/1/2010" will appear, but "1/01/2010" will not.

<img width="1484" alt="image" src="https://user-images.githubusercontent.com/114873837/216458978-e2fa2c20-c223-466c-82e8-ede94c8e24d9.png">

<img width="1497" alt="image" src="https://user-images.githubusercontent.com/114873837/216459125-ea2a4fc4-adf7-4c06-8e67-882f13b9b5a7.png">

To get more specific with the search criteria, two or more of the filter fields can be filled with reference values. 

<img width="1484" alt="image" src="https://user-images.githubusercontent.com/114873837/216459492-b6fc2a3e-2c1e-4f38-8e14-2714ccc68877.png">

Using multiple search filters is also helpful when trying to examine general trends by type, such as "all unusual light observations in the US".

<img width="1404" alt="image" src="https://user-images.githubusercontent.com/114873837/216459965-92ef4a32-2a12-41d4-af2c-e244fa4f4184.png">

To remove the filters on the table to restore the entire table to the display, delete the values from the filter boxes and hit the "Enter" key. The original table will reset.

## Summary: 
### Drawbacks to design

As described in the instructions, the user must be very exact in their capitalization, spacing, and formatting when entering the data values in order for the filters to recognize the results. They likely would need to review the complete table before applying any filters in order to make sure they are matching the value as written - which defeats the point of a quick search tool!

### Recommendations:

To improve utility of the search function, I would recommend the following changes to the model:
1. To resolve this issue of specificity, 
2. To improve the user's ability to identify trends in the data, it would be helpful to standardize the "Duration" column to a consistent format. For example, if one value reads as "15 minutes", another as "15 mins.", and another as "about 15 minutes", this makes it difficult to recognize the values as the same duration. If all durations were stored in reference to a traditional hh:mm:ss format (for example, 1:00, :15, :30), it could make it easier for a user to quickly locate sightings of, say, 30 seconds or longer in a given location. Towards this goal, I would also recommend the ability to include ranges for numerical values in the table, such as Duration (which should also be added to the html as a filter option for analytical purposes) or Date of the sighting. A user may want to know sightings that occurred on the exact day of 1/1/2010, but they could gather more meaningful data on trends if they could observe sightings data for the entire month of January, the first quarter of 2010, etc.
