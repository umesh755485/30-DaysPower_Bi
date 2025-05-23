<h1>Power BI Series Day 2: Data Modeling and Creating Relationships</h1>

<p>
     * What is Data Modeling in Power BI?
          Data modeling in Power BI is the process of structuring your data tables and defining how they relate to each other. This step is crucial for building                efficient, accurate, and interactive reports and dashboards
</p>


<h2> ## Key Concepts</h2>
<p>
     * Fact Table: Stores measurable, quantitative data, repeated data... that table is called as fact table  (e.g., sales, transactions).
    <br>
     * Dimension Table: Contains descriptive attributes(we can say unique values) (e.g., customer, product, date).
    <br>
     * Star Schema: The recommended layout, where a central fact table connects to multiple dimension tables. This structure is simple, efficient, and improves performance
</p>

<h2>Steps to Create a Data Model and Relationships</h2>
1. Import Your Data
   * Load tables from sources like Excel, SQL, or CSV into Power BI.

2. Open Model View
   * Click the Model icon on the left sidebar to visualize your tables and relationships.

3. Create Relationships
   * Automatic: Power BI may detect and create relationships based on matching column names.



       <img src="Day2/relationship-of-tables.png"  alt="relation-of-tables" />

  
 

## Manual:
* Drag a field (key column) from one table to the matching field in another table.

Or, go to Modeling > Manage Relationships > New to define the relationship.

4. Set Relationship Properties
Cardinality: Most commonly "One-to-Many" (1:*), where the "one" side is a dimension table and the "many" side is a fact table.

Cross Filter Direction: Usually set to "Single" for best performance.

Active/Inactive: You can have multiple relationships but only one active at a time between two tables.

5. Validate and Optimize
Test your relationships using visuals and slicers.

Remove unnecessary columns and tables to keep your model lean and performant
