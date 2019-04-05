# Express REST API

This is an example of REST API for data managing at MongoDB database.

## Build and run

* Install dependencies: `npm install`

* Create `credentials.js` file and put the following content here:
    
    ```
    const pass = "mongodb+srv://<USERNAME>:<PASSWORD>@cluster0-okon8.mongodb.net/<DBNAME>?retryWrites=true";
    module.exports = {
        pass
    }
    ```
    Where you should replace <USERNAME>, <PASSWORD> and <DBNAME> with your username, password 
        and database name at the MongoDB database accordingly.
    
* Run the service: `node server`

## Structure

Structure of the object `Data` is located in `data.js` file.
<br/>
Structure of the object `Token` is located in `token.js` file.

There it is possible to change internal structure and behaviour of the objects.

`credentials.js` file is needed to provide the api an information for the connection to the database.

`Server.js` is where the data manipulation methods are located.