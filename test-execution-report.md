# Test Execution Report

## 1. Project Details

- **Project:** REST API Testing with Postman
- **API under test:** JSONPlaceholder
- **Base URL:** https://jsonplaceholder.typicode.com
- **Tool:** Postman
- **Test data and cases:** `test-cases.xlsx`
- **Collection:** `Rest API testing.postman_collection.json`
- **Execution date:** Enter the date you ran the tests

## 2. Objective

The objective of this test run is to validate selected JSONPlaceholder endpoints using Postman. Checks cover response status codes, response body structure, expected field values, query-parameter filtering, and a negative scenario.

## 3. Execution Summary

Fill in this summary after running all seven requests and reviewing their Test Results.

| Metric | Result |
|---|---|
| Total requests tested | 7 planned |
| Passed requests | Enter verified count |
| Failed requests | Enter verified count |
| Blocked / not run | Enter count |
| Overall result | Complete after execution |

**Important:** Count a request as passing only after you have run it and confirmed its assertions pass. A request may contain multiple assertions.

## 4. Test Execution Details

| ID | Scenario | Method and endpoint | Expected result | Actual result | Status |
|---|---|---|---|---|---|
| TC-001 | Retrieve a post | GET `/posts/1` | `200 OK`; expected post fields are present | Fill from Postman | Not recorded |
| TC-002 | Filter posts | GET `/posts?userId=1` | `200 OK`; response is an array and each post has `userId = 1` | Fill from Postman | Not recorded |
| TC-003 | Negative test | GET `/posts/999999` | `404 Not Found`; empty JSON object | Fill from Postman | Not recorded |
| TC-004 | Submit a new post | POST `/posts` | `201 Created`; response matches submitted values and includes an ID | Fill from Postman | Not recorded |
| TC-005 | Replace a post | PUT `/posts/1` | `200 OK`; response has expected updated fields | Fill from Postman | Not recorded |
| TC-006 | Partially update a post | PATCH `/posts/1` | `200 OK`; title is updated and expected fields remain present | Fill from Postman | Not recorded |
| TC-007 | Delete a post | DELETE `/posts/1` | Record and validate the status/body actually returned by the API | Fill from Postman | Not recorded |

Replace **Not recorded** with **PASS** or **FAIL** only after you run each request and check its Test Results. If a request cannot be sent because of a network or tool error, record it as **BLOCKED** rather than FAIL.

## 5. Issues and Observations

- JSONPlaceholder is a demo API. Write operations such as POST, PUT, PATCH, and DELETE are simulated; responses do not demonstrate persistent database changes.
- Record any unexpected status codes, assertion failures, or request execution errors here.
- For each failure, include the request name, expected result, actual result, and what you did to investigate it.

## 6. Conclusion

Complete this section after all requests have been executed. Summarize the number of passed, failed, and blocked requests, and mention any unresolved issues. Do not claim that all tests passed unless the Postman results confirm it.
