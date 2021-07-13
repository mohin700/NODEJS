# Authintacitation MongoDB
### 1. Select Admin DB 
```use admin```

### 2. Create Root User -
```
db.createUser(
  {
    user: "root",
    pwd: "ckax3{H6xqpEggM",
    roles: [ { role: "userAdminAnyDatabase", db: "admin" }, "readWriteAnyDatabase" ]
  }
)
```

### 3. Create New DB level User -
``` 
 db.createUser(
   {
     user: "cryptacoraUser",
     pwd: "]hV@!6^vJ~?RsE%c",
     roles: [ { role: "dbOwner", db: "cryptacora" } ]
   }
 )
``` 
 
### 4. Update User Info
```
db.updateUser(
    "root", //DB user 
  {
    roles: [ { role: "userAdminAnyDatabase", db: "admin" }, "readWriteAnyDatabase" ] //Updated Data
  }
)
```

### 5. Connect from application 
```
mongoose.createConnection(
  "mongodb://localhost:27017/dbName", // url with DB
  {
    "auth": {
      "authSource": "admin"
    },
    "user": "root", // username 
    "pass": "mohin123", // password
    useCreateIndex: true, 
    useUnifiedTopology: true, 
    useNewUrlParser: true,
    useFindAndModify: false 
  }
); 
```
