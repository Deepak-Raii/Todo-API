These are the TODO-APP API's.
Here i create seven API's, with JWT token,
first i check user is valid or not, if user is valid then he can perform CRUD operation. and if user is not valid, then he can not perform any operation.

1) User Signup API,
    method: POST,
    here user POST four data (username, password, email, age);
    
    http://localhost:3001/signup

2) User Signin API.
    method: GET,
    here we get token, after providing "email and password".
    
    http://localhost:3001/signin

3) Create TODO API,
    method: POST,
    here we will post (token for authentication, taskname, taskinformation, description, status, status will be "PENDING" bydefault at the time of creating TODO task, it will show status "COMPLETE" when user read the perticular TODO task).
    
    http://localhost:3001/addTodo

4) Read All TODO with Pagination API,
    method: GET,
    here we get all the todo after providing token. I have use pagination in this api, it show 5 data on a single page.
    
    http://localhost:3001/readTASK

5) Read the TODO task API,
    method: GET,
    here we get the todo task after providing token for authentication and taskname for perticular task. Here status will change pending to complete, means when user read the task then status will change pending to complete.
    
    http://localhost:3001/readTODO


6) Update TODO and Send mail API,
    method: PUT,
    here we will provide token for authentication, and we can update taskname, taskinformation, and description. if you want to send mail then you have to provide gmail account.

    http://localhost:3001/updateTODO

7) Delete TODO API,
    method: DELETE,
    here we provide token for authentication and taskname for delete the task.

    http://localhost:3001/daleteTODO
