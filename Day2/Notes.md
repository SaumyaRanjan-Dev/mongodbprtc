# MongoDB Query API

The MongoDB Query API is the primary method to interact with your data. It supports various operations and functionalities to manage and query data effectively.

## MongoDB Query API Features

### Two Primary Uses:
1. **CRUD Operations**: Perform Create, Read, Update, and Delete operations.
2. **Aggregation Pipelines**: Transform and analyze data.

### Use Cases:
- **Adhoc Queries**: Utilize tools like mongosh, Compass, VS Code, or MongoDB drivers for various programming languages.
- **Data Transformations**: Leverage aggregation pipelines for complex data processing.
- **Document Joins**: Combine data from different collections.
- **Graph and Geospatial Queries**: Query graph structures and geospatial data.
- **Full-Text Search**: Perform text-based searches.
- **Indexing**: Enhance query performance by indexing fields.
- **Time Series Analysis**: Analyze and manage time-series data.

## MongoDB `mongosh` Create Database

### Create a Database Using `mongosh`

After connecting to your database using `mongosh`, you can determine the current database by typing:
```bash
db
```
If you connected using the connection string from the MongoDB Atlas dashboard, you should be connected to the `myFirstDatabase` database.

### Show All Databases
To list all available databases, type:
```bash
show dbs
```
Note: If `myFirstDatabase` is not listed, it is because the database is empty. MongoDB does not display empty databases.

### Change or Create a Database
To switch to an existing database or create a new one, use the `use` command followed by the database name:
```bash
use <database_name>
```

### Example
Create a new database named `blog`:
```bash
use blog
```
If the `blog` database does not exist, this command will create it.
