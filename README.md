# MongoDB 

In this repository, you'll find a collection of MongoDB terminal commands, along with instructions on how to perform common tasks using the MongoDB shell.

## Getting Started

Before you can start using MongoDB terminal commands, you'll need to have MongoDB installed and your MongoDB server running.

### Prerequisites

Make sure you have the following prerequisites:

- [MongoDB](https://www.mongodb.com/try/download/community) installed on your local machine or a remote server.

## Connecting to MongoDB

To connect to your MongoDB server using the MongoDB shell, follow these steps:

### Step 1: Open the MongoDB Shell

Open your terminal or command prompt and enter the following command to launch the MongoDB shell:

```bash
mongo
```

### Step 2: Connect to the MongoDB Server

Once the shell is open, you can connect to your MongoDB server. Replace `<server_address>` with your MongoDB server's address (e.g., localhost) and `<port>` with the port number (e.g., 27017):

```bash
mongo --host <server_address> --port <port>
```

You should see a connection message indicating that you're connected to the MongoDB server.

## Creating a Database

To create a new database in MongoDB, you can use the following command:

```bash
use <database_name>
```

Replace `<database_name>` with your desired database name. If the database doesn't exist, MongoDB will create it for you.

## Creating a Collection

Collections in MongoDB are where your data is stored. You can create a new collection in your database as follows:

```bash
db.createCollection('<collection_name>')
```

Replace `<collection_name>` with the name of your collection.

## Usage

You can now start using MongoDB terminal commands to interact with your database and collections. Here are some common tasks:

### Inserting Documents

```bash
db.<collection_name>.insertOne({ key1: 'value1', key2: 'value2' })
db.<collection_name>.insertMany([
  { key1: 'value1', key2: 'value2' },
  { key1: 'value3', key2: 'value4' }
])
```

### Querying Documents

```bash
db.<collection_name>.find({ key1: 'value1' })
db.<collection_name>.findOne({ key1: 'value1' })
```

### Updating Documents

```bash
db.<collection_name>.updateOne({ key1: 'value1' }, { $set: { key2: 'new_value' } })
db.<collection_name>.updateMany({ key1: 'value1' }, { $set: { key2: 'new_value' } })
```

### Deleting Documents

```bash
db.<collection_name>.deleteOne({ key1: 'value1' })
db.<collection_name>.deleteMany({ key1: 'value1' })
```

## Contribution

Contributions to this repository are welcome! If you have MongoDB terminal commands or examples you'd like to share, please open a pull request.
