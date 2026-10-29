# Prompt:
Write an API reference page in Markdown for GET /posts/{id}.
 Use ONLY the facts below. If something is missing, write [NEEDS INFO].
 Do not invent parameters, status codes, or limits.

Facts:
- Method: GET
 - Endpoint: /posts/{id}
 - Parameter: id (1), id(9999)
- Response fields: id, title, body, userId
 Success status code: [200]
- Error status code (id 9999): [404]
- Example response : 200

# Output
## GET /posts/{id}

Returns a single post by its ID.

## Request

```http
GET /posts/{id}
```

- **Base URL:** https://jsonplaceholder.typicode.com
- **Authentication:** [NEEDS INFO]
- **Rate limits:** [NEEDS INFO]

---
## Path parameters				
| Name | Type           | Required       | Description    | Example values |
| :--- | :------------- | :------------- | :------------- | :------------- |
| id   | integer | Yes | ID of the post to return | 1, 9999        |
---

## Example request
```bash
curl -X GET "https://jsonplaceholder.typicode.com/posts/1"
```
---
## Response

| Field  | Type           | Description    |
| :----- | :------------- | :------------- |
| id     | integer| ID of the post |
| title  | string | Title of the post |
| body   | string | Text of the post |
| userId | string | ID of a user associated with the post |

-----
## Status codes

| Code | Meaning | Example id |
| :--- | :--- | :--- |
| 200 | Success | 1 |
| 404 | [NEEDS INFO] | 9999 |
----


## Example response
### Status: 200
```json
[NEEDS INFO]
```

## Example error response
### Status: 404
```json
[NEEDS INFO]
```

## Open items
- “Example response: 200” gives a status code but no body. I left the JSON blocks as [NEEDS INFO].
- The meaning of 404 and its response body are not stated.
- Parameter type, required status, and all field types and descriptions are missing.
- :warning: Verify: the 404 for id 9999 comes from your facts. Confirm it against the live API.

