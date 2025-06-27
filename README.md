# Selenium_Project

Built a modular test automation framework using Java, Selenium WebDriver, and TestNG.  
Implemented Page Object Model (POM) design for better scalability.  
Executed functional test cases like login, product search, cart flow, and checkout.  
Integrated Maven for build, and Extent Reports for detailed test logs with screenshots.  
Logged all test events for traceability and easier debugging.

🧪 Project Overview:
This project involves developing an automated test suite for a sample e-commerce website using Selenium WebDriver with Java,
built using the Page Object Model (POM) design pattern.
Test cases were designed and executed using TestNG, managed via Maven, and results were logged with detailed reporting.

🛠 Tools & Technologies Used:
Category	   -   Tools / Tech,
Programming Language -	Java,
Testing Framework	- TestNG,
Automation Tool	- Selenium WebDriver,
Build Tool	- Maven,
Design Pattern -	Page Object Model (POM),
Reporting Tool -	Extent Reports,
Browser Driver -	ChromeDriver,
IDE	IntelliJ / -  SpringToolsSuit.

🔍 Module-Wise Logs / Features Explanation:
✅ 1. Test Setup Logs
Launched browser using WebDriver.

Navigated to base URL.

Maximized window and set implicit wait.

Logs include:

pgsql
Copy
Edit
INFO: Browser launched successfully.
INFO: Navigated to https://www.naaptol.com/
✅ 2. Login Module
Tested valid and invalid logins.

Logged success & failure cases:

vbnet
Copy
Edit
INFO: Entered username: testuser
INFO: Entered password: ******  
PASS: User successfully logged in.
FAIL: Invalid credentials error displayed.
✅ 3. Product Search & Filter
Searched for a product and applied filters.

Verified search results, product names, and prices.

vbnet
Copy
Edit
INFO: Search term entered: "Laptop"
PASS: Product list loaded with 10 results.
✅ 4. Add to Cart & Checkout
Verified product addition, quantity updates, and total price.

Validated cart persistence after page refresh.

vbnet
Copy
Edit
INFO: Added "Dell Laptop" to cart
INFO: Cart updated with quantity = 2
PASS: Cart reflects correct total amount.
✅ 5. Error Handling & Screenshot Logging
For any failure, screenshots were captured and attached to reports.

yaml
Copy
Edit
ERROR: Checkout button not clickable.
Screenshot saved: /Screenshots/checkout_error.png
✅ 6. Reporting Logs
Extent report generated after test suite run.

Summary:

Total tests: 39

Passed: 32

Failed: 7

Report includes:

Test name

Steps

Status

Screenshot (for failures)

✅ 7. Reusable Components / Utilities
Created utility classes:

BaseTest.java → Setup & teardown

BrowserFactory.java → Browser init

ScreenshotUtil.java → Screenshot capture

ConfigReader.java → Read from properties file

