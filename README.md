<body>

<h1>RESTful Web Services with Spring Boot</h1>

<p>
This project is a <strong>RESTful Web Service</strong> built with
<strong>Spring Boot</strong> to practice core backend concepts such as
request mapping, dependency injection, validation, and exception handling.
</p>

<h2>🚀 Features</h2>
<ul>
    <li>Spring Boot standalone web application</li>
    <li>RESTful APIs using <code>@RestController</code></li>
    <li>HTTP methods: GET, POST, PUT, DELETE</li>
    <li>Path variables and query parameters</li>
    <li>Request body handling with <code>@RequestBody</code></li>
    <li>Validation using <code>@Valid</code></li>
    <li>Global and custom exception handling</li>
    <li>Service layer with constructor-based dependency injection</li>
</ul>

<h2>🏗 Architecture</h2>
<pre>
Controller
   ↓
Service
   ↓
Utility / In-memory Storage
</pre>

<h2>▶️ Run the Application</h2>

<p><strong>Run from IDE:</strong></p>
<p>Run the Spring Boot main class from Eclipse or IntelliJ.</p>

<p><strong>Run as standalone application:</strong></p>
<pre>
mvn clean package
java -jar target/your-application-name.jar
</pre>

<p>
Application runs at:
<code>http://localhost:8080</code>
</p>

<h2>🧪 Test</h2>
<p>You can test the APIs using Postman, curl, or a web browser.</p>

<pre>
GET http://localhost:8080/users/{userId}
</pre>

<h2>📦 Tech Stack</h2>
<ul>
    <li>Java</li>
    <li>Spring Boot</li>
    <li>Spring Web</li>
    <li>Maven</li>
    <li>Embedded Tomcat</li>
</ul>

<hr>

<p><strong>Author:</strong> Alexis</p>

</body>

