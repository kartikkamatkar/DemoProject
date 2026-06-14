# Project Management Form using JsonPowerDB

## Overview

This project is a simple Project Management Form developed using HTML and JavaScript. It allows users to store project details in JsonPowerDB (JPDB).

The application collects project information and inserts it into the PROJECT-TABLE relation of the COLLEGE-DB database.

## Features

* Add project details
* Form validation
* Store records in JsonPowerDB
* Reset form functionality
* Simple and user-friendly interface

## Input Fields

* Project ID
* Project Name
* Assigned To
* Assignment Date
* Deadline

## Database Details

### Database Name

COLLEGE-DB

### Relation Name

PROJECT-TABLE

### Primary Key

Project-ID

## Technologies Used

* HTML5
* JavaScript
* JsonPowerDB
* Fetch API

## Project Structure

```
Login2ExploreProject/
│
├── index.html
└── README.md
```

## How It Works

1. User enters project details.
2. Form validation checks required fields.
3. Data is converted into JSON format.
4. A PUT request is sent to JsonPowerDB.
5. Data is stored in PROJECT-TABLE.
6. Success message is displayed.
7. Form is reset for the next entry.

## Sample Record

```json
{
  "Project-ID": "P101",
  "Project-Name": "Quiz Application",
  "Assigned-To": "Kartik",
  "Assignment-Date": "2026-06-14",
  "Deadline": "2026-06-30"
}
```

## Setup Instructions

### Clone Repository

```bash
git clone https://github.com/kartikkamatkar/DemoProject.git
```

### Open Project

```bash
cd DemoProject
```

### Run Application

Open the `index.html` file in your browser or use Live Server in VS Code.

## JsonPowerDB Configuration

Update the following values in the JavaScript code:

```javascript
const connToken = "YOUR_CONNECTION_TOKEN";
const dbName = "COLLEGE-DB";
const relName = "PROJECT-TABLE";
```

Replace `YOUR_CONNECTION_TOKEN` with your own JsonPowerDB connection token.

## Benefits of JsonPowerDB

* High Performance
* REST API Based
* Lightweight Database
* Easy Integration
* JSON Document Storage

## Future Enhancements

* Search Project by ID
* Update Existing Project
* Delete Project
* View All Projects
* Improved User Interface

## Author

Kartik Kamatkar
