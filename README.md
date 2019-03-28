# go-echo-mongo
Simple Golang REST application with Echo Framework & MongoDB

# How to run
These are the steps to run this app: 
1. Make sure Golang,Glide(Go Package Manager), and MongoDB are installed
2. Go to project root directory (```$GOPATH/src/github.com/.../go-echo-mongo```)
3. Run command ```glide install``` to install the dependencies
4. Run command ```go run main.go``` to start the server

# Endpoint
These are the list of endpoint:

Method       | Headers                          | URI               | Description       | Response Success |
------------ | -------------------------------- | ----------------- | -----------------
POST         | ```Accept: 'application/json'``` | /users            | Create new user.  | ```{"data":{"userId":"USER001","firstName":"Patrick","lastName":"Sangian","email":"patricksangian@gmail.com","password":"14qwafzx","createdAt":"2019-03-27T16:57:35.604+07:00","updatedAt":"2019-03-27T16:57:35.604+07:00"},"error":false,"message":"Detail of user"}``` |
GET          | ```Accept: 'application/json'``` | /users/<:userID>  | Get user by ID.   ||
GET          | ```Accept: 'application/json'``` | /users            | Get list of user. ||

# References
- [YouTube] (https://www.youtube.com/playlist?list=PLMrwI6jIZn-3a4Hjn-GoYihbMBAzZ6Ae3)
- [GitHub] (https://github.com/bxcodec/go-clean-arch)
