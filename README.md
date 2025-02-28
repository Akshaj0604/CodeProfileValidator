# CodeProfileValidator

CodeProfileValidator is a Django web application that allows users to check the existence of profiles on various coding platforms by providing the platform name and username.

## Features

 **Platform Support**: Supports checking profiles on multiple coding platforms including HackerRank, CodeChef, Codeforces, and GeeksforGeeks.
 **Cross-Origin Requests**: Configured to accept requests from specified origins using CORS (Cross-Origin Resource Sharing).
 **Simple API**: Provides a simple API endpoint for checking profile existence by passing platform name and username.

 **NOTE: This project is hosted on Render with limited support to `HackerRank`, `CodeChef`, `Codeforces`, and `GeeksforGeeks`. If you want to use it locally, you will need to set up your own Django application.**

## Using the Existing App Hosted on Render

1. **Access the API:**

   - You can use the existing app hosted on Render to access the API and check profile existence on various coding platforms.

   - Endpoint: `https://codeprofilevalidator.onrender.com/check-url-platform/`

   - Parameters:
     - `platform`: Name of the coding platform (e.g., leetcode, hackerrank, codechef).
     - `username`: Username to check.

   - Response:
     - `exists`: Boolean value indicating whether the profile exists.
     - `url`: URL of the profile.

2. **Available Platforms:**

   - HackerRank
   - CodeChef
   - Codeforces
   - GeeksforGeeks
  
**Example:** 
```
https://codeprofilevalidator.onrender.com/check-url-platform/?platform=hackerrank&username=<yourusername>
```

## Setting Up Your Own Django Application

### Local Setup

1. **Fork the Repository:**

   Click the "Fork" button in the top-right corner of the repository.

2. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/CodeProfileValidator.git
   cd CodeProfileValidator
   ```

3. **Create a Virtual Environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```
   If using Windows, use the following command:
   ```bash
   venv\Scripts\activate
   ```

4. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

5. **Run the Development Server:**

   ```bash
   python manage.py runserver
   ```

   The development server will start running at `http://127.0.0.1:8000/`.

### API Endpoint

You can use the following endpoint to check the existence of profiles:

- Endpoint: `http://127.0.0.1:8000/check-url-platform/`
- Method: GET
- Parameters:
  - `platform`: Name of the coding platform (e.g., hackerrank, codechef).
  - `username`: Username to check.

- Response:
  - `exists`: Boolean value indicating whether the profile exists.
  - `url`: URL of the profile.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Create a new pull request.

## License

This project is licensed under the Apache-2.0 License. See the [LICENSE](LICENSE) file for more details.