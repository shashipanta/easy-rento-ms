# EASY-RENTO

This is a muti-module **Spring Boot monorepo project** managed with **Maven**.
It contains multiple microservices and shared libraries organized under a single repository

---
## 📁 Project Structure
```
EASY-RENTO/
|-- pom.xml                 # Parent POM (manages modules and shared config)
|== config-server/          # Microservice for centralized config repository
|== discovery-server/       # Microservice for automatic discovery of services
|== api-gateway/            # Microservice for single entry point, route requests to services, rate-limiting
|-- shared/                 # Shared code and utilities used by services
|-- auth-service/           # Microservice for user and AUTH related operations
|-- notification-service    # Microservice for sending SMS / emails / real time notifications
```
---
## 🧪 Getting Started
To run the project, following prerequisites should be looked upon:

### prerequisites

- Java 17+
- Maven 3.8+
- IDE: Intellij IDEA (prefered) | VS Code

### Build All Modules

To clean and build all modules:

```bash
mvn clean install
```

---
## Development
Each service is a standalone Spring Boot Application so
```bash
cd auth-service
mvn spring-boot:run
```

### Run all Unit and Integration tests
```bash
mvn test
```

### Run test for a specific module
```bash
cd auth-service
mvn test
```

## 🤝 Contributing

1. Fork the repo
2. Commit your changes (git commit -m 'Add feature')
3. Push to the branch (git push origin feature/YourFeature)
4. Open a Pull Request

