# API Testing with Postman

> Assignment No. 4 – API Testing using Postman

## 📌 Project Overview

This repository contains a Postman-based API testing assignment focused on validating REST APIs through automated request execution, response verification, and test scripting.

The project demonstrates:

* API request creation and execution
* Validation of HTTP status codes
* Response body verification
* JSON response handling
* Environment and collection usage
* Automated API test scripting using Postman
* API workflow testing
* QA testing practices and reporting

The assignment is designed to showcase practical API testing skills commonly used in Quality Assurance (QA), Software Testing, and Automation Testing roles.

---

# 📂 Repository Structure

```bash
Izzah-10P-Shine-QA-Assignment-4/
│
├── postman/                 # Postman collections and related files
├── .postman/                # Postman workspace/configuration files
└── README.md                # Project documentation
```

> The exact contents of the folders may vary depending on the exported collections and environments included in the repository.

---

# 🧪 Technologies & Tools Used

| Tool / Technology   | Purpose                                       |
| ------------------- | --------------------------------------------- |
| Postman             | API testing and request execution             |
| REST API            | Backend communication and testing             |
| JSON                | Request/response data format                  |
| JavaScript          | Writing Postman test scripts                  |
| Newman *(optional)* | Command-line execution of Postman collections |

---

# 🎯 Objectives of the Assignment

The main goals of this assignment are:

* Understand REST API testing fundamentals
* Learn how to create and organize Postman collections
* Validate API responses and status codes
* Automate API testing using scripts
* Improve debugging and response analysis skills
* Practice real-world QA testing workflows

---

# 🔍 Features Implemented

The project may include the following testing operations:

## ✅ API Request Testing

* GET requests
* POST requests
* PUT requests
* DELETE requests

## ✅ Response Validation

* Status code verification
* Response time checks
* Response body validation
* Header validation
* JSON field verification

## ✅ Automated Assertions

Example validations:

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

```javascript
pm.test("Response contains expected data", function () {
    const responseData = pm.response.json();
    pm.expect(responseData).to.have.property("id");
});
```

## ✅ Environment Variables

* Base URL handling
* Dynamic token usage
* Reusable variables

## ✅ Collection Organization

* Grouped API endpoints
* Structured request folders
* Reusable test scripts

---

# ⚙️ Setup Instructions

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/IzzahKazmi/Izzah-10P-Shine-QA-Assignment-4.git
```

## 2️⃣ Open Postman

Download and install Postman:

[Postman Official Website](https://www.postman.com/downloads/)

## 3️⃣ Import Collection

1. Open Postman
2. Click **Import**
3. Select the exported collection from the `postman/` folder
4. Import environment files if included

## 4️⃣ Run the Collection

* Open the imported collection
* Click **Run Collection**
* Execute all API tests

---

# ▶️ Running Tests with Newman (Optional)

Newman allows Postman collections to run from the command line.

## Install Newman

```bash
npm install -g newman
```

## Run Collection

```bash
newman run collection.json
```

---

# 🧠 QA Concepts Demonstrated

This assignment demonstrates important QA concepts including:

* Functional Testing
* API Validation
* Smoke Testing
* Regression Testing
* Test Automation
* Error Handling
* Assertion-Based Testing
* Response Verification

---

# 📸 Example Workflow

Typical testing workflow followed in this project:

1. Send API request
2. Receive server response
3. Validate status code
4. Verify response body
5. Check headers and timing
6. Execute automated assertions
7. Generate test results

---

# 🚀 Possible Improvements

Future enhancements can include:

* CI/CD integration
* Automated test reporting
* Data-driven testing
* Authentication token automation
* Advanced test scripting
* Integration with Jenkins/GitHub Actions
* Load and performance testing

---

# 📚 Skills Demonstrated

This project highlights practical skills in:

* API Testing
* Software Quality Assurance
* Test Automation
* REST APIs
* Postman Collections
* JSON Handling
* JavaScript Assertions
* Debugging and Validation
