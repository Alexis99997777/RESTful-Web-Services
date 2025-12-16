<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>RESTful Web Services with Spring Boot</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            line-height: 1.6;
            margin: 40px;
            background-color: #ffffff;
            color: #333;
        }
        h1, h2, h3 {
            color: #2c3e50;
        }
        h1 {
            border-bottom: 2px solid #eaeaea;
            padding-bottom: 10px;
        }
        code {
            background-color: #f4f4f4;
            padding: 3px 6px;
            border-radius: 4px;
            font-size: 0.95em;
        }
        pre {
            background-color: #f4f4f4;
            padding: 15px;
            overflow-x: auto;
            border-radius: 6px;
        }
        ul {
            margin-left: 20px;
        }
        li {
            margin-bottom: 6px;
        }
        .section {
            margin-top: 40px;
        }
        .footer {
            margin-top: 60px;
            font-size: 0.9em;
            color: #666;
            border-top: 1px solid #eaeaea;
            padding-top: 20px;
        }
    </style>
</head>

<body>

<h1>RESTful Web Services with Spring Boot</h1>

<p>
This project is a <strong>RESTful Web Service</strong> built using
<strong>Spring Boot</strong>. It was created to practice and demonstrate
core backend concepts such as request mapping, dependency injection,
validation, exception handling, and running a web service as a
standalone application.
</p>

<p>
The application follows a clean, layered architecture and uses
Spring Boot best practices, including constructor-based dependency
injection and centralized exception handling.
</p>

<div class="section">
    <h2>🚀 Features Implemented</h2>

    <h3>Project Setup</h3>
    <ul>
        <li>Create a Spring Boot project using Spring Boot Initializr</li>
        <li>Run the web service as a standalone application (embedded Tomcat)</li>
    </ul>

    <h3>REST Controller & Request Mapping</h3>
    <ul>
        <li><code>@RestController</code> and <code>@RequestMapping</code></li>
        <li>Handle HTTP methods:
            <ul>
                <li>GET</li>
                <li>POST</li>
                <li>PUT</li>
                <li>DELETE</li>
            </ul>
        </li>
    </ul>

    <h3>Request Data Handling</h3>
    <ul>
        <li>Read path variables using <code>@PathVariable</code></li>
        <li>Read query parameters using <code>@RequestParam</code></li>
        <li>Support required and optional request parameters</li>
        <li>Read HTTP POST request body using <code>@RequestBody</code></li>
    </ul>

    <h3>Validation</h3>
    <ul>
        <li>Validate request body using <code>@Valid</code></li>
        <li>Bean validation annotations (e.g. <code>@NotNull</code>, <code>@Size</code>)</li>
    </ul>

    <h3>Response Handling</h3>
    <ul>
        <li>Return Java objects as HTTP responses</li>
        <li>Automatic conversion to JSON / XML</li>
        <li>Set HTTP response status codes using
            <code>ResponseEntity</code> and <code>@ResponseStatus</code>
        </li>
    </ul>

    <h3>Temporary Data Storage</h3>
    <ul>
        <li>Store user data temporarily using an in-memory data structure (e.g. Map)</li>
    </ul>

    <h3>Exception Handling</h3>
    <ul>
        <li>Global exception handling</li>
        <li>Custom error message objects</li>
        <li>Handle generic, specific, and custom-defined exceptions</li>
        <li>Catch multiple exceptions with a single handler method</li>
    </ul>

    <h3>Dependency Injection</h3>
    <ul>
        <li>Create a service layer using <code>@Service</code></li>
        <li>Use Spring IoC container for dependency management</li>
        <li>Constructor-based dependency injection</li>
    </ul>
</div>

<div class="section">
    <h2>🏗 Project Architecture</h2>

    <pre>
Controller Layer
    ↓
Service Layer
    ↓
Utility / Temporary Data Storage
    </pre>

    <ul>
        <li><strong>Controller Layer</strong>: Handles HTTP requests and responses</li>
        <li><strong>Service Layer</strong>: Contains business logic</li>
        <li><strong>Utility Classes</strong>: Shared helper logic (e.g. ID generation)</li>
    </ul>
</div>

<div class="section">
    <h2>🧠 Key Concepts Practiced</h2>
    <ul>
        <li>RESTful API design</li>
        <li>Spring Beans and IoC Container</li>
        <li>Dependency Injection (Field vs Constructor-based)</li>
        <li>Request lifecycle vs Bean lifecycle</li>
        <li>Standalone Spring Boot application execution</li>
        <li>Separation of concerns</li>
    </ul>
</div>

<div class="section">
    <h2>▶️ Running the Application</h2>

    <h3>Option 1: Run from IDE</h3>
    <p>
        Run the main Spring Boot application class directly from your IDE
        (Eclipse or IntelliJ).
    </p>

    <h3>Option 2: Run as Standalone Application</h3>

    <p>Build the project:</p>
    <pre>
mvn clean package
    </pre>

    <p>Run the generated JAR file:</p>
    <pre>
java -jar target/your-application-name.jar
    </pre>

    <p>
        The application will start on:
        <code>http://localhost:8080</code>
    </p>
</div>

<div class="section">
    <h2>🧪 Testing the API</h2>
    <p>You can test the API using:</p>
    <ul>
        <li>Postman</li>
        <li>curl</li>
        <li>Web browser (for GET requests)</li>
    </ul>

    <p>Example request:</p>
    <pre>
GET http://localhost:8080/users/{userId}
    </pre>
</div>

<div class="section">
    <h2>📦 Technologies Used</h2>
    <ul>
        <li>Java</li>
        <li>Spring Boot</li>
        <li>Spring Web</li>
        <li>Maven</li>
        <li>Embedded Tomcat</li>
        <li>JSON / XML serialization</li>
    </ul>
</div>

<div class="section">
    <h2>📚 Learning Purpose</h2>
    <p>
        This project was created for learning and practicing Spring Boot
        RESTful web services, with a focus on understanding request handling,
        dependency injection, exception handling, and application structure.
    </p>
</div>

<div class="footer">
    <p><strong>Author:</strong> Alexis</p>
</div>

</body>
</html>
