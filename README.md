# My test documentation :open_file_folder:

[![GitHub last commit](https://img.shields.io/github/last-commit/MonikaDzik/test_cases?color=lightgreen&logo=github)](https://github.com/MonikaDzik)

Here you will find projects that I run independently. There will be more and more of them over time. I write test cases to constantly practice my skills. I even found some bugs 😃

----

# Bug Reports :bug:



## [Rosmann](https://www.rossmann.pl/)

Preconditions:
browser open at: https://www.rossmann.pl/ ; user properly logged into an account ; few (at least five) items added to cart



Title / Severity | Steps to reproduce | Expected result | Effect received | Likelihood of recurrence
:---------------:|:--------------------| :---------------: | :---------------: | :-----------:
The cart preview is displayed incorrectly <br />/<br /> LOW | 1. Having several (at least five) items in the basket, return to the main page by clicking on the "ROSMANN" button at the top of the page <br /> 2. Hover your cursor over the shopping cart icon in the upper right part of the screen <br /> | Preview shows the actual contents of the cart | Cart preview shows no items name or photo. All items names are replaced by *-NaN zł* notification - see [photo](https://drive.google.com/file/d/1EjAdpfUxiOVca5ti8P5wKjLfcQPUkjH6/view?usp=sharing) | LOW - despite numerous attempts, the observed error was not reproduced |

*Description:*  Windows 10 Home (x64), browser Firefox ver. 110.0


## [cararena.pl](https://cararena.pl/)

Preconditions:
browser open at: https://cararena.pl/formularz-finansowanie#step1 ; email address generated using the [10minutemail.net](10minutemail.com) website

Title / Severity | Steps to reproduce | Expected result | Effect received
:---------------:|:--------------------| :---------------: | :---------------:
Contact form disappears <br />/<br /> MEDIUM | 1. Enter generated email address and press "Następny krok" <br /> 2. At the top left of the page, select step 1 (circled number) to go back to the previous step | The form goes back to the previous page | Contact form disappears 

*Description:*  Windows 10 Home (x64), browser Chrome ver. 110.0.5481.78


## [mepel.pl](https://mepel.pl/)

Preconditions: browser open at: https://mepel.pl/

Title / Severity | Steps to reproduce | Expected result | Effect received
:---------------:|:--------------------| :---------------: | :---------------:
No newsletter in English language version <br />/<br /> MEDIUM | 1. Open https://mepel.pl/ on browser <br /> 2. Select English language on top right corner of the page by clicking on England flag <br /> 3. Go to end of the page and enter email address in newsletter field | Correct subscription | There is no newsletter field on English language vershion
Differences in product availability depending on language version <br /> PART 1 <br />/<br /> MEDIUM | 1. Open https://mepel.pl/ on browser <br /> 2. Select English language on top right corner of the page by clicking on England flag <br /> 3. Change language few times from English to Polish and back <br /> 4. Compare the displayed panels | Polish and English site version looks the same | In English version at the top of the page you can see an advertising panel, which is not available in the Polish language version
Differences in product availability depending on language version <br /> PART 2 <br />/<br /> MEDIUM | 1. Open https://mepel.pl/ on browser  <br /> 2. Select English language on top right corner of the page by clicking on England flag  <br /> 3. In searching bar type: "redrewno" and press enter  <br /> 4. Repeat 1-3 steps but with Polish site version <br /> 5. Compare displayed products | Polish and English site version looks the same | English language version allows you to purchase products and the Polish version does not

*Description:*  Windows 10 Home (x64), browser Chrome ver. 110.0.5481.78

----

# Test cases :paperclip:

## [mepel.pl](https://mepel.pl/)
  ###  **Searching:**
  
Preconditions: browser open at: https://mepel.pl/
Title | Action | Expected result
------|--------| ---------------
Correct search | In the search bar at the top of the page enter: "d&d" and press enter | List of products containing the searched phrase along with information about availability
Search for an incomplete phrase | In the search bar at the top of the page: "d" and press enter | Incorrect search criteria message is displayed - minimum two characters required
Phrase search | In the search bar at the top of the page enter the phrase: "d&d monster" and press enter | List of products containing the searched phrase along with information about availability
Searching without entering any criteria | In the search bar at the top of the page do not enter any phases and click the magnifying glass on the right | Below the search bar a message appears asking to enter a searching phrase

*Description:*  Windows 10 Home (x64), browser Chrome ver. 110.0.5481.78


###   **Newsletter:**

Preconditions: browser open at: https://mepel.pl/; email address generated using the [10minutemail.net](10minutemail.com) website

Title | Action | Expected result
------|--------| ---------------
Correct subscription | In the "newsletter" field at the bottom of the page, enter the email address you generated and click "zapisz się!" | Confirmation email has been sent
Re-subscribe to the same email address | In the "newsletter" field at the bottom of the page, enter same email address you generated and click "zapisz się!" | Redirected to a page with information "this address is already in the database", a field is displayed that allows you to unsubscribe, the repeated email address is already entered in the field
Incorrect email | In the "newsletter" field at the bottom of the page, enter email address without "@" symbol and click "zapisz się!" | Redirected to a page with the message: Invalid email address format

*Description:*  Windows 10 Home (x64), browser Chrome ver. 110.0.5481.78




## Contact
Have questions? Feel free to write!

:email: alex.mon8787@gmail.com

[![LinkedIn](https://img.shields.io/badge/Here%20Is%20My%20Profile-LinkedIn-informational)](https://www.linkedin.com/in/monika-dzik-wro-test76aa/)
