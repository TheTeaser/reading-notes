# Reading Topics #34: API Deployment

## Django Settings Best Practices:

1. Keep settings in a separate module: 

    It is recommended to keep all your Django settings in a separate module, typically named settings.py or settings/__init__.py.

2. Use environment variables: 

    Store sensitive information and environment-specific settings (e.g., database credentials, API keys) as environment variables instead of hardcoding them in the settings file. The python-decouple library is often recommended to manage environment variables.

3. Split settings into multiple files: 

    Split your settings into multiple files based on their purpose or functionality. For example, you can have separate files for database settings, logging settings, third-party app settings, etc. Use the from .settings import * convention to import all the settings from the separate files into the main settings.py file.

---

## White Noise Library:

- WhiteNoise contributes to the efficient serving of static files and the steps to integrate it into a Django project:

    1. Gzip compression: WhiteNoise automatically compresses static files on the fly using Gzip compression. This reduces the file size and improves network transfer speeds, resulting in faster loading times for static assets.

    3. Caching: WhiteNoise sets appropriate HTTP cache headers for static files, allowing client-side caching in the browser. This means that once a static file is downloaded, subsequent requests for the same file can be served from the browser's cache, reducing server load and improving performance.

    3. No file system access: WhiteNoise serves static files directly from memory, without needing to access the file system for every request. This eliminates the overhead of file I/O operations, resulting in faster response times.

- Here are the steps to integrate WhiteNoise into a Django project:

    1. Install WhiteNoise.
    2. Configure Django settings.
    3. Configure web server.
    4. Collect static files: Run the collectstatic management command.
    5. Deploy the application. 

---

## Cross-Origin Resource Sharing (CORS): 

- The purpose of CORS in web applications is to control and restrict access to resources based on the domain or origin of the requesting client. By implementing and configuring CORS in a Django project, you can specify which domains are allowed to make cross-origin requests to your application and define the rules for handling those requests.

- To implement and configure CORS in a Django project, you can follow these steps:

    1. Install the django-cors-headers package.
    2. Configure Django settings.
    3. Configure additional CORS settings: Optionally, you can configure additional settings to customize the behavior of CORS.
    4. Test your application to ensure that the CORS configuration works as expected.
---