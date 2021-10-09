
# Instagram API

In the project, MongoDB was used locally. All functions have been
implemented using standard go library

The password of a user was encrypted and stored in its encrypted form in the database, when a user makes a GET reuqest for a user, the password returned in JSON is encrypted.

The project is divied into 3 folders, the handler file implements all the API endpoint functions and has method to connect to database. The model file implements the data struture for the API and the encrypt file has functions to encrypt the password. main.go file starts the server on port 8000.

```
Attributes of Users :
Id
Name
Email
password

Attributes of posts :
Id
Caption
Image_URL
Timestamp
UserId
```
## API Reference

#### Create users 
```http
  POST /users
```

#### Get users By ID 

```http
  GET /users/{id}
```
#### Create posts 

```http
  POST /posts
```
#### Get post By ID 

```http
  GET /posts/{id}
```
#### Get all post by a user

```http
  GET /posts/users/{id}
```

## Screenshots

Create a User 
![CreateUser](https://user-images.githubusercontent.com/62784600/136660575-a5582a18-d045-4dc8-b015-2dc0784536a4.png)

Get a User by ID 
Password is encrypted
![GetUserByID](https://user-images.githubusercontent.com/62784600/136660597-86cce7cc-9f33-491f-a278-57edf6502e94.png)

Create a Post
![CreatePost](https://user-images.githubusercontent.com/62784600/136660624-79e38872-b25d-4f2f-9f51-c62092df1b7b.png)

Get a Post by ID
![GetPostByID](https://user-images.githubusercontent.com/62784600/136660669-7c8e416c-447a-4562-a9ad-95753830111a.png)

Get all post made by a User
![last1](https://user-images.githubusercontent.com/62784600/136660707-f8d6a9e4-5d6c-400a-84a6-3a5984224f75.png)
![last2](https://user-images.githubusercontent.com/62784600/136660709-dadf2a3f-9b50-4574-b1c6-22cae77e435d.png)
![last3](https://user-images.githubusercontent.com/62784600/136660712-9dabe6e6-bf6f-48f9-b33f-91e49046bce7.png)

Data stored in mongo
![App Screenshot](https://imgur.com/0wAUxnp)

