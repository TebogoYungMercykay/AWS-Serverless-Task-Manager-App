# Architecture

The application follows a serverless microservices architecture:

1. **Frontend (React)** communicates with API Gateway
2. **API Gateway** routes requests to appropriate Lambda functions
3. **Lambda Functions** handle business logic and database operations
4. **DynamoDB** stores task data persistently
5. **Auth0** manages user authentication and JWT tokens

![Serverless](./images/serverless-framework.png)

## Application Screenshots

### Landing Page

*Screenshot showing the application's landing page and initial user interface*

![Landing Page](images/screenshots/image-11.png)

### Authentication Flow

*Screenshot demonstrating the Auth0 login process*

![Auth0 Login](images/screenshots/image-12.png)

### Task Dashboard

*Screenshot of the main task management interface after authentication*

![Task Dashboard](images/screenshots/image-13.png)

### Task Creation

*Screenshot showing the create new task functionality*

![Create Task](images/screenshots/image-19.png)

### Task Management

*Screenshot demonstrating task editing, completion, and deletion features*

![Create Task](images/screenshots/image-16.png)

![Create Task](images/screenshots/image-17.png)

![Task Management](images/screenshots/image-20.png)

![Task Management](images/screenshots/image-21.png)

![Task Management](images/screenshots/image-22.png)

## API Endpoints

The serverless backend exposes the following REST API endpoints:

```
GET    /tasks          - Retrieve all tasks for authenticated user
POST   /tasks          - Create a new task
PUT    /tasks/{id}     - Update an existing task
DELETE /tasks/{id}     - Delete a task
GET    /tasks/{id}     - Retrieve a specific task
```

## Deployment Proof

### Serverless Login

![Serverless](images/screenshots/image-01.png)

### Serverless Framework Deployment

*Screenshot of successful serverless deployment output*

![Serverless Deploy](images/screenshots/image-28.png)

![Serverless Deploy](images/screenshots/image-02.png)

![Serverless Deploy](images/screenshots/image-03.png)

![Serverless Deploy](images/screenshots/image-04.png)

### AWS Console Screenshots

*Screenshots showing successful deployment in AWS Console*

![Lambda Functions](images/screenshots/image-05.png)

#### Lambda Functions

![Lambda Functions](images/screenshots/image-31.png)

#### API Gateway

![API Gateway](images/screenshots/image-10.png)

![API Gateway](images/screenshots/image-30.png)

#### s3 Bucket

![s3 Bucket](images/screenshots/image-08.png)

![s3 Bucket](images/screenshots/image-09.png)

#### CloudFormation Stack

![CloudFormation Stack](images/screenshots/image-06.png)

### Auth0 Configuration

*Screenshot showing Auth0 application configuration*

![Auth0 Config](images/screenshots/image-12.png)

![Auth0 Config](images/screenshots/image-27.png)

## Testing and Functionality

### API Testing

*Screenshots showing API endpoints usage*

![API Testing](images/screenshots/image-25.png)

### Browser Network Tab

*Screenshot of browser developer tools showing successful API calls*

![Network Tab](images/screenshots/image-30.png)

![Network Tab](images/screenshots/image-31.png)

## Setup Instructions

For detailed setup and deployment instructions, refer to the [Setup Manual](./manual.pdf).

---
