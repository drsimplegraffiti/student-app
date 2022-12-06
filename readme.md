>  Lombok annotations to reduce the boilerplate code such as getter/setter methods, and constructors.

```
@Entity annotation is used to mark the class as a persistent Java class.
@Table annotation is used to provide the details of the table that this entity will be mapped to.
@Id annotation is used to define the primary key.
@GeneratedValue annotation is used to define the primary key generation strategy. In the above case, we have declared the primary key to be an Auto Increment field.
@Column annotation is used to define the properties of the column that will be mapped to the annotated field. You can define several properties like name, length, nullable, updateable, etc.
```


#### Always create the db in the mysql bench or terminal before running the app


---
#### Endpoints
POST localhost:6767/api/users

```json
{
  "id": 1,
  "firstName": "abayomi",
  "lastName": "joseph",
  "email": "a@b.c"
}
```


#### Get all users
> GET localhost:6767/api/users

#### Get single user by id
> POST localhost:6767/api/users/{id}

#### Delete single user by id
> DELETE localhost:6767/api/users/{id}


#### Update single user by id
> PUT localhost:6767/api/users/{id}
```json
 "firstName" : "abayomi",
  "lastName": "joseph",
  "email": "a@b.c"
```


---

#### Order endpoints

#### Create new order
> POST localhost:6767/api/orders
```
"orderTrackingNumber":"Yhs78",
"totalQuantity":45,
"totalPrice":9000,
"status":"Completed"
```

#### Get all orders
> GET localhost:6767/api/orders


---

####  Create new address
> POST localhost:6767/api/address
```
"name":"London bridge",
"city":"Lagos",
"state":"Lagos",
"country":"Nigeria",
"zipcode":"23401"
```


#### Removing Github remote from the project 
> For the Invalid VCS root mapping error you can fix it by deleting the vcs.xml file located in the .idea folder of your project and then rebuild your project.
