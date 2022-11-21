# Latitude vs X

This project brings a comparison of the data extracted about cities located across the globe, taking into consideration the following information:
* Max Temperature
* Humidity
* Cloudiness
* Wind Speed

Despite it has been covered in a separate project to deal with CSV files, and eventually API calls to get the correct latitude/longitude of a particular city, this new project brings an opportunity to create a view of this analysis using HTML pages, nicely implemented using CSS and Bootstrap.

In summary, the page is organised in 4 pages:
* A  **landing page** that contains the following elements:
	- An explanation of the project.
	- A link to each visualization page. For these, a sidebar containing a preview image of each visualization. Clicking an image, it takes the user to that visualization.

* Four  **visualisation pages**, each with the following elements:
	- A descriptive title and a heading tag.
	- The visualization for the selected comparison (latitude vs. max temperature, latitude vs. humidity, latitude vs. cloudiness, or latitude vs. wind speed).        
	- A paragraph describing the visualization and its significance.

* A **comparisons page** that does the following:
	- All the visualisations on the same page so that people can easily compare them.
	- Uses a Bootstrap grid for the visualizations. This grid contains two visualisations across a medium or large screen and one visualization across an extra-small or small screen.

* A  **data page** that displaying a responsive table containing the data that the visualisations use, as follows:
	- The table configured as a Bootstrap  `table`  component.
	- The data must comes from the extraction of the data available in the provided CSV file using panda. This Jupyter notebook is also available in the project repository `load_csv.ipynb` (under the folder `Resources`).

Finally, and very important, at the top of every page, this website also has a navigation bar that does the following:
* Contains the name of the site on the left side of the navigation bar, allowing users to return to the landing page from any page.
* Contains a drop-down menu, named Plots, on the right side of the navigation bar that contains a link to each visualization page.
* Provides two more text links on the right side: Comparisons, which links to the comparisons page, and Data, which links to the data page.
* Is responsive (via media queries).