

<h1>HSK Hanyu Instructions</h1>
<p></p>
<h2>Install mongodb in docker</h2>
<p>Create a mongodb container in docker with bitnami's image</p>
<h3>Example Command:</h3>
<p>docker run --name mongodb -e MONGODB_USERNAME=dev1 -e MONGODB_PASSWORD=password123 -e MONGODB_DATABASE=my_database -e  MONGODB_ROOT_PASSWORD=passwordroot -p 27017:27017 bitnami/mongodb:latest</p>

<h2>connection.json</h2>
<p>This program needs a connection file to connect to your db. It's ignored by git so different environment's connection files are not over written on git pull</p>
<h3>connection.json example</h3>
<p>{ <br>
    &nbsp;&nbsp;&nbsp;&nbsp;"Hosts": "localhost:27017",<br>
    &nbsp;&nbsp;&nbsp;&nbsp; "Database": "my_database",<br>
    &nbsp;&nbsp;&nbsp;&nbsp; "Username": "dev1",<br>
    &nbsp;&nbsp;&nbsp;&nbsp; "Password": "password123",<br>
    &nbsp;&nbsp;&nbsp;&nbsp; "Collection": "cedict",<br>
    &nbsp;&nbsp;&nbsp;&nbsp; "Origin1": "http://localhost:4200",<br>
    &nbsp;&nbsp;&nbsp;&nbsp; "Origin2": "http://localhost:4200",<br>
}
</p>

<h2>Create Database</h2>
<p>Enter into the create Database folder and type go run main.go . This will create all the collections needed to run the api</p>


