# REST API Testing with Postman

## Project Overview

This project demonstrates beginner-level REST API testing using Postman and the JSONPlaceholder demo API. It includes requests for retrieving, filtering, creating, replacing, partially updating, and deleting posts, along with JavaScript assertions to validate response status codes and response data.

**Base URL:** https://jsonplaceholder.typicode.com

> Note: JSONPlaceholder is a demo API. Write operations such as POST, PUT, PATCH, and DELETE are simulated and are not permanently saved to a real database.

## Tools and Technologies

- **Postman** — sending API requests and running tests
- **JavaScript assertions in Postman** — validating status codes and response data
- **JSONPlaceholder** — demo REST API used for practice
- **Microsoft Excel** — documenting test scenarios and results

## Test Scenarios

| Test scenario | Method | Endpoint | Purpose |
|---|---|---|---|
| Retrieve a post | GET | `/posts/1` | Check a single post and its required fields |
| Filter posts | GET | `/posts?userId=1` | Check that returned posts belong to user 1 |
| Negative test | GET | `/posts/999999` | Check the response for a nonexistent post |
| Submit a new post | POST | `/posts` | Validate the create response and submitted data |
| Replace a post | PUT | `/posts/1` | Validate the updated post response |
| Partially update a post | PATCH | `/posts/1` | Validate the changed title and remaining fields |
| Delete a post | DELETE | `/posts/1` | Validate the deletion response |

## What Is Tested?

- HTTP response status codes
- Response body structure and data
- Required fields and expected values
- Query-parameter filtering
- A negative scenario using a nonexistent post
- Basic automated assertions using Postman's JavaScript test scripts

## Project Files

- `Rest API testing.postman_collection.json` — exported Postman collection containing the requests and scripts
- `test-cases.xlsx` — test-case spreadsheet with scenarios, expected results, actual results, and status

## How to Run

1. Download and install Postman.
2. Import the exported Postman collection JSON file.
3. Open a request in the collection.
4. Click **Send** to execute the request.
5. Review the response status and body.
6. Open **Test Results** to review the assertions.

## Learning Outcomes

Through this project, I practised sending common HTTP methods, working with query parameters and JSON request bodies, checking API responses, and using JavaScript assertions in Postman.

## Limitations

JSONPlaceholder is intended for practice and testing. Successful POST, PUT, PATCH, or DELETE responses do not mean data was permanently created, changed, or removed.

---

**Project type:** Beginner REST API testing practice project  
**Author:** Abhinandan Kumar Sharma
