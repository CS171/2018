---
layout: lab
---

<img src="cs171-logo.png" width="200">

&nbsp;

# Homework 1

In the first part of this homework you will create a simple webpage with HTML and CSS.

In the second part, you will search for different visualizations on the web and you will analyze the key aspects of what makes these visualizations *good* or *bad*, in your opinion.

This homework assumes that you have read Chapter 3 (up to page 36) in *D3 - Interactive Data Visualization for the Web* (Second Edition!) by Scott Murray.

&nbsp;


## 1. Web Development Basics: HTML & CSS (5 points)


### Data

The following table shows countries with an alarming hunger situation on the basis of the Global Hunger Index (GHI) scores from 1990, 2000 and 2014. The Index ranks countries on a 100-point scale, with 0 being the best score (no hunger) and 100 being the worst.

Country | 1990 | 2000 | 2014
------------ | ------------- | ------------ | ------------
Central African Republic | 51.9	 | 51.4 | 46.9
Chad | 65 | 52 | 46.4
Haiti | 52.1 | 42.8	 | 37.3
Madagascar | 44.8 | 44.1 | 36.3
Sierra Leone | 58.8	 | 53.5 | 38.9
East Timor | — | — | 40.7
Zambia | 47 | 50.9 | 41.1


*The Global Hunger Index (GHI) is designed to comprehensively measure and track hunger globally and by country and region. Calculated each year by the International Food Policy Research Institute (IFPRI), the GHI highlights successes and failures in hunger reduction and provides insights into the drivers of hunger.* (IFPRI, 2015)


### Design and Implementation

Please follow these instructions.

a. **Create a new HTML file `index.html` and a new external CSS file.**

You should give some thought to the organization of the files and folders of your web/visualization projects. Instead of dumping everything in one folder we suggest the following structure for the beginning:
	
```
hw/	
	index.html
	css/ 		...folder with all CSS files
	js/ 		...folder with all JavaScript files
```

b. **Include your external stylesheet in your HTML file**

c. **Add a headline to the HTML `body`**

d. **Implement the given table (Global Hunger Index) in HTML** 

Please be aware of the different html tags for rows with column names and rows with actual data (i.e., table header, table row).

e. **Add several custom styles to your external CSS file**

You can choose your design parameters freely (i.e., decisions about fonts, colors or scales are up to you) but make sure to include at least:
	
  - Custom font (e.g. Arial)
  - Custom style for the headline
  - Highlight column names in the table
  - Alternating row colors for the table

*Keeping your CSS rules separate means that you can use styles multiple times and your HTML documents remain clean and understandable.*

f. **Download and include the given JavaScript file `sorttable.js` at the bottom of the `body`-Element.**

