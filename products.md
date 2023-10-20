# Assignment: Golang Product Versioning/Revisions

## Objective:

Develop a comprehensive system in Golang that manages the revisions of products on a shopping site. As products evolve, their attributes might change, including price, description, and more. It's essential to maintain a history of these revisions for analysis and traceability purposes.

---

## Core Requirements:

### 1. Product Model:

- Unique ID
- Name
- Description
- Price
- Image URL
- Timestamp of creation and update
- Any other attributes you deem necessary

### 2. Revision Model:

- Linked to Product Model
- Revision Number
- Attributes that changed
- Previous Value
- New Value
- Timestamp of revision

### 3. APIs:

- Add a new product
- Update an existing product
- Fetch all revisions of a product
- Fetch details of a specific product (latest attributes)
- Fetch details of a specific product for a specific revision number

### 4. Persistence:

- Implement a database (can be SQL or NoSQL, based on your preference) to persist product and revision details. Usage of ORMs or direct queries is up to you.

### 5. Unit Tests:

- Unit tests covering the critical functions and methods.

### 6. Documentation:

- A comprehensive README detailing the system's architecture, APIs, setup instructions, and any other relevant information.

---

## Bonus Points:

### 1. Docker:

Containerize the application using Docker, providing a `Dockerfile` and a `docker-compose` file for easier setup and deployment.

### 2. Pagination:

Introduce pagination in the API that fetches all product revisions.

### 3. Event-driven architecture:

Instead of saving revisions directly upon product update, produce an event and consume it to save the revision, simulating a more real-world microservices scenario.

### 4. Integration Tests:

- Integration tests covering the APIs and database operations.

### 6. **Monitoring with Prometheus**:

Implement monitoring for your application using Prometheus. Integrate with the [Prometheus Go client library](https://github.com/prometheus/client_golang) to set up custom metrics that can help in monitoring the performance and health of your application.

### 7. **Distributed Tracing with OpenTracing**:

Integrate [OpenTracing](https://opentracing.io/) for distributed tracing. This should provide insights into the journey of requests as they travel across various components of the system, helping in diagnosing performance bottlenecks and understanding system behavior.

---

## Technology Stack Suggestions:

- **Backend:** Golang
- **Database:** PostgreSQL, MySQL, MongoDB, or any other of your preference.
- **Testing:** Go's built-in testing package or any other testing library/framework you're comfortable with.
- **API Documentation:** Swagger, Postman, or any other tool you prefer.
- **Containerization:** Docker

---

## Submission:

- Share the codebase with us by pushing it to a public GitHub repository.
- Ensure that your commit history is clean and commits are meaningful, showing the progression of the project.
- Make sure that the README is comprehensive and helps any developer set up the project without any hassles.

---

## Evaluation Criteria:

1. **Functionality:** Does the application perform all the defined requirements?
2. **Code Quality:** Is the code modular, readable, and maintainable?
3. **Testing:** Are all the tests passing? Is there a good coverage of unit and integration tests?
4. **Documentation:** Is the documentation clear and comprehensive?
5. **Bonus Points:** Have any of the bonus points been achieved?

---

Wishing you the best of luck! We look forward to reviewing your solution.
