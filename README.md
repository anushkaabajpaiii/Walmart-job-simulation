# Walmart-job-simulation
Implemented a modified heap for Walmart's priority queue, designed a UML for data processors with multiple modes and databases, created an ERD for pet products, shipments, and customer transactions, and developed a Python script to merge and load shipment data into a normalized SQLite database.
1. Priority Queue for Walmart Shipping Department
This project involved implementing a modified heap structure in Java to optimize a priority queue for the Walmart Shipping Department. The heap design incorporated 2^x children for each parent node, allowing benchmarking of insert and pop max operations to minimize bottlenecks. The implementation ensured performance and correctness while allowing scalability for different x values.

2. UML Class Diagram for Data Processors
The task focused on drafting a UML class diagram for a pipeline processor system. The processor supported three modes:

Dump mode (drops data),

Passthrough mode (inserts data into a database), and

Validate mode (validates and inserts data).
It also allowed switching between databases such as Postgres, Redis, and Elastic. The goal was to structure code abstractly while meeting specific functionality requirements.

3. ERD for Pet Product Management Database
This project involved creating an Entity-Relationship Diagram (ERD) to design a relational database for managing pet products. The database stored details for:

Pet food (name, manufacturer, weight, flavor, health conditions),

Pet toys (material, durability), and

Pet apparel (color, size, care instructions).
The system also tracked customer transactions, shipments between warehouses and stores, and manufacturer details. It normalized data relationships to ensure efficiency and scalability.

4. Data Ingestion into SQLite Database
This project required writing a Python script to process and load data from three spreadsheets into an SQLite database. The spreadsheets contained:

Information about shipments (origin_warehouse, destination_store, and product_quantity).

Products in each shipment (shipment_identifier and product).

Additional shipment details (origin_warehouse, destination_store, and driver_identifier).
The script merged related data, transformed it to fit the database schema, and inserted it into two tables: Shipments and ShipmentDetails.

5. Python Script for Database Population
The Python script processed data from the spreadsheets by:

Merging shipments and product data using shipment_identifier.

Normalizing the data into tables for shipments and detailed product information.

Populating the database with all required fields like product quantity, shipment origins, and destinations.
The database schema was created to handle real-world scenarios, ensuring data integrity and compatibility with future updates.
