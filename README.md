# HomeAwayExercise1
The page classes are created under the package "com.homeaway.pages" The test cases classes are created under the package "com.homeaway.testcases"

API Test Cases: 2 Tests in One Test Class. API related tasks are performed using the FuelStationUtil.class

Testrunner class: Provided a testrunner class to run all the 3 tests through commandline

TestSuite class: A JUnit TestSuite class to run all the 3 tests

Framework: Simple and light framework using JUnit and PageObject design pattern

Assumptions: The testdata is static and is provided by the test designer in the testcases

Test Case #1 : Submit an Order for iPhone 4s

This is the test case to perform validation related to Submitting an Order
1) Open the Shopping portal on fireforx browser
2) Search for iPhone 4s by typing in the search box
3) Select the correct item using the link description
4) Add the item to the cart
5) Checkout
6) Verify the Cost and checks if the total cost is correct summation of other
costs

Test Case #2: Update Profile This is the test script to perform Account Update validations

1) Script Logs in to an existing account
2) Navigates to the profile page
3) Updates the nickname to a random name
4) Updates the display name to the above name
5) Navigates back to the home page
6) Logout
7) Logs back in using the same account
8) Navigates to the profile page and validates the changes are still existing
9) Reverts back the nickname and display name to initial values for the next run

Test Case #3: Remove from cart and verify empty cart message

This is the test case to perform the cart validation
1) The script looks for the item based on passed parameter; It adds the item
to the cart based on passed parameter;
2) Removes the item from the cart
3) Validates the empty cart message is displayed

Test Case #4 : API Validation to check station ID and Fetch Data for Station Name = HYATT AUSTIN
- Extracts all the fuel stations from the response JSON file
- Fetches the StationID from the File and Validates with Expected Station ID
- Stores the station ID in the dataFile.txt

Test Case #5: API Validation to check the Station Address using Station ID
 - Fetches the stationID from the dataFile.txt
 - sends the query through HTTPS
 - From the response JSON file extracts Street Address, City, State and Zip code
 - Compares with Expected Address
