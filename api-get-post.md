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
| 404 | Not Found | 9999 |
----


## Example response
### Status: 200
```json
200
```

## Example error response
### Status: 404
```json
404
```

