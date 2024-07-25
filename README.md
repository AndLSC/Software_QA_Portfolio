
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

#### :books: My Software Testing Skills:

**Jira/Xray** | **Trello** | **Python** | **SQL** | **Postman** | **Selenium Webdriver** | **Pytest** | **SoapUI** | **HTML** | **Git**



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
 **[Automated Shopping Cart](https://github.com/AndLSC/Automated_Shopping_Cart.git)**




## Manual Testing Example

### Test Case Template
Following the shopping cart example, the manual test cases are listed below.

| **Test_ID**| **Functionality**   | **Test_Detail**   | **Test_Type**   | **Severity**   | **Device and Browser**  |**Preconditions**   | **Test_Data**   | **Steps_Description**   | **Expected_Result**   | **Obtained_Result**   | **Test Status**| **Test Evidence**|
|---------------------|---------------------|-------------------|-----------------|----------------|---------------------|-----------------|-------------|:-------------|-----------------------|-----------------------|-------------------|---------------------|
| TC01  | Authentication - Login | Verifying that users can log in successfully.|Functional | Critical | Windows 10-Chrome(version 126.0.6478.183) |  Credentials are valid. | Username: standard_user Password: secret_sauce | 1. Go to [Website](https://www.saucedemo.com).<br>2. Type username and password.<br>3. Click on the button "Login" | User must be redirected to the URL of [inventory page](https://www.saucedemo.com/inventory.html) | Inventory page is displayed.| Pass | [Login_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login/test_login_1.png)<br>[Login_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login/test_login_2.png)| 
| TC02  | Authentication - Login failed | Verifying that the system displays an error message(1) when a user enters invalid credentials.  |Functional | Medium | Windows 10-Chrome(version 126.0.6478.183) | Credentials are not valid. | Username: standard_user Password: incorrect | 1. Go to [Website](https://www.saucedemo.com)<br>2. Type username and password.<br>3. Click on the button "Login" | System must display the following error message(1): "Username and password do not match any user in this service"  | Error message(1) is displayed.| Pass | [LogFailed_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_1.png)| 
| TC03  | Authentication - Login failed | Verifying that the system displays an error message(1) when a user enters invalid credentials.  |Functional | Medium | Windows 10-Chrome(version 126.0.6478.183) | Credentials are not valid. | Username: incorrect Password: secret_sauce | 1. Go to [Website](https://www.saucedemo.com)<br>2. Type username and password.<br>3. Click on the button "Login" | System must display the following error message(1): "Username and password do not match any user in this service"  | Error message(1) is displayed.| Pass | [LogFailed_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_2.png)|
| TC04  | Authentication - Login failed | Verifying that the system displays an error message(2) when a user enters invalid credentials.  |Functional | Medium | Windows 10-Chrome(version 126.0.6478.183) | Credentials are not valid. | Username: standard_user Password:| 1. Go to [Website](https://www.saucedemo.com)<br>2. Type username and password.<br>3. Click on the button "Login" | System must display the following error message (2): "Password is required"  | Error message(2) is displayed.| Pass | [LogFailed_3](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_3.png)|
| TC05  | Authentication - Login failed | Verifying that the system displays an error message(3) when a user enters invalid credentials.  |Functional | Medium | Windows 10-Chrome(version 126.0.6478.183) | Credentials are not valid. | Username:   Password: secret_sauce| 1. Go to [Website](https://www.saucedemo.com)<br>2. Type username and password.<br>3. Click on the button "Login" | System must display the following error message(3): "Username is required"  | Error message is displayed(3).| Pass | [LogFailed_4](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_4.png)|
| TC06  | Authentication - Login failed | Verifying that the system displays an error message(3) when a user enters invalid credentials.  |Functional | Medium | Windows 10-Chrome(version 126.0.6478.183) | Credentials are not valid. | Username:   Password: | 1. Go to [Website](https://www.saucedemo.com)<br>2. Type username and password.<br>3. Click on the button "Login" | System must display the following error message(3): "Username is required"  | Error message is displayed(3).| Pass | [LogFailed_5](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_login_failed/test_login_failed_5.png)|
| TC07  | Authentication - Logout | Verifying that users can log out of their accounts successfully.  |Functional | Critical | Windows 10-Chrome(version 126.0.6478.183) | Credentials are valid. | Username: standard_user Password: secret_sauce | 1. Go to [Website](https://www.saucedemo.com)<br>2. Type username and password.<br>3. Click on the button "Login".<br>4. Click on the top left menu.<br>5. Click on the logout option.| [Login](https://www.saucedemo.com) page must be displayed | Login page is displayed.| Pass | [Logout_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_logout/test_logout_1.png) [Logout_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/1.authetication/test_logout/test_logout_1.png)|
| TC08  | Shopping cart - Add | Verifying that users can add items to the shopping cart.  |Functional | Critical | Windows 10-Chrome(version 126.0.6478.183) | User logs in successfully. | Username: standard_user Password: secret_sauce | 1. Click on the button "Add to cart" of any product.<br>2. Click on the shopping cart icon.| Items must be added to the shopping cart | Items were added to the shopping cart successfully. | Pass | [Add_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_add_items_to_cart/test_add_items_to_cart_1.png)<br>[Add_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_add_items_to_cart/test_add_items_to_cart_2.png)|
| TC09  | Shopping cart - Remove | Verifying users can successfully remove items from the shopping cart.  |Functional | Medium | Windows 10-Chrome(version 126.0.6478.183) | User logs in successfully. | Username: standard_user Password: secret_sauce | 1. Click on the button "Add to cart" of any product.<br>2. Click on the shopping cart icon.<br>3. Click on the button "Remove".| Shopping cart must be empty | Shopping cart is empty. | Pass | [Remove_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_remove_items_from_cart/test_remove_items_from_cart_1.png)<br>[Remove_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_remove_items_from_cart/test_remove_items_from_cart_2.png)<br>[Remove_3](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/2.shopping_cart/test_remove_items_from_cart/test_remove_items_from_cart_3.png)|
| TC10  | Shopping cart - Update | Verifying users can update items in the shopping cart successfully.  |Functional | Medium | Windows 10-Chrome(version 126.0.6478.183) | User logs in successfully. | Username: standard_user Password: secret_sauce | 1. Click on the shopping cart icon.<br>2. Click on the button "Remove".<br>3. Click on the button "Continue Shopping".<br>4. Repeat steps 1 and 2. | Shopping cart must be updated with new items added | Shopping cart is updated. | Pass | [Update_1](https://github
| TC11  | Checkout | Verifying that users can complete the checkout process successfully.  |Functional | Critical | Windows 10-Chrome(version 126.0.6478.183) | 1. User logs in successfully. 2. Items were added to the shopping cart. | Username: standar_user Password: secret_sauce | 1. Click on the shopping cart icon.<br>2. Click on the button "Checkout".<br>3. Fill in the form with sample data.<br>4. Click on the button "Continue".<br>5. Validate the information displayed.<br>6. Click on the button "Finish".<br>7. Click on the button "Back Home".| 1. The checkout process must be successful.<br>2. The home page must be displayed. | The checkout process is successful and the home page is displayed. | Pass | [checkout_1](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_1.png)<br>[checkout_2](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_2.png)<br>[checkout_3](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_3.png)<br>[checkout_4](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_4.png)<br>[checkout_5](https://github.com/AndLSC/Automated_Shopping_Cart/blob/main/Screenshots/3.checkout/test_checkout_5.png)


  
## Bug Documentation
Under construction



## Learning Journey
🔨 Working on it:<br>

 **Cypress IO** | **Certification ISTQB Foundation Level**   | **API Automation**   

## Contact Information


💻 [LinkedIn](https://www.linkedin.com/in/andreinasoto/)

📧 [Contact Information Form](https://forms.gle/M9kkbVYsDNM4Zr1V8).
