# My test documentation :open_file_folder:

Here you will find projects that I run independently. There will be more and more of them over time. I write test cases to constantly practice my skills. I even found some bugs 😃

----

# Test cases :paperclip:

## [mepel.pl](mepel.pl)
  ###  **Searching:**
  
Preconditions: browser open at: https://mepel.pl/
Title | Action | Expected result
------|--------| ---------------
correct search | in the search bar at the top of the page enter: "d&d" and press enter | a list of products containing the searched phrase along with information about availability
search for an incomplete phrase | in the search bar at the top of the page: "d" and press enter | Incorrect search criteria message is displayed - minimum two characters required
phrase search | in the search bar at the top of the page enter the phrase: "d&d monster" and press enter | a list of products containing the searched phrase along with information about availability
searching without entering any criteria | in the search bar at the top of the page do not enter any phases and click the magnifying glass on the right | below the search bar a message appears asking to enter a searching phrase

*Description:*  Windows 10 Home (x64), browser Chrome ver. 110.0.5481.78


###  * **Newsletter:**

Preconditions: browser open at: https://mepel.pl/, email address generated using the [10minutemail.net](10minutemail.com) website
Title | Action | Expected result
------|--------| ---------------
correct subscription | in the "newsletter" field at the bottom of the page, enter the email address you generated and click "zapisz się!" | confirmation email has been sent
re-subscribe to the same email address | in the "newsletter" field at the bottom of the page, enter same email address you generated and click "zapisz się!" | redirected to a page with information "this address is already in the database", a field is displayed that allows you to unsubscribe, the repeated email address is already entered in the field
incorrect email | in the "newsletter" field at the bottom of the page, enter email address without "@" symbol and click "zapisz się!" | redirected to a page with the message: Invalid email address format

*Description:*  Windows 10 Home (x64), browser Chrome ver. 110.0.5481.78


---

# Bug Reports :beetle:

## [mepel.pl](mepel.pl)

Preconditions: browser open at: https://mepel.pl/

Title / Severity | Steps to reproduce | Expected result | Effect received
:---------------:|:--------------------| :---------------: | :---------------:
no newsletter in English language version <br />/<br /> MEDIUM | 1. open https://mepel.pl/ on browser <br /> 2. select English language on top right corner of the page by clicking on England flag <br /> 3. go to end of the page and enter email address in newsletter field | correct subscription | there is no newsletter field on English language vershion
differences in product availability depending on language version <br /> PART 1 <br />/<br /> MEDIUM | 1. open https://mepel.pl/ on browser <br /> 2. select English language on top right corner of the page by clicking on England flag <br /> 3. change language few times from English to Polish and back <br /> 4. compare the displayed panels | Polish and English site version looks the same | in English version at the top of the page you can see an advertising panel, which is not available in the Polish language version
differences in product availability depending on language version <br /> PART 2 <br />/<br /> MEDIUM | 1. open https://mepel.pl/ on browser  <br /> 2. select English language on top right corner of the page by clicking on England flag  <br /> 3. in searching bar type: "redrewno" and press enter  <br /> 4. repeat 1-3 steps but with Polish site version <br /> 5. compare displayed products | Polish and English site version looks the same | English language version allows you to purchase products and the Polish version does not

*Description:*  Windows 10 Home (x64), browser Chrome ver. 110.0.5481.78