[http://www.cs171.org/2018/assets/scripts/hw1/sorttable.js](http://www.cs171.org/2018/assets/scripts/hw1/sorttable.js)

Make sure to save the contents of this file as .js file! This script provides some additional functionality and makes your table sortable. Over the course of the semester, you will learn more about integrating interactive components with JavaScript but for this homework it is fine if you include our given library. Example integration:

```
<script src="js/sorttable.js"></script>
```

g. **Add the class name `sortable` to the `table`-Element**

If you have implemented everything correctly you should be able to sort the columns by clicking on the column names.

h. **Add a two-column layout below the table**

You should use the empty containers in the following exercise (*Good & Bad Visualizations*). Add the screenshots to the left column and the descriptions of the visualizations to the right column.

*We recommend the use of Bootstrap's [grid-system](https://getbootstrap.com/docs/3.3/css/#grid). It is very flexible and will definitely be helpful for future projects. 

*As a general rule, only use html `<table>` tags in an html layout to display data that can be well-represented in rows and columns (i.e., tabular data). Do not use it as a general layouting device!*


&nbsp;

## 2. *Good & Bad* Visualizations (5 points)


*The use of visualization to present information is pervasive in the media. A visual representation is a powerful and effective way to make complicated and confusing information more relevant and easy to understand.*

Here are some general questions to consider as you go through the next section: What is your opinion about good and bad visualizations? What are the characteristics of a good visualization and what makes a visualization bad, not understandable, or misleading (communicating the wrong information)?


a. **Search online for two good and two bad visualizations.**

Please choose examples from different authors/sources and put the focus on *static visualizations without interactivity*. You can use [http://viz.wtf/](http://viz.wtf/) for inspiration, but please try to find examples from different sources.

b. **Analyze the different design choices and visual encodings. Use the knowledge you have gained during lecture.**
   
Add your analysis in the next step (c) to the `index.html` file.
   
c. **Extend your previously created** `index.html` **file and add the following for each visualization:**

   * One screenshot
   * Describe the design choices (type, color, scale, visual elements, ...)
   * Explain in a paragraph why you have classified the respective visualization as good or bad. Describe the positive and negative aspects.
   * Authors of visualizations try to convey a specific point of view on a given dataset. What do you think the author wanted to communicate? Can you suggest any improvements?
   * Reference (i.e., link) to the source

***Add this information to your two-column layout.*** *In one column the screenshot and in the other column the design choices, positive and negative aspects etc.*

d. ***You should also make use of the (un)ordered list in HTML.*** *It helps you to structure information.*

e. **Create an image slider**

Use the four screenshots from your good and bad visualizations and create a slider/carousel. It should always show a single image and automatically slide to the next image after a few seconds.

***The slider should be visible above your examples.***

*You can use Bootstraps's carousel component, look for it here: [http://getbootstrap.com/javascript/](http://getbootstrap.com/javascript/)*

***Make sure your webpage is visually pleasing (e.g., image sizes are appropriate, images and text work together)

## 3. Bonus Task (1.0 points)

If you were able to finish all the previous tasks and feel up for a challenge, here is a bonus task for you. Each homework will contain a bonus task, which is completely optional and meant as additional challenge. Be aware that extra credit for bonus tasks is only given if the rest of the homework has been completed and the full possible points have been received.

***Graduate students: If you are taking CS171 as a graduate level course, the bonus tasks are required for you, please make sure you always complete them!***

Visualize the GHI scores from Task 1 in a tool of your choice (Excel, Tableau, R, Python, D3, ...) and insert the result into your webpage. It can be either a static image or an interactive visualization. Add a caption that exlains your visualization.

If you have not used Tableau so far, we would recommend you to have a look at it: [http://www.tableau.com/academic/students](http://www.tableau.com/academic/students).

- As a student you can download Tableau Desktop for free.
- You can export visualizations to Tableau Public and embed them in websites



## 4. Submit Homework on Canvas

**Go to Canvas and click on the HW 1 - Submission link in the week's modules. Next, upload a zipped folder containing your homework files.**

To upload an entire directory structure please compress your entire local directory (that contains your lab and homework) into a zip file. Use the following recommended folder structure:

```
/submission_hw1_FirstnameLastname	
	hw/
	    index.html
	    css/ 		...folder with all CSS files
	    js/ 		...folder with all JavaScript files
	    ...
```
Note that you should add your name to the filename using CamelCase style, e.g., ```submission_hw1_JohnDoe.zip``` if your name is John Doe. 

**Congratulations for finishing Homework 1! See you in class!**


<!--
*For your final submission you will have to:*

- Click the 'submit' button
Double-check your 'latest submission', check that all the visualizations are working as you expect. You can run them directly in Vocareum and look at them in a new window.
- Upload a teaser image of your homework (under 'Action'/'upload gallery thumbnail'. This teaser will show up in the classes gallery and should motivate other students to look at your solution in more detail.

*After the homework deadline you will be able to:*

- Look at the gallery with all other student submissions
- Give peer feedback or comments to other students (Please use proper manners and constructive criticism!)
- Give stars to other students' work (this will not influence grading!)
 
-->
