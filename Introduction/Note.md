<!-- CSS Grid -->

<!-- Introduction:  -->

CSS Grid Layout is a powerful layout system available in CSS. It allows developers to create complex layouts easily and efficiently. Unlike Flexbox, which is one-dimensional (either a row or a column), CSS Grid is two-dimensional, allowing for both rows and columns.

<!-- Basic Concepts of CSS Grid -->

<!-- Defining a Grid Container -->

To use CSS Grid, you need to define a grid container using the display: grid; property.

<!-- Project 1 :  Defining a Grid Container-->

<!-- Grid Lines, Tracks, and Cells -->

<!-- Defining Rows and Columns -->

You can define the number of rows and columns using the grid-template-rows and grid-template-columns properties.


<!-- 

<style>
    .grid-container {
        display: grid;
        grid-template-columns: 100px 200px 100px;
        grid-template-rows: 50px 100px;
        gap: 10px;
    }
    .grid-item {
        background-color: #ccc;
        padding: 20px;
        text-align: center;
    }
</style>


 -->


 <!-- Explanation:  -->
 
 This creates a grid with 3 columns (100px, 200px, and 100px) and 2 rows (50px and 100px).

 <!-- Mini-Project: Custom Grid Layout with Varying Column and Row Sizes  -->

Create a layout with different sized columns and rows to understand how grid-template-columns and grid-template-rows work.


<!-- 
Enhance the Layout: Add more styles or content to the grid items to see how they adjust within the different-sized columns and rows.


<style>
    .grid-item {
        background-color: #ccc;
        padding: 20px;
        text-align: center;
        border: 1px solid #000;  /* Added border for better visibility */
    }
</style>


 -->


 <!-- Grid Areas -->

 <!-- Naming Grid Areas: -->
 
  You can name grid areas and place items accordingly using the grid-template-areas property.

<!-- Mini-Project: Create a Webpage Layout with Named Grid Areas -->
<!-- 

<style>
    .grid-container {
        display: grid;
        grid-template-areas: 
            'header header header'
            'sidebar content content'
            'footer footer footer';
        gap: 10px;
    }
    .header {
        grid-area: header;
    }
    .sidebar {
        grid-area: sidebar;
    }
    .content {
        grid-area: content;
    }
    .footer {
        grid-area: footer;
    }
</style>

 -->




 <!-- 
 
 
 <style>
    .header {
        background-color: #f8b400;  /* Yellow */
        padding: 20px;
        text-align: center;
    }
    .sidebar {
        background-color: #4caf50;  /* Green */
        padding: 20px;
        text-align: center;
    }
    .content {
        background-color: #2196f3;  /* Blue */
        padding: 20px;
        text-align: center;
    }
    .footer {
        background-color: #ff5722;  /* Orange */
        padding: 20px;
        text-align: center;
    }
</style>

 
  -->



  <!-- Grid Item Placement -->

  <!-- Placing Items:   -->


 You can place items explicitly using properties like grid-column-start, grid-column-end, grid-row-start, and grid-row-end.


 <!-- 
 
 <style>
    .grid-container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 10px;
    }
    .grid-item:nth-child(1) {
        grid-column: 1 / 3;  /* span two columns */
    }
    .grid-item:nth-child(2) {
        grid-row: 2 / 4;  /* span two rows */
    }
</style>

  -->



  <!--5. Responsive Design with Grid -->


  <!-- Media Queries and Auto-fill:  -->
  
  Combine CSS Grid with media queries to create responsive designs.

  <!-- 
  <style>
    .grid-container {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
        gap: 10px;
    }
</style>

   -->


<!-- 
Mini-Project: Create a responsive photo gallery that adjusts the number of columns based on screen size.
 -->


 <!-- Advanced Grid Properties -->

 <!-- Grid Auto Flow:  -->

  Controls how auto-placed items are inserted in the grid.

  <!-- Mini-Project: Create a layout with grid auto-flow to manage how items are placed. -->