# 📖 Data Analytics Glossary & Key Terms
## Essential Vocabulary for Interview Success

## 📋 Table of Contents
1. [Data Fundamentals](#data-fundamentals)
2. [Statistical Terms](#statistical-terms)
3. [SQL and Database Terms](#sql-and-database-terms)
4. [Python and Programming Terms](#python-and-programming-terms)
5. [Business Intelligence Terms](#business-intelligence-terms)
6. [Analytics Methodologies](#analytics-methodologies)
7. [Industry-Specific Terms](#industry-specific-terms)

---

## 📊 Data Fundamentals

### **Algorithm**
- **Definition**: Step-by-step instructions for solving a problem
- **Example**: Our data cleaning process (remove duplicates → fix formats → validate)
- **Interview Context**: "I followed a systematic algorithm to ensure consistent data quality"

### **API (Application Programming Interface)**
- **Definition**: Way for different software systems to communicate
- **Example**: Kaggle API to download datasets
- **Interview Context**: "I used APIs to automate data collection from multiple sources"

### **Big Data**
- **Definition**: Datasets too large or complex for traditional tools
- **Characteristics**: Volume, Velocity, Variety, Veracity
- **Interview Context**: "While our Walmart dataset is manageable, I understand Big Data principles"

### **Data Lake**
- **Definition**: Storage system for raw data in its native format
- **Comparison**: Unlike databases, data lakes store unstructured data
- **Interview Context**: "Data lakes are useful for storing diverse data types before processing"

### **Data Warehouse**
- **Definition**: Central repository for structured, processed data
- **Purpose**: Optimized for analysis and reporting
- **Interview Context**: "I loaded clean Walmart data into databases, similar to a data warehouse"

### **Dataset**
- **Definition**: Collection of related data organized for analysis
- **Example**: Our 10,051 Walmart transactions
- **Interview Context**: "I worked with a retail dataset containing customer transaction records"

### **Data Pipeline**
- **Definition**: Series of processes that move data from source to destination
- **Example**: CSV → Python cleaning → Database → SQL analysis
- **Interview Context**: "I built an end-to-end pipeline from raw data to business insights"

### **Data Quality**
- **Definition**: Measure of data's fitness for its intended use
- **Dimensions**: Accuracy, Completeness, Consistency, Timeliness
- **Interview Context**: "I addressed quality issues by removing 81 duplicates and standardizing formats"

### **Data Type**
- **Numeric**: Numbers (integers, floats)
- **Categorical**: Categories or labels
- **Temporal**: Time-related data
- **Boolean**: True/False values
- **Interview Context**: "I converted price strings to numeric type for mathematical operations"

### **ETL (Extract, Transform, Load)**
- **Extract**: Get data from source systems
- **Transform**: Clean and process the data
- **Load**: Put processed data into target system
- **Interview Context**: "My project demonstrates complete ETL pipeline implementation"

### **Feature Engineering**
- **Definition**: Creating new variables from existing data
- **Example**: Calculating total_amount = unit_price × quantity
- **Interview Context**: "I engineered features to enable better business analysis"

### **Metadata**
- **Definition**: Data about data (column names, data types, descriptions)
- **Example**: Knowing that 'rating' column ranges from 1-10
- **Interview Context**: "Understanding metadata helped me interpret the analysis correctly"

---

## 📈 Statistical Terms

### **Average (Mean)**
- **Definition**: Sum of all values divided by count
- **Formula**: Σx / n
- **Example**: Average transaction amount across all sales
- **Interview Context**: "I calculated mean values to understand typical customer behavior"

### **Median**
- **Definition**: Middle value when data is sorted
- **When to Use**: Better than mean when outliers exist
- **Example**: Median transaction value shows typical purchase size
- **Interview Context**: "I used median to avoid skewing from extremely high-value transactions"

### **Mode**
- **Definition**: Most frequently occurring value
- **Example**: Most common payment method in our dataset
- **Interview Context**: "Mode analysis revealed customer payment preferences"

### **Standard Deviation**
- **Definition**: Measure of how spread out data points are
- **Interpretation**: Low = consistent, High = variable
- **Interview Context**: "Standard deviation helped identify consistent vs. variable performance"

### **Correlation**
- **Definition**: Relationship between two variables
- **Range**: -1 (negative) to +1 (positive)
- **Example**: Correlation between price and customer rating
- **Interview Context**: "I analyzed correlations to identify factors affecting customer satisfaction"

### **Distribution**
- **Definition**: How values are spread across the range
- **Types**: Normal, skewed, uniform
- **Interview Context**: "Understanding distribution helped me choose appropriate analysis methods"

### **Outlier**
- **Definition**: Data point significantly different from others
- **Impact**: Can skew analysis results
- **Example**: $500 transaction when most are under $100
- **Interview Context**: "I identified and appropriately handled outliers in the dataset"

### **Percentile**
- **Definition**: Value below which a percentage of data falls
- **Example**: 75th percentile of transaction amounts
- **Interview Context**: "Percentile analysis revealed spending patterns across customer segments"

### **Sample vs Population**
- **Population**: All possible data points
- **Sample**: Subset of population
- **Example**: Our 10K transactions are a sample of all Walmart transactions
- **Interview Context**: "I treated our dataset as a representative sample for analysis"

### **Statistical Significance**
- **Definition**: Likelihood that observed differences are real, not random
- **Importance**: Helps validate findings
- **Interview Context**: "I ensured adequate sample sizes for statistically significant results"

---

## 🗄️ SQL and Database Terms

### **ACID Properties**
- **Atomicity**: All or nothing transactions
- **Consistency**: Data integrity maintained
- **Isolation**: Concurrent transactions don't interfere
- **Durability**: Committed changes persist
- **Interview Context**: "I understand database reliability principles"

### **Aggregate Functions**
- **COUNT()**: Number of records
- **SUM()**: Total of numeric values
- **AVG()**: Average value
- **MIN()/MAX()**: Smallest/largest values
- **Interview Context**: "I used aggregation to summarize business metrics"

### **Database Schema**
- **Definition**: Structure of database tables and relationships
- **Components**: Tables, columns, data types, constraints
- **Interview Context**: "I designed schema to optimize for analytical queries"

### **Index**
- **Definition**: Database structure that improves query performance
- **Trade-off**: Faster reads, slower writes
- **Interview Context**: "Indexing on frequently queried columns improves performance"

### **JOIN Operations**
- **INNER JOIN**: Records matching in both tables
- **LEFT JOIN**: All records from left table, matches from right
- **RIGHT JOIN**: All records from right table, matches from left
- **FULL OUTER JOIN**: All records from both tables
- **Interview Context**: "I used JOINs to combine related datasets for comprehensive analysis"

### **Normalization**
- **Definition**: Organizing data to reduce redundancy
- **Levels**: 1NF, 2NF, 3NF (First, Second, Third Normal Form)
- **Interview Context**: "Normalized design prevents data inconsistency issues"

### **Primary Key**
- **Definition**: Unique identifier for each record
- **Properties**: Not null, unique, immutable
- **Example**: invoice_id in our Walmart data
- **Interview Context**: "Primary keys ensure data integrity and enable reliable joins"

### **Query Optimization**
- **Definition**: Improving query performance
- **Techniques**: Proper indexing, efficient WHERE clauses, avoiding SELECT *
- **Interview Context**: "I write efficient queries to handle large datasets effectively"

### **Subquery**
- **Definition**: Query nested inside another query
- **Types**: Correlated, non-correlated
- **Example**: Finding branches with above-average sales
- **Interview Context**: "Subqueries enable complex analytical comparisons"

### **Window Functions**
- **Definition**: Perform calculations across related rows
- **Examples**: RANK(), ROW_NUMBER(), LAG(), LEAD()
- **Interview Context**: "Window functions enabled sophisticated ranking and trend analysis"

---

## 🐍 Python and Programming Terms

### **Data Frame**
- **Definition**: Two-dimensional labeled data structure in pandas
- **Similar to**: Excel spreadsheet or SQL table
- **Interview Context**: "I used DataFrames for all data manipulation tasks"

### **Function**
- **Definition**: Reusable block of code that performs specific task
- **Benefits**: Code organization, reusability, testing
- **Interview Context**: "I created functions to standardize repetitive data processing tasks"

### **Library/Package**
- **Definition**: Collection of pre-written code modules
- **Examples**: pandas, numpy, matplotlib
- **Interview Context**: "I leveraged established libraries rather than reinventing functionality"

### **Loop**
- **Definition**: Code structure that repeats actions
- **Types**: for loops, while loops
- **Interview Context**: "I used loops to process multiple data files efficiently"

### **Null/NaN Values**
- **Definition**: Missing or undefined data
- **Handling**: Drop, fill, interpolate
- **Interview Context**: "I developed strategies for handling missing data appropriately"

### **Object-Oriented Programming (OOP)**
- **Definition**: Programming paradigm using objects and classes
- **Concepts**: Encapsulation, inheritance, polymorphism
- **Interview Context**: "Understanding OOP helps me work with complex data structures"

### **Series**
- **Definition**: One-dimensional labeled array in pandas
- **Relationship**: DataFrame columns are Series objects
- **Interview Context**: "I used Series for single-column operations and analysis"

### **Variable**
- **Definition**: Named storage location for data
- **Types**: String, integer, float, boolean, list, dictionary
- **Interview Context**: "Proper variable naming makes code readable and maintainable"

---

## 💼 Business Intelligence Terms

### **Dashboard**
- **Definition**: Visual display of key metrics and KPIs
- **Purpose**: Real-time monitoring and decision support
- **Interview Context**: "I would create dashboards to visualize my analysis findings"

### **Data Visualization**
- **Definition**: Graphical representation of data
- **Types**: Bar charts, line graphs, scatter plots, heat maps
- **Interview Context**: "Visualization makes complex data insights accessible to stakeholders"

### **Key Performance Indicator (KPI)**
- **Definition**: Measurable value demonstrating business objective achievement
- **Examples**: Revenue growth, customer satisfaction, profit margin
- **Interview Context**: "I identified KPIs relevant to Walmart's business objectives"

### **Business Intelligence (BI)**
- **Definition**: Technologies and strategies for data analysis and presentation
- **Components**: Data warehousing, reporting, analytics, visualization
- **Interview Context**: "My project demonstrates end-to-end BI implementation"

### **Dimensional Modeling**
- **Definition**: Data warehouse design technique
- **Components**: Fact tables (metrics) and dimension tables (attributes)
- **Interview Context**: "I understand how to structure data for analytical reporting"

### **Drill-down/Drill-up**
- **Drill-down**: View more detailed data
- **Drill-up**: View summarized data
- **Example**: Company → Region → Store → Category
- **Interview Context**: "I designed analysis to support different levels of detail"

### **OLAP (Online Analytical Processing)**
- **Definition**: Technology for complex analytical queries
- **Operations**: Slice, dice, drill, pivot
- **Interview Context**: "OLAP concepts guided my multidimensional analysis approach"

### **ROI (Return on Investment)**
- **Definition**: Measure of investment efficiency
- **Formula**: (Gain - Cost) / Cost × 100%
- **Interview Context**: "I can calculate ROI for data-driven business initiatives"

---

## 🔬 Analytics Methodologies

### **A/B Testing**
- **Definition**: Comparing two versions to determine which performs better
- **Application**: Testing payment method promotions
- **Interview Context**: "I understand experimental design for business optimization"

### **Cohort Analysis**
- **Definition**: Studying groups of users over time
- **Example**: Analyzing customer behavior by signup month
- **Interview Context**: "Cohort analysis reveals customer lifecycle patterns"

### **Descriptive Analytics**
- **Definition**: What happened in the past
- **Example**: Total sales by branch last quarter
- **Interview Context**: "My Walmart analysis primarily used descriptive methods"

### **Diagnostic Analytics**
- **Definition**: Why something happened
- **Example**: Why did sales drop in certain stores?
- **Interview Context**: "I investigated root causes of performance variations"

### **Predictive Analytics**
- **Definition**: What is likely to happen
- **Techniques**: Machine learning, statistical modeling
- **Interview Context**: "I could extend analysis to forecast future sales trends"

### **Prescriptive Analytics**
- **Definition**: What should be done
- **Output**: Recommendations and optimal actions
- **Interview Context**: "I provided actionable recommendations based on data insights"

### **Regression Analysis**
- **Definition**: Statistical method for examining relationships
- **Types**: Linear, logistic, polynomial
- **Interview Context**: "Regression could model factors affecting sales performance"

### **Segmentation**
- **Definition**: Dividing customers/data into meaningful groups
- **Example**: High-value vs. low-value customers
- **Interview Context**: "I segmented data by branch, category, and payment method"

---

## 🏪 Industry-Specific Terms (Retail Analytics)

### **Basket Analysis**
- **Definition**: Analyzing items purchased together
- **Purpose**: Cross-selling and product placement
- **Interview Context**: "Market basket analysis could optimize product recommendations"

### **Customer Lifetime Value (CLV)**
- **Definition**: Total value a customer brings over their relationship
- **Calculation**: Average order value × frequency × lifespan
- **Interview Context**: "CLV analysis guides customer acquisition investment"

### **Inventory Turnover**
- **Definition**: How quickly inventory is sold and replaced
- **Formula**: Cost of goods sold / Average inventory
- **Interview Context**: "High turnover indicates efficient inventory management"

### **Same-Store Sales**
- **Definition**: Sales comparison for stores open in both periods
- **Purpose**: Measure organic growth excluding new store impact
- **Interview Context**: "Same-store sales show true business performance"

### **SKU (Stock Keeping Unit)**
- **Definition**: Unique identifier for each product variant
- **Example**: Different sizes/colors of same product have different SKUs
- **Interview Context**: "SKU-level analysis provides detailed product insights"

### **Point of Sale (POS)**
- **Definition**: Where transactions occur
- **Data**: Transaction details, timing, payment methods
- **Interview Context**: "POS data is the foundation of retail analytics"

---

## 🎯 Interview Success Tips

### **How to Use This Glossary**

1. **Before Interview**: Review terms relevant to the job description
2. **During Interview**: Use terminology naturally, don't force it
3. **When Explaining**: Define terms if interviewer might not know them
4. **Show Understanding**: Connect terms to real business impact

### **Red Flags to Avoid**

- Using terms incorrectly
- Over-using jargon without substance
- Not being able to explain terms you use
- Memorizing definitions without understanding application

### **Green Flags to Demonstrate**

- Connecting technical terms to business value
- Explaining complex concepts simply
- Using appropriate terminology for the audience
- Showing how terms relate to your project experience

Remember: The goal isn't to use every term, but to use the right terms correctly and demonstrate deep understanding of the concepts behind them!