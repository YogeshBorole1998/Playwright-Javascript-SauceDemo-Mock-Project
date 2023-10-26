# Playwright Javascript Mock Project : 
An example project demonstrating automation of Playwright with JavaScript with page object design pattern framework.

# Application Under Test : 
We are using https://www.saucedemo.com/ as the Application Under Test. This App is a React.js Frontend.<br>
URL: https://www.saucedemo.com/

# Scenarios : 
> Scenario 1: Login as a standard user to verify the products page and logout from the application<br>
> Scenario Description: User logs into the website and verifies all the elements on the products page and logs out from the application. This is like a Smoke test.<br>
> Testname: TC_01_productPage.test.js
<br>

> Scenario 2: Login as a standard user to complete the checkout workflow<br>
> Scenario Description: User logs into the website and completes the checkout workflow and logs out from the application. This is a Happy path test scenario.<br>
> Testname: TC_02_checkoutWorkflow.test.js
<br>

> Scenario: 3: Login as a standard user to select a product item and then login as a performance_glitch_user to complete the checkout workflow<br>
> Scenario Description: The application is verified with all the necessary buttons and links on all the pages including error messages by the standard user. Then the checkout process is therefore completed by the performance_glitch_user.<br>
> Testname: TC_03_checkoutWithSUandPGU.test.js
<br>

> Scenario 4: Login as a “problem_user” to add a product item to the shopping cart and then complete the checkout workflow by logging in as a “performance_glitch_user”<br>
> Scenario Description: User is logged in as “Problem_user” and adds an item to the cart. User fills in the firstname, lastname and postal code. Since the “Problem_user” cannot perform the checkout process because of the lastname error message, user logs off the application.<br>
> Performance_glitch_user log into the application and completes the checkout workflow.<br>
> Testname: TC_04_checkoutWithPUandPGU.test.js
<br>

> Scenario 5: Login as locked_out_user to verify error message and then Login as performance_glitch_user to add a product item to the cart and logout from the application.<br>
> Login as a standard user now to complete the checkout workflow.<br>
> Scenario Description: User is logged in as “Locked_out_user” to validate the error message on the Login page.<br>
> Now, Login as a performace_glitch_user and add a product item to the cart and logout of the application.<br>
> Standard user is logged in and verifies the product item added by the performance glitch user earlier and completes the checkout workflow.<br>
> Testname: TC_05_checkoutWithPGUandSU.test.js
> <br>

# Project Results :
1. HTML Report : npx playwright show-report OR npx playwright test --reporter=html <br><br>
<img width="519" alt="image" src="https://github.com/YogeshBorole1998/Playwright-Javascript-SauceDemo-Mock-Project/assets/104203768/18c10c09-3325-4172-ab2a-6ffc2a6b7b8c"> <br>

2. Dot Report : <br><br> <img width="568" alt="image" src="https://github.com/YogeshBorole1998/Playwright-Javascript-SauceDemo-Mock-Project/assets/104203768/ad7bc625-7a97-4105-8779-5166ba5cbf25"> <br>
3. List Report : <br><br><img width="741" alt="image" src="https://github.com/YogeshBorole1998/Playwright-Javascript-SauceDemo-Mock-Project/assets/104203768/0a631c4e-9503-4e99-9e71-b6ddf50eff46"><br>
4. Line Report : <br><br> <img width="580" alt="image" src="https://github.com/YogeshBorole1998/Playwright-Javascript-SauceDemo-Mock-Project/assets/104203768/0623d961-fa7f-47bc-a253-dafd86b241a9"><br>
5. Allure Report : npx playwright test --project chromium -->  allure generate allure-results -o allure-report --clean --> allure open allure-report <br><br> <img width="902" alt="image" src="https://github.com/YogeshBorole1998/Playwright-Javascript-SauceDemo-Mock-Project/assets/104203768/1c7ccb71-de81-4e31-a986-e361d1865b62">
<br>





