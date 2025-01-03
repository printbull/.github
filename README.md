# Requirements Document
## Stakeholder Identification
### System User
The stakeholder here refers to the person that will be using our system to keep track of their assets. <br>

### System Developer
The stakeholder here refers to the person that will be developing the system to provide services to the users. <br>

## User Story
### Stakeholder (User)
**US1:** As a user, I want to register to the service using my email and password so that I can use the service. <br>
**US2:** As a user, I want to ensure that I am not creating a duplicate account so that I can avoid creating a duplicate account. <br>
**US3:** As a user, I want to ensure that the credentials that I entered are encrypted in a secure manner so that I can be safe from data breach. <br>
**US4:** As a user, I want to verify my email when I register to the system, so that other people cannot use my email to create an account of their own. <br>
**US5:** As a user, I want to login to the system using the email and password that I used for registration so that I can access the service. <br>
**US6:** As a user, I want to have an option to save my credentials required for login so that I can avoid entering my credentials whenever I need to login. <br>
**US7:** As a user, I want to remain logged in until I logout or exit the service so that I can avoid logging in repeatedly. <br>
**US8:** As a user, I want to request an email to reset my password so that I can revive my account in case I forget my password. <br>
**US9:** As a user, I want to logout from the system so that I can end my session securely. <br>
**US10:** As a user, I want to delete my account so that I can keep my personal data safe. <br>
**US11:** As a user, I want to manage my account so that I can change my saving goals, asset distribution plan, notification, etc. <br>


**US12:** As a user, I want to create a planned portfolio so that I can plan my assets distribution. <br>
**US13:** As a user, I want to add USD, KRW, JPY, SEK, Stock, Gold, Fund, Cryptocurrency, ELS, Bonds to my planned portfolio so that I can plan my portfolio in a diverse manner. <br>
**US14:** As a user, I want to save the portfolio that I created so that I can see how it goes in the future. <br>
**US15:** As a user, I want to name the portfolio that I created so that I can have a general idea of the portfolio that I created. <br>
**US16:** As a user, I want to add a short description of the portfolio that I created so that I can understand the reasoning behind the portfolio that I have created. <br>
**US17:** As a user, I want the system to automatically record the timestamp of the time that I created my portfolio so that I know when I created the portfolio in the future. <br>
**US18:** As a user, I want to see the percentage of each assets I added to the portfolio so that I can have an intuitive view of the portfolio. <br>
**US19:** As a user, I want to see how dangerous the portfolio I planned is so that I can be aware that the portfolio I have created can be dangerous. <br>
**US20:** As a user, I want the system to automatically save the starting price of each assets in the portfolio so that I know whether the portfolio I made is winning or losing. <br>
**US21:** As a user, I want to see the winning / losing rate in percentage compared to the time I created the portfolio so that I know whether the portfolio I made is winning or losing in an intuitive view. <br>
**US22:** As a user, I want to see all the portfolios I have created so that I can see how well they are performing. <br>
**US23:** As a user, I want to see the ranking of the portfolios that I have created in terms of the rate of return so that I know how I should be dealing. <br>
**US24:** As a user, I want to see how the rate of return would have changed if I made an altering decision of assets distribution so that I can invest in a higher return rate. <br>
**US25:** As a user, I want to see how well my portfolios have performed compared to major indexes (S&P 500, NASDAQ, DOW JONES etc.) so that I know whether the portfolio I created is beating the market or not. <br> 
**US15:** As a user, I want to delete the portfolio that I created so that I only keep what I want in my account. <br>
**US16:** As a user, I want to set the total cash I will be investing and see how much I would actually have to buy so that I can see how much cash I need to prepare. <br>
As a user, I want to see all portfolios I have created so that I can see how well they are performing. <br>

### TBD
**US:** As a user, I want to see what would have happened if I were to buy a single stock every day


## Functional Requirements
### User Service
#### Registration
**FR1.1.1:** The system shall allow the users to create an account using their email and password. <br>
**FR1.1.2:** The system shall verify the password by enforcing the user to enter the password twice. <br>
**FR1.1.3:** The system shall enforce the user to choose a strong password. <br>
**FR1.1.4:** The system shall require users to consent to Terms of Service Agreement. <br>
**FR1.1.5:** The system shall require users to consent to the Privacy Policy Agreement. <br>
**FR1.1.6:** The system shall ensure that the users' credential are saved in an encrypted manner in the database. <br>
**FR1.1.7:** The system shall verify that the email entered by the user has not been used to create an account previously. <br>
**FR1.1.8:** The system shall verify that the email entered by the user is a real email. <br>
**FR1.1.9:** The system shall feedback the user upon successful registration. <br>
**FR1.1.10:** The system shall feedback the user upon failed registration. <br>

#### Authentication
**FR1.2.1:** The system shall allow the users to login via entering their correct email and password pair. <br>
**FR1.2.2:** The system shall provide an option for the user to either hide or show password while entering the credentials. <br>
**FR1.2.3:** The system shall provide a method to recover the user account's password in case the user forgets. <br>
**FR1.2.4:** The system shall notify the user in case the login fails. <br>
**FR1.2.5:** The system shall redirect the user to the main page when it succeeds in authorizing the user. <br>
**FR1.2.6:** The system shall allow the user to stay logged in while using the system. <br>
**FR1.2.7:** The system shall allow the user to logout from the system. <br>
**FR1.2.8:** The system shall provide an option for the user to save email and password for future logins. <br>

#### Account Management
**FR1.3.1:** The system shall allow the user to delete personal account. <br>
**FR1.3.2:** The system shall allow the users to change their password. <br>
**FR1.3.3:** The system shall allow the users to view the ‘Terms of Service Agreement’, and ‘Privacy Policy Agreement’ that the users have agreed on upon registration.

### Portfolio Service
#### Portfolio Creation
**FR2.1.1:** The system shall allow the user to create a virtual assets portfolio. <br>
**FR2.1.2:** The system shall provide the user to choose what kind of assets (USD, KRW, JPY, SEK, Stock, Gold, Fund, Cryptocurrency, ELS, Bond etc.) to add to their portfolio. <br>
**FR2.1.3:** The system shall enforce the user to set the name of the portfolio, and write a short description about it. <br>
**FR2.1.4:** The system shall automatically record the starting price of each assets upon the creation of the portfolio. <br>
**FR2.1.5:** The system shall automatically record the date of creation upon the portfolio is created. <br>
**FR2.1.6:** The system shall enforce the user to select the percentage of each assets they have added to the portfolio. <br>
**FR2.1.7:** The system shall save the created portfolio in the database. <br>
**FR2.1.8:** The system shall alert the user that the type of assets added in the portfolio cannot be edited upon creation. <br>

#### Portfolio Status Tracking
**FR2.2.1:** The system shall update the price of each assets in the portfolio based on the information fetched by the *Asset Price Tracking Service*. <br>
**FR2.2:** The system shall record the price of each assets (Stock, Gold, Fund, Bond) in the portfolio at the end of the market. <br>
**FR2.2:** The system shall record the price of each assets (USD, KRW Savings, JPY, SEK, Cryptocurrency, ELS) in the portfolio at 23:59. <br>

#### Portfolio Display
**FR2.3:** The system shall display all portfolios that the user has created. <br>
**FR2.3:** The system shall display the title, short description, and date of creation of the portfolio. <br>
**FR2.3:** The system shall display the rate of return for each portfolios created by the users. <br>
**FR2.3:** The system shall display the percentage of each asset types that are included in the portfolio. <br>
**FR2.3:** The system shall display how much the portfolio is exposed to dangerous assets. <br>
**FR2.3:** The system shall display the portfolios in the order of return rate (ascending and descending). <br>
**FR2.3:** The system shall allow the users to see what difference there would have been if they were to change the distribution ratio of each assets in the portfolio. <br>
**FR2.3:** The system shall display the how well / poor the user's portfolio compared to the major indices (S&P 500, NASDAQ, Dow Jones etc.) within the same period of time. <br>
**FR2.3:** The system shall display the historical change of the portfolio that the user has created. <br>


### Asset Price Tracking Service
#### Asset Price Fetch
**FR3.1:** The system shall fetch the prices of each assets (Stock, Gold) that the users have added to their portfolio from the national database. <br>
**FR3.1:** The system shall immediately fetch the prices of the newly added asset. <br>
**FR3.1:** The system shall save the prices of the fetched assets in a temporary file. <br>
**FR3.1:** The system shall automatically delete the temporary file once the market opens on the preceding working day. <br>

#### Asset Price Publish
**FR3.2:** The system shall publish the prices of each assets that the *Asset Price Tracking Service* has fetched. <br>


