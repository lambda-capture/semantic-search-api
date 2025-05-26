# Semantic-Search-API
🔎 RESTful API for Text-retrieval &amp; Semantic Search of Macro Data<br>
<a href="https://colab.research.google.com/github/lambda-capture/Semantic-Search-API/blob/main/API-notebook.ipynb" target="_blank">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"/>
</a>
<a href="https://lambda-capture.com/">
    <img src="https://img.shields.io/website-up-down-green-red/http/app.lambda-capture.com/.svg?label=API%20Status" alt="API Status"/>
</a>
<a href="https://github.com/lambda-capture/mcp-server">
    <img src="https://img.shields.io/website-up-down-green-red/http/lambda-mcp.azurewebsites.net/health-check/.svg?label=Remote%20MCP%20Server" alt="Remote MCP Server"/>
</a><br>
<a href="https://lambda-capture.com/waitlist" target="_blank"><strong>Join Waitlist (24h) for free API Key</strong></a> | 
<a href="https://lambda-capture.com" target="_blank">Visit our Website</a> | 
<a href="mailto:support@lambda-capture.com" target="_blank">Get in touch</a><br><br>
---
Waitlist sources are restricted to Central Banking Reports from the Federal Reserve, ECB, and Bank of England. These include key publications covering monetary policy decisions and judgments, market intelligence, forecasts, macroeconomic projections, and implementation notes. Each Waitlist account receives up to 1,000 free API requests. 
### Remote MCP Server
Visit our [Remote MCP Server](https://github.com/lambda-capture/mcp-server) for seamless tool call integration into AI models.
### Search Type: 
Cosine Similarity, Datetime Filters, Source Filters, Text size (in tokens), Type (chart, table, text). 
### Requests:
The API uses HTTP GET requests to retrieve data. The parameters for the request are passed in the body of the request as a JSON object.
### Response:
Response data is a JSON list (list of dictionaries). Error Response is a JSON dictionary with key "error"
### Curl CLI Example :
```bash

curl --request GET \
  --url "https://app.lambda-capture.com/semantic-search/" \
  --header "Content-Type: application/json" \
  --data '{
    "api_key": "your-api-key",
    "query_text": "Inflation expectations",
    "max_results": 1,
    "score": 0.75,
    "start_date": "2024-01-01",
    "end_date": "2024-12-31",
    "type": ["text", "table"],
    "source": ["Bank of England"]
  }'
```
Footnote: Replace \ with ^ when running outside UNIX systems

© 2024 Lambda Capture Limited (Registration Number 15845351) 52 Tabernacle Street, London, EC2A 4NJ - All rights reserved
