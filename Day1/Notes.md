# MongoDB

MongoDB is a document database and can be installed locally or hosted in the cloud.

## SQL vs Document Databases

- **SQL Databases**:  
  SQL databases are considered relational databases. They store related data in separate tables. When data is needed, it is queried from multiple tables to join the data back together.

- **MongoDB (Document Database)**:  
  MongoDB is often referred to as a non-relational database. This does not mean that relational data cannot be stored in document databases, but rather that relational data is stored differently. A better term is "non-tabular database."

  MongoDB stores data in flexible documents. Instead of having multiple tables, you can keep all your related data together. This makes reading your data very fast.  
  In MongoDB, multiple groups of data are called **collections** instead of tables.

## Local vs Cloud Database

- **Local Database**:  
  MongoDB can be installed locally, allowing you to host your own MongoDB server on your hardware. This requires managing your server, upgrades, and maintenance.  
  You can download and use the MongoDB open-source Community Server for free.

- **Cloud Database**:  
  For ease of use, MongoDB Atlas—a cloud database platform—can be used. This eliminates the need to host your own local database.  
  To experiment with code examples, you will need access to a MongoDB database.  
  **Sign up for a free MongoDB Atlas account** to get started.

## Creating a Cluster

1. Create an account on MongoDB Atlas.
2. Set up a free "Shared Cluster."
3. Choose your preferred cloud provider and region.

### Configure Access

- **Database Access**:  
  Create a new user and keep track of the username and password.

- **Network Access**:  
  Add your current IP address to the list of allowed IP addresses.

## Install MongoDB Shell (mongosh)

To interact with your MongoDB database, install the MongoDB Shell (`mongosh`).

### Installation Instructions

Follow the [official instructions](https://www.mongodb.com/docs/mongodb-shell/install/) to install `mongosh` on your operating system.

### Verify Installation

Open your terminal and type:

```bash
mongosh --version
```

You should see the latest version installed.  
The version used in this tutorial is **v1.3.1**.

## Connect to the Database

To connect to your database, you will need a database-specific connection string.

1. In the MongoDB Atlas dashboard, under **Databases**, click the **Connect** button for your Cluster.
2. Choose **Connect with the MongoDB Shell**.
3. Copy your connection string.

### Example

Your connection string will look similar to this:

```bash
mongosh "mongodb+srv://cluster0.ex4ht.mongodb.net/myFirstDatabase" --apiVersion 1 --username YOUR_USER_NAME
```

Paste your connection string into your terminal and press Enter.  
You will be prompted to enter the database user password you created earlier.

You are now connected to the database.
