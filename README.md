🚀 AI Image Background Remover System
📌 Overview

VisionClean is a Spring Boot-based backend service that allows users to upload images and process them asynchronously for AI-powered background removal. The system integrates with an external AI API and manages processing status efficiently using a scalable layered architecture.

🛠 Tech Stack

-Java

-Spring Boot

-Spring Web (REST APIs)

-Spring Data JPA

-MySQL

-Maven

⚙️ Key Features

-RESTful API for image upload

-Asynchronous background removal processing

-External AI API integration

-Image status tracking (PENDING, COMPLETED, FAILED)

-Exception handling and timeout management

-Scalable layered architecture (Controller → Service → Repository)

🏗 Architecture

-The project follows a layered architecture:

-Controller Layer → Handles HTTP requests and responses
-Service Layer → Business logic and external API calls
-Repository Layer → Database operations using JPA

This ensures clean code structure, maintainability, and scalability.

🔄 Workflow

-User uploads an image via REST API.

-Image metadata is stored in MySQL with status PENDING.

-Background removal process is triggered asynchronously.

-External AI API processes the image.

-Status updates to COMPLETED or FAILED.

-User can check processing status via API.

📊 Database Design

The system stores:

-Image ID

-File path / URL

-Processing status

-Timestamp

This allows proper tracking of concurrent image requests.

🚀 How to Run

-Clone the repository

-Configure MySQL database in application.properties

-Add external AI API credentials

-Run the Spring Boot application

🎯 Learning Outcomes

-Implemented asynchronous processing in Spring Boot

-Integrated third-party AI APIs

-Managed concurrency and status tracking

-Designed clean layered architecture
