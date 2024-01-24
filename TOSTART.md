    <strong>
How to run this Api
</strong>
<p>
At first open postman 
<li>
Method: POST
http://localhost:8000/api/regseter
<p>
Click in body of postman
go to form-data
fill here 
key and value
<li>
key 'name'
key 'email'
key 'password'
key 'c_password'
</li>
<li>
value 'testuser'
value 'user@gmail.com'
value 'user'
value 'user'
</li>
it will make user and give token like this 
    <br>
{
    "success": true,   <br>
    "data": {  <br>
        "token": "4|duRq29y9VBPxRpc2uBnxupHJeHUbt4Xyqx4HxcYpfb0ef858",  <br>
        "name": "user"  <br>
    },  <br>
    "message": "User registered successfully"  <br>
}
      <br>
</p>
</li>




<li>
Method: POST
http://localhost:8000/api/login 
<p>
Click in body of postman
go to form-data
provide your user data 
key and value
<li>
 
key 'email'
key 'password'
 
</li>
<li>
 
value 'user@gmail.com'
value 'user'
 
</li>
it will make user and give token for login that user like this 
{
    "success": true,
    "data": {
        "token": "5|ZV5hvCdW9Zg4njWHz8b9HbJqiEMp6BaK1GNG3009fc2ca61e",
        "name": "user"
    },
    "message": "User login successfully"
}
</p>
</li>
<li>
to see the user or list user 
Method will be GET
http://localhost:8000/api/user
<p>
go to Authorization  choose Bearer Token here enter that login token then it will list that token user 
</p>
<p>
like this 
{
    "id": 4,
    "name": "user",
    "email": "email@gmail.com",
    "email_verified_at": null,
    "created_at": "2024-01-24T07:19:11.000000Z",
    "updated_at": "2024-01-24T07:19:11.000000Z"
}
</p>
</li>

</p>
