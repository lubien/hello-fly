# Hello Fly Monorepo

This monorepo contains minimal HTTP server applications implemented in various programming languages and frameworks. Each application listens on the PORT environment variable and returns a simple hello message.

## Project Structure

```
hello-fly/
├── .gitignore
├── README.md
├── hello-fly-nodejs-16/
├── hello-fly-nodejs-18/
├── hello-fly-nodejs-20/
├── hello-fly-nodejs-22/
├── hello-fly-python-2/
├── hello-fly-python-3/
├── hello-fly-python-3.9/
├── hello-fly-dotnet-core-3.1/
├── hello-fly-dotnet-5/
├── hello-fly-dotnet-6/
├── hello-fly-dotnet-7/
├── hello-fly-dotnet-8/
├── hello-fly-java-spring-gradle/
└── hello-fly-java-spring-maven/
```

## Projects

### Node.js Applications

#### hello-fly-nodejs-16
- **Technology**: Node.js 16.x
- **Run**: `cd hello-fly-nodejs-16 && npm start`
- **Default Port**: 3000

#### hello-fly-nodejs-18
- **Technology**: Node.js 18.x
- **Run**: `cd hello-fly-nodejs-18 && npm start`
- **Default Port**: 3000

#### hello-fly-nodejs-20
- **Technology**: Node.js 20.x
- **Run**: `cd hello-fly-nodejs-20 && npm start`
- **Default Port**: 3000

#### hello-fly-nodejs-22
- **Technology**: Node.js 22.x
- **Run**: `cd hello-fly-nodejs-22 && npm start`
- **Default Port**: 3000

### Python Applications

#### hello-fly-python-2
- **Technology**: Python 2.x
- **Run**: `cd hello-fly-python-2 && python server.py`
- **Default Port**: 3000

#### hello-fly-python-3
- **Technology**: Python 3.x
- **Run**: `cd hello-fly-python-3 && python3 server.py`
- **Default Port**: 3000

#### hello-fly-python-3.9
- **Technology**: Python 3.9
- **Run**: `cd hello-fly-python-3.9 && python3.9 server.py`
- **Default Port**: 3000

### .NET Applications

#### hello-fly-dotnet-core-3.1
- **Technology**: .NET Core 3.1
- **Run**: `cd hello-fly-dotnet-core-3.1 && dotnet run`
- **Default Port**: 3000

#### hello-fly-dotnet-5
- **Technology**: .NET 5
- **Run**: `cd hello-fly-dotnet-5 && dotnet run`
- **Default Port**: 3000

#### hello-fly-dotnet-6
- **Technology**: .NET 6 (Minimal API)
- **Run**: `cd hello-fly-dotnet-6 && dotnet run`
- **Default Port**: 3000

#### hello-fly-dotnet-7
- **Technology**: .NET 7 (Minimal API)
- **Run**: `cd hello-fly-dotnet-7 && dotnet run`
- **Default Port**: 3000

#### hello-fly-dotnet-8
- **Technology**: .NET 8 (Minimal API)
- **Run**: `cd hello-fly-dotnet-8 && dotnet run`
- **Default Port**: 3000

### Java Spring Boot Applications

#### hello-fly-java-spring-gradle
- **Technology**: Java 11, Spring Boot 2.7.14, Gradle
- **Build**: `cd hello-fly-java-spring-gradle && ./gradlew build`
- **Run**: `cd hello-fly-java-spring-gradle && ./gradlew bootRun`
- **Default Port**: 3000

#### hello-fly-java-spring-maven
- **Technology**: Java 11, Spring Boot 2.7.14, Maven
- **Build**: `cd hello-fly-java-spring-maven && ./mvnw package`
- **Run**: `cd hello-fly-java-spring-maven && ./mvnw spring-boot:run`
- **Default Port**: 3000

## Environment Variables

All applications respect the `PORT` environment variable. If not set, they default to port 3000.

Example:
```bash
PORT=8080 npm start
PORT=8080 python server.py
PORT=8080 dotnet run
PORT=8080 ./gradlew bootRun
PORT=8080 ./mvnw spring-boot:run
```

## Prerequisites

- **Node.js applications**: Respective Node.js versions installed
- **Python applications**: Python 2 or Python 3 installed as required
- **.NET applications**: .NET SDK for the respective version installed
- **Java applications**: Java 11 or higher installed

## Testing

Once running, you can test any server with:
```bash
curl http://localhost:3000
```

Each server will respond with a greeting message indicating its technology stack.

## Git Ignore Files

Each project has its own `.gitignore` file tailored to its specific technology stack, and there's also a root `.gitignore` file that covers common patterns across all projects.