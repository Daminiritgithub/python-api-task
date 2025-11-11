# python-api-task
# User API Fetcher

A Python script that fetches user data from the JSONPlaceholder API and displays it in a clean, readable format. This project demonstrates API integration, JSON handling, error management, and data filtering.

[![Python Version](https://img.shields.io/badge/python-3.6%2B-blue)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Table of Contents

- [About](#about)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Output Example](#output-example)
- [Error Handling](#error-handling)
- [Project Structure](#project-structure)
- [Technical Details](#technical-details)

## About

This project was developed as part of a Python internship assignment to demonstrate proficiency in:
- Making GET requests to RESTful APIs
- Parsing and handling JSON data
- Implementing loops and data iteration
- Error handling and edge case management
- Writing clean, well-documented code

##  Features

- Fetches user data from JSONPlaceholder public API
- Displays user details: Name, Username, Email, and City
- Clean, formatted console output
- **Bonus Feature**: Filters users by city name (cities starting with 'S')
- Comprehensive error handling for:
  - Network connection failures
  - API timeouts
  - HTTP errors (4xx, 5xx)
  - Empty responses
  - Invalid JSON data
  - Well-commented, beginner-friendly code

##  Prerequisites

Before running this script, ensure you have:

- **Python 3.6 or higher** installed on your system
- **pip** (Python package manager)
- **Internet connection** (to access the API)

To check your Python version:
```bash
python --version
```

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/user-api-fetcher.git
cd user-api-fetcher
```

### 2. Install Dependencies

Install the required `requests` library:

```bash
pip install -r requirements.txt
```

Or install directly:
```bash
pip install requests
```

## 🚀 Usage

Run the script from your terminal:

```bash
python user_fetcher.py
```

The script will:
1. Fetch all users from the API
2. Display complete user information
3. Show filtered results (cities starting with 'S')

##  Output Example

```
User Data Fetcher - JSONPlaceholder API
Fetching user data from API...
Successfully fetched 10 users.

--- ALL USERS ---

User 1:
  Name: Leanne Graham
  Username: Bret
  Email: Sincere@april.biz
  City: Gwenborough
------------------------

User 4:
  Name: Patricia Lebsack
  Username: Karianne
  Email: Julianne.OConner@kory.org
  City: South Elvis
------------------------

[... more users ...]

--- BONUS: USERS FROM CITIES STARTING WITH 'S' ---

User 4:
  Name: Patricia Lebsack
  Username: Karianne
  Email: Julianne.OConner@kory.org
  City: South Elvis
------------------------

User 6:
  Name: Mrs. Dennis Schulist
  Username: Leopoldo_Corkery
  Email: Karley_Dach@jasper.info
  City: South Christy
------------------------

Displayed 2 user(s) with cities starting with 'S'.
```

## Error Handling

The script gracefully handles various error scenarios:

| Error Type | Handling |
|------------|----------|
| Connection Error | Displays friendly error message and exits |
| Timeout | Alerts user about timeout (10s limit) |
| HTTP Error | Shows HTTP status code and error details |
| Empty Response | Warns user about empty data |
| Invalid JSON | Handles JSON parsing errors |

## 📁 Project Structure

```
user-api-fetcher/
│
├── user_fetcher.py      # Main Python script
├── README.md            # Project documentation (this file)
├── requirements.txt     # Python dependencies
└── .gitignore          # Git ignore file (optional)
```

##  Technical Details

### API Endpoint

- **URL**: `https://jsonplaceholder.typicode.com/users`
- **Method**: GET
- **Response Format**: JSON
- **Data Returned**: Array of 10 user objects

### Dependencies

- **requests** (>=2.31.0): For making HTTP requests

### Key Functions

| Function | Description |
|----------|-------------|
| `fetch_users()` | Fetches user data from API with error handling |
| `display_users()` | Formats and displays user information |
| `main()` | Orchestrates the entire workflow |

## Testing

### Test on Google Colab

You can also test this script on Google Colab:
1. Go to [Google Colab](https://colab.research.google.com/)
2. Create a new notebook
3. Copy the entire code into a cell
4. Run the cell

### Expected Results

- Successfully fetches 10 users
- Displays all user information correctly
- Filters and shows 2 users from cities starting with 'S'

##  Assignment Requirements

This project fulfills all internship assignment requirements:

- [x] Use GET method to call API endpoint
- [x] Parse JSON response
- [x] Loop through users and display required fields
- [x] Use `requests` library
- [x] **Bonus**: Filter users by city starting with 'S'
- [x] **Bonus**: Comprehensive error handling
- [x] Clean, well-commented code
- [x] README with instructions

## Author

**Damini Saxena**
- GitHub:[https://github.com/Daminiritgithub]
- Email: daminisaxena49@gmail.com

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- [JSONPlaceholder](https://jsonplaceholder.typicode.com/) - Free fake API for testing
- Python `requests` library documentation
- Anthropic's Claude for development assistance

---

**Note**: This is an educational project created for internship assessment purposes.

## Support

If you encounter any issues:
1. Check that Python 3.6+ is installed
2. Verify internet connection
3. Ensure `requests` library is installed
4. Check the API endpoint is accessible

For questions or issues, please open an issue on GitHub.

⭐ **If you found this helpful, please star this repository!**
