# Code-Validator


My Approach:

I've developed a web application using Python and Flask that validates HTML, CSS, and JavaScript code submissions. Here's a breakdown of how it works:

Setting Up the Application: I've used Flask, a Python web framework, to create the application. Flask makes it easy to handle HTTP requests and responses.

Validation Endpoints: I've defined three specific URLs (/validate-html, /validate-css, and /validate-js) where users can send their code for validation.

Validation Functions: For each endpoint, I've created a function (validate_html, validate_css, and validate_js) that receives the code from the user and passes it to the appropriate validation logic.

Validation Logic: Inside the validation functions, there are placeholder functions (validate_html_code, validate_css_code, and validate_js_code) where the actual validation of the code occurs. These functions check for errors in the code and return a list of any issues found.

Response Handling: If there are errors in the code, the server responds with a JSON object containing details about the errors and a status code of 400 (indicating a client-side error). If the code is error-free, the server sends a success message with a status code of 200.

Running the Application: To test the application during development, I've enabled debug mode. This provides helpful features like detailed error messages and automatic server restarts when changes are made to the code.

In summary, my application provides a straightforward way for users to submit their HTML, CSS, and JavaScript code for validation, helping them identify and fix any errors before submitting their assignments on the learning platform.








How to set up and run the validator?

To run this code, you'll need Python and Flask installed on your system. Here are the setup instructions:

Install Python: If you haven't already, download and install Python from the official website: Python Downloads. Follow the installation instructions for your operating system.

Install Flask: Once Python is installed, you can install Flask using pip, Python's package installer. Open a command prompt or terminal and run the following command:

Copy code
pip install flask
Copy and Save the Code: Copy the provided code and save it into a file with a .py extension, such as validator.py.

Run the Application: Navigate to the directory where you saved validator.py using the command prompt or terminal. Then, run the script by executing the following command:

Copy code
python validator.py
Access the Endpoints: Once the application is running, you can access the validation endpoints using HTTP POST requests. You can use tools like cURL, Postman, or write your own code to send requests to http://localhost:5000/validate-html, http://localhost:5000/validate-css, and http://localhost:5000/validate-js with appropriate JSON payloads containing the code to be validated.

Testing: Test the application by sending code snippets to the validation endpoints and observing the responses. Ensure that the validation logic behaves as expected and provides accurate feedback for the submitted code.

That's it! You now have the code running locally, allowing you to validate HTML, CSS, and JavaScript submissions for your learning platform.

