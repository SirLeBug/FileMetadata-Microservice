## Overview

This is a simple File Metadata Microservice built with Node.js, Express, and Multer. It allows users to upload a file via a POST request and returns metadata about the uploaded file including its name, type, and size.

Users can interact with the service by submitting a file through a form, and the service responds with a JSON object describing the file.

---

## About

This project is part of the [freeCodeCamp](https://www.freecodecamp.org/) Backend Development and APIs curriculum. It helped me practice working with file uploads in Node.js using the Multer middleware, handling multipart form data, and extracting file metadata.

---

## Usage

- **POST** `/api/fileanalyse` — Upload a single file using form-data with the key `upfile`.  
  Returns a JSON response with the uploaded file's metadata.

---

## Examples

- **POST** `/api/fileanalyse` with form-data:
  - Key: `upfile`
  - Value: (select a file to upload)  

  Returns:  
  ```json
  {
    "name": "example.txt",
    "type": "text/plain",
    "size": 128
  }