
# Spring Boot Cloud Config

This repository contains an example project showcasing the usage of Spring Cloud Config with a Spring Boot application. It demonstrates how to centralize and manage the configuration of multiple microservices using Spring Cloud Config Server.

## Prerequisites

Before running this example, ensure that you have the following installed:

- Java Development Kit (JDK) 17 or later
- Maven
- Spring 3.0

## Getting Started

To get started with this example, follow these steps:

1. Clone the repository:

   ```shell
   git clone https://github.com/peirisabhi/springboot-cloud-config.git
   ```

2. Navigate to the project directory:

   ```shell
   cd springboot-cloud-config
   ```

3. Build the project using Maven:

   ```shell
   mvn clean package
   ```

4. Run the application:

   ```shell
   mvn spring-boot:run
   ```

5. The application should now be running locally. You can access the application endpoints defined in the example.

## Configuration

This example demonstrates the usage of Spring Cloud Config Server. The configuration files for the microservices can be found in the `config-repo` directory. The `application.properties` file in the Config Server project (`springboot-cloud-config-server`) contains the configuration for the location of the configuration files:

```properties
spring.cloud.config.server.git.uri=file:///${user.dir}/config-repo
```

By default, the example uses a local Git repository (`file:///${user.dir}/config-repo`) to store the configuration files. You can modify this configuration to use a remote Git repository or any other supported backend for storing the configuration.

## Usage

This example project includes two sample microservices (`springboot-cloud-config-client` and `springboot-cloud-config-server`) to demonstrate the usage of Spring Cloud Config. The `springboot-cloud-config-client` microservice retrieves its configuration from the Config Server.

Feel free to explore the code and modify it to suit your needs. The code is extensively documented to help you understand each step and the purpose of different components.

## Contributing

Contributions to this project are welcome. If you find any issues or have ideas for improvements, please open an issue or submit a pull request.


## Contact

For any questions or feedback, please contact:


Abhishek Peiris
- Email: abhishekpeiris9@gmail.com
- GitHub: [@peirisabhi](https://github.com/peirisabhi)
