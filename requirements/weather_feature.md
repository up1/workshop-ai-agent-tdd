# Weather Feature
* Retrieves the current weather for a specified city

## API Specification
* Endpoint: POST /api/skills/weather
* Description: Fetches weather for an agent workflow.
* Request Body: { "city": "string" }
* Responses: 
  * 200 OK: { "weather": "sunny" }
  * 400 Bad Request: { "error": "City is required" }

## Input validation in table format 
| Field | Type   | Required | Description                  |
|-------|--------|----------|------------------------------|
| city  | string | yes      | The name of the city to fetch weather for |

## Output validation in table format 
| Field   | Type   | Required | Description                  |
|---------|--------|----------|------------------------------|
| weather | string | no       | The current weather for the specified city |
| error   | string | no       | The error message if the request was invalid |