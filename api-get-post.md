#Prompt:
Write an API reference page in Markdown for GET /posts/{id}.
 Use ONLY the facts below. If something is missing, write [NEEDS INFO].
 Do not invent parameters, status codes, or limits.
Facts:
 Method: GET
 Endpoint: /posts/{id}
 Parameter: id (1), id(9999)
 Response fields: id, title, body, userId
 Success status code: [200]
 Error status code (id 9999): [404]
 Example response : 200

Output
GET /posts/{id}
Returns a single post by its ID.
Request
http
GET /posts/{id}
Base URL: [NEEDS INFO]
Authentication: [NEEDS INFO]
Rate limits: [NEEDS INFO]
----
Path parameters				
| Name | Type           | Required       | Description    | Example values |
| :--- | :------------- | :------------- | :------------- | :------------- |
| id   | \[NEEDS INFO\] | \[NEEDS INFO\] | \[NEEDS INFO\] | 1, 9999        |

Example request
curl -X GET "[BASE_URL]/posts/1"
----
Response

| Field  | Type           | Description    |
| :----- | :------------- | :------------- |
| id     | \[NEEDS INFO\] | \[NEEDS INFO\] |
| title  | \[NEEDS INFO\] | \[NEEDS INFO\] |
| body   | \[NEEDS INFO\] | \[NEEDS INFO\] |
| userId | \[NEEDS INFO\] | \[NEEDS INFO\] |

-----
Status codes

| Code | Meaning | Example id |
| :--- | :--- | :--- |
| 200 | Success | 1 |
| 404 | [NEEDS INFO] | 9999 |
----


Example response
Status: 200
json
[NEEDS INFO]
Example error response
Status: 404
json
[NEEDS INFO]

Open items
“Example response: 200” gives a status code but no body. I left the JSON blocks as [NEEDS INFO].
The meaning of 404 and its response body are not stated.
Parameter type, required status, and all field types and descriptions are missing.
:warning: Verify: the 404 for id 9999 comes from your facts. Confirm it against the live API.

