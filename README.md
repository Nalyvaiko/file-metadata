# File Metadata Microservice

A Node.js/Express microservice that accepts file uploads and returns metadata including name, type, and size.

## Features

- Accepts single file upload via form
- Responds with file metadata:
  - `name`: original filename
  - `type`: MIME type
  - `size`: file size in bytes
- File size limit: 10MB
- Rate limiting (100 requests per 15 minutes)
- CORS support
- Security headers via Helmet
- Graceful shutdown handling
- 404 and 500 error handling