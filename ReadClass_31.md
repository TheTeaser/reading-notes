# Reading Topics #31: Django REST Framework & Docker:

## Docker Container:

*The key components of a Docker container are as follows:*


- Docker Image: A Docker image is a read-only template that contains the application and all its dependencies, including the operating system, libraries, and runtime environment. 

- Containerization: Containers are instances of Docker images that are created and run on a host system.

- Docker Engine: The Docker Engine is the runtime environment that runs and manages Docker containers.

*The key benefits of Docker containers in streamlining development and deployment of applications are:*

- Portability: Docker containers encapsulate the application and its dependencies, making them highly portable across different environments. Developers can build and test applications locally in containers and then deploy the same containers in production, ensuring consistent behavior and eliminating the "works on my machine" problem.

- Isolation: Containers provide process-level isolation, ensuring that each application runs in its own isolated environment. This isolation prevents conflicts between applications and allows multiple applications to run on the same host without interference.

- Efficiency: Docker containers are lightweight and share the host system's operating system kernel, resulting in reduced resource usage and improved efficiency. Containers start quickly, scale easily, and require fewer resources compared to traditional virtual machines.

---

## How to build a website using Django:

1. Set up Django Project.
2. Create Django app and define the models.
3. Create the database tables and degind the URL patterns.
4. Implement views and templates and import the rest of your website with the wanted functionaliaties.
---
## Django V.S. Django REST frameworks:


*Django and Django REST framework (DRF) are both popular frameworks for web development in Python, but they serve different purposes. Here are the primary differences between Django and Django REST framework:*

1. Web Application vs. API Development:

    - Django: Django is a high-level web framework primarily used for building full-stack web applications. It provides a robust set of tools and features for handling various aspects of web development, such as URL routing, database ORM, forms, authentication, templating, and more.
    - Django REST framework: DRF is an extension of Django that specifically focuses on building APIs (Application Programming Interfaces). It provides additional features and functionality to simplify the development of RESTful APIs, including support for serialization, authentication, permissions, viewsets, and API documentation.
2. Serialization and API Rendering:

    - Django: Django includes a serialization framework that allows converting Django models or querysets to and from different formats like JSON, XML, or YAML. However, the serialization capabilities in Django are more limited compared to DRF.
    - Django REST framework: DRF provides a powerful serialization framework that allows developers to define serializers for translating complex data types, such as models, into Pythonic data types that can be easily rendered into various formats. DRF supports serialization of relationships, nested data structures, and complex validation.
3. API Views and Viewsets:

    - Django: Django uses regular views, typically defined as Python functions or class-based views, to handle HTTP requests and generate responses. Developers have more control over the request/response flow but need to handle request parsing, serialization, and response rendering manually.
    - Django REST framework: DRF introduces the concept of viewsets and generic views, which provide higher-level abstractions for handling common API operations. Viewsets map CRUD (Create, Retrieve, Update, Delete) actions to specific HTTP methods automatically. Generic views provide pre-built functionality for common API views, such as listing objects, creating objects, or retrieving a single object.
4. Authentication and Permissions:

    - Django: Django offers various authentication mechanisms, such as session-based authentication, token-based authentication, and integration with external authentication providers. It also provides flexible permission controls, allowing developers to define access restrictions at the view level.
    - Django REST framework: DRF builds on Django's authentication and permission system and provides additional authentication classes and permission classes specific to API development. It offers ready-to-use authentication options like token authentication, JSON Web Tokens (JWT), and OAuth2. DRF also includes permission classes for implementing authorization rules, such as allowing read-only access, requiring authentication, or custom permission logic.
5. API Documentation:

    - Django: Django does not provide built-in tools for generating API documentation, although there are third-party libraries available for this purpose.
    - Django REST framework: DRF includes a powerful and customizable API documentation tool called "Browsable API." It generates interactive HTML documentation that allows developers to browse and test API endpoints directly from the web browser. DRF also supports integration with popular documentation tools like Swagger and OpenAPI.
---