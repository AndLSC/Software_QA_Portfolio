
# :computer: Welcome to my Portfolio!

🔨 This portfolio will be continuously under construction. It is a space to share my knowledge, add small practice projects and examples, and share my next learning steps. Stay tuned for updates!


## Table of Contents

- [About Me](#about-me) 

- [Selenium Project](#selenium-project)

- [Manual Testing Example](#manual-testing-example)

- [Bug Documentation](#bug-documentation)

- [Learning Journey](#learning-journey)

- [Contact Information](#contact-information)

    
  
## About Me 

👩 I am a passionate QA professional who makes sure every project is successful and of high quality. With a keen eye for detail, I excel at identifying and resolving issues effectively. I love making things happen precisely and excellently, always aim to deliver exceptional results. My dedication to quality assurance is driven by a genuine commitment to ensuring everything works perfectly.

:books: My Software Testing Skills:

Jira/Xray | Trello | Python | SQL | Postman | Selenium Webdriver | Pytest |



## Selenium Project

Description: 

This project involves automating the shopping cart process on an e-commerce [website](https://www.saucedemo.com/) using Selenium WebDriver. The goal is to ensure the shopping cart functionality works as expected under various scenarios.

Key Features and Functionalities Tested:

- Adding items to the cart.
- Removing items from the cart.
- Updating item quantities.
- Proceeding to checkout.

Tools:

- IDE: PyCharm
- Automation tool: Selenium WebDriver with Python
- Browser: Chrome and Firefox
- Testing Framework: pytest

Challenges Faced:

- Handling Xpath for similar web elements.
- Managing timeouts and synchronization issues.

Code and Documentation:

You can find the complete code and detailed documentation, including some test cases, report, video, and screenshots for this project, in the following GitHub repository:
 [Automated Shopping Cart](https://github.com/AndLSC/Automated_Shopping_Cart.git)




## Manual Testing Example

### Test Case Template
Following the shopping cart example, the manual test cases are listed below.

| **Test_ID**         | **Functionality**   | **Test_Detail**   | **Test_Type**   | **Severity**   | **Preconditions**   | **Test_Data**   | **Steps**   | **Expected Result**   | **Obtained Result**   | **Test Status**   | **Test Evidence**   |
|---------------------|---------------------|-------------------|-----------------|----------------|---------------------|-----------------|-------------|-----------------------|-----------------------|-------------------|---------------------|
| TC01  | Authentication - Login | Verifying that users can log in successfully.|Functional | Critical | Credentials are valid. | Username: standar_user Password: secret_sauce | 1. Go to [Website](https://www.saucedemo.com). 2. Type username and password. 3. Click on the button "Login" | User must be redirected to the Url of [inventory page](https://www.saucedemo.com/inventory.html) | Inventory page is displayed.| Pass | [Login 1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login/test_login_1.png) [Login 2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login/test_login_2.png)| 
| TC02  | Authentication - Login failed | Verifying that system displays an error message (1) when user enters invalid credentials.  |Functional | Critical | Credentials are not valid. | Username: standard_user Password: incorrect | 1. Go to [Website](https://www.saucedemo.com) 2. Type username and password. 3. Click on the button "Login" | System must displayed the following error message (1): "Username and password do not match any user in this service"  | Error message (1) is displayed.| Pass | [LogFailed_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_1.png)| 
| TC03  | Authentication - Login failed | Verifying that system displays an error message (1) when user enters invalid credentials.  |Functional | Critical | Credentials are not valid. | Username: incorrect Password: secret_sauce | 1. Go to [Website](https://www.saucedemo.com) 2. Type username and password. 3. Click on the button "Login" | System must displayed the following error message (1): "Username and password do not match any user in this service"  | Error message (1) is displayed.| Pass | [LogFailed_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_2.png)|
| TC04  | Authentication - Login failed | Verifying that system displays an error message (2) when user enters invalid credentials.  |Functional | Critical | Credentials are not valid. | Username: standard_user Password:| 1. Go to [Website](https://www.saucedemo.com) 2. Type username and password. 3. Click on the button "Login" | System must displayed the following error message (2): "Password is required"  | Error message (2) is displayed.| Pass | [LogFailed_3](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_3.png)|
| TC05  | Authentication - Login failed | Verifying that system displays an error message (3) when user enters invalid credentials.  |Functional | Critical | Credentials are not valid. | Username:   Password: secret_sauce| 1. Go to [Website](https://www.saucedemo.com) 2. Type username and password. 3. Click on the button "Login" | System must displayed the following error message (3): "Username is required"  | Error message is displayed (3).| Pass | [LogFailed_4](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_4.png)|
| TC06  | Authentication - Login failed | Verifying that system displays an error message (3) when user enters invalid credentials.  |Functional | Critical | Credentials are not valid. | Username:   Password: | 1. Go to [Website](https://www.saucedemo.com) 2. Type username and password. 3. Click on the button "Login" | System must displayed the following error message (3): "Username is required"  | Error message is displayed (3).| Pass | [LogFailed_5](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_5.png)|
| TC07  | Authentication - Logout | Verifying that users can log out of their accounts in successfully.  |Functional | Critical | Credentials are valid. | Username: standar_user Password: secret_sauce | 1. Go to [Website](https://www.saucedemo.com) 2. Type username and password. 3. Click on the button "Login". 4. Click on the top left menu. 5. Click on the logout option.| [Login](https://www.saucedemo.com) page must be displayed | Login page is displayed.| Pass | [Logout_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_logout/test_logout_1.png) [Logout_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_logout/test_logout_1.png)
| TC08  | Shopping cart - Add | Verifying that users can add items to shopping cart successfully.  |Functional | Critical | User logs in successfully. | Username: standar_user Password: secret_sauce | 1. Click on the button "Add to cart" of any product. 2. Click on the shopping cart icon.| Items must be added to the shopping cart | Items were added to the shopping cart successfully. | Pass | [Add_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_add_items_to_cart/test_add_items_to_cart_1.png) [Add_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_add_items_to_cart/test_add_items_to_cart_2.png)
| TC09  | Shopping cart - Remove | Verifying that users can remove items from the shopping cart successfully.  |Functional | Critical | User logs in successfully. | Username: standar_user Password: secret_sauce | 1. Click on the button "Add to cart" of any product. 2. Click on the shopping cart icon. 3. Click on the button "Remove".| Shopping cart must be empty | Shopping cart is empty. | Pass | [Remove_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_remove_items_from_cart/test_remove_items_from_cart_1.png) [Remove_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_remove_items_from_cart/test_remove_items_from_cart_2.png) [Remove_3](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_remove_items_from_cart/test_remove_items_from_cart_3.png)
| TC10  | Shopping cart - Update | Verifying that users can update items in the shopping cart successfully.  |Functional | Critical | User logs in successfully. | Username: standar_user Password: secret_sauce | 1. Click on the shopping cart icon. 2. Click on the button "Remove". 3. Click on the button "Continue Shopping". 4. Repeat step 1 and 2. | Shopping cart must be updated with new items added | Shopping cart is updated. | Pass | [Update_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_update_items_in_cart/test_update_items_in_cart_1.png) [Update_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_update_items_in_cart/test_update_items_in_cart_2.png) [Update_3](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_update_items_in_cart/test_update_items_in_cart_3.png) [Update_4](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_update_items_in_cart/test_update_items_in_cart_4.png) [Update_5](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_update_items_in_cart/test_update_items_in_cart_5.png)
| TC11  | Checkout | Verifying that users can complete the checkout process successfully.  |Functional | Critical | 1. User logs in successfully. 2. Items were added to shopping cart. | Username: standar_user Password: secret_sauce | 1. Click on the shopping cart icon. 2. Click on the button "Checkout". 3. Fill in the form with sample data. 4. Click on the button "Continue". 5. Validate the information displayed. 6. Click on the button "Finish". 7. Click on the button "Back Home".| 1. Checkout proccess must be successful. 2. Home page must be displayed. | Checkout process is successful and home page is displayed. | Pass | [checkout_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_1.png) [checkout_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_2.png) [checkout_3](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_3.png) [checkout_4](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_4.png) [checkout_5](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_5.png)



## Bugs Documentation

Under construction
## Learning Journey

Working on it: 
- Cypress
- ISTQB Foundation Level Examen preparation
- API Test Automation
  
## Contact Information


💻 [LinkedIn](https://www.linkedin.com/in/andreinasoto/)

📧 [Contact Information Form](https://forms.gle/M9kkbVYsDNM4Zr1V8).
