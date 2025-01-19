# Positive Testing Postman Collection

This repository contains a Postman collection for positive testing of project management APIs. The collection includes tests for creating, updating, and deleting projects, ensuring proper functionality and performance.

---

## Collection Overview

The collection contains the following requests:

1. **Create a New Project**  
   - Endpoint: `POST {{base url}}/{{api v2}}/add_project`
   - Body Parameters:
     - `name`: Name of the project.
     - `announcement`: Announcement text for the project.
   - Tests:
     - Verify the status code is `200`.
     - Ensure the response time is less than `500ms`.
     - Validate the returned project name and announcement.

2. **Update Project**  
   - Endpoint: `POST {{base url}}/{{api v2}}/update_project/{{projectID}}`
   - Body Parameters:
     - `update_project_name`: New name for the project.
     - `update_announcement`: New announcement text.
   - Tests:
     - Verify the status code is `200`.
     - Ensure the response time is less than `400ms`.
     - Validate the updated project name and announcement.

3. **Delete Project**  
   - Endpoint: `POST {{base url}}{{api v2}}/delete_project/{{projectID}}`
   - Tests:
     - Verify the status code is `200`.
     - Ensure the response time is less than `400ms`.

