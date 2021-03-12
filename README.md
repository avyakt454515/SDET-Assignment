# SDET-Assignment
Q1 . Solution 

1.Name should be written only in alphabet without any special character and without any numerical in it
2.Email should be written with @ symbol
3.Password textbox is in password format so that it cannot will visible
4.If we want to show what is the password there is check box with it 
5.Phone number should be written only in numerical form
6.ther should be a link present to forward to new page where terms or conditions is written 
7.User should be register when we agree terms and condititons
8.when we click on register we should verify that all the details are correct with our test cases if not give error according to the test case
9.when click on register otp is sent to the given phone number
10.If otp is not come in mobile there should be button to resend the otp 
11.and after that we forward to the next page 
12.After otp sent to number verify the otp so that to verify the phone number is right
13.If otp is not right there should be a button to change a phone number or to resend otp 
14.If the otp is correct user should register to the database
15.Than we will forward to the on boarding screen 



Test Cases 

Sr No.	Test Cases	Feature	Description	Steps To Execute	Test Data / Input	Expected Results
1	TC-001	User Interface	Check all the text boxes, radio buttons, buttons, etc	1. Click on Radio buttons, buttons and dropdowns	N/a	UI should be perfect
2	TC-002	Required fields	Check the required fields by not filling any data	1. Do not enter any value in the field.
2. Click on the Register button.	N/a	It should show a mandatory symbol (*) on mandatory fields.
3	TC-003	Required fields	Check user should Register by filling all the required fields	1. Enter valid values in the required fields.
2. Click the Register button.	N/a	1. Users should be registered successfully.
2. A successful registration message should show.
3. Mail should send to the user
4	TC-004	Optional Fields	Check all the optional fields when do not fill data	1. Do not enter any detail in optional fields
2. Enter valid data in required fields
3. Click on the Signup button	N/a	1. It should not ask to fill the optional fields
2. User should be registered successfully
3. A successful registration message should show
4. Mail should send to the user
5	TC-005	Optional Fields	Check all the optional fields when filling data	1. Enter valid data in optional fields
2. Enter valid data in required fields
3. Click on the Register button	N/a	1. User should be registered successfully
2. A successful registration message should show
3. Mail should send to the user
6	TC-006	Email validation	• Check the Email text field that has an Email address without @ symbol. • Check the Email text field that has a random string instead of a real email. • Check the Email text field that has @ symbol written in words. • Check the Email text field that has a missing dot in the email address.	1. Enter Invalid Emails
2. Click on the Register Button.	1.testAtgmail.com
2.test@gmailcom
3.test@gmail
4.@gmail	It should show the validation message for valid email
7	TC-007	Email validation	Check all the valid emails	1. Enter valid Emails
2. Click on the Register Button.	1.test.22@gmail.com
2.test@gmail.com	It should not show any validation message
8	TC-008	Phone Number validation	Check the phone number when passing alphanumeric data	1. Enter alphanumeric data in phone field
2. Click on Register button	1. dada5$7567#7	It should show the validation message 8 for Phone Number
9	TC-009	Phone Number validation	Check the phone number when not pass country code	1. Enter valid phone number without country code
2.Click on Register button	1. 9012078654	It should show the validation message for country code is required
10	TC-010	Phone Number validation	Check the phone number when passing country code	1. Enter valid phone number with country code
2.Click on Register button	1. +9190112244	It should not show any validation message
11	TC-011	Password Validation	Check the password limit when enter value less than min	1. Enter value which is alphanumeric but less than 8.
2.Click on Register button	1. Password	It should show validation message
12	TC-012	Password Validation	Check the password limit when enter value greater than max	1. Enter alphanumeric value but more than 32.
2.Click on Register button	Any Random string with numbers	It should show validation message
13	TC-013	Password Validation	Check the password when passing only numbers	1. Enter a value in numbers which is in between 8-32
2.Click on Register button	1. 12345678	It should show validation message
14	TC-014	Password Validation	Check the password when passing valid data	1. Enter value in alphanumeric which is in between 8-32
2.Click on Register button	1. Pass123456	It should not show any validation message
15	TC-015	Required Fields	Verify if blank spaces are passed in required fields.	1. Go to the Site.
2. Passed blank spaces in required fields.
3. Click on the Register button	N/a	Those Blank spaces should trim and Validation error message for required fields should visible.
16	TC-016	Required Fields	Verify user can verify its Email ID	1. Go to the Email.
2. Click on the verification link.	test22@gmail.com	User should get a verification link and able to verify his/her Email ID.
17	TC-017	Phone Number Validation	Verify if the length of the phone number is incorrect i.e. less than 10.	1. Enter phone number less than 10 digits.
2.Enter all required fields.
3.Click on Register Button	91901122	It should show the validation error message for phone number length.
18	TC-018	Phone Number Validation	Verify if the length of the phone number is incorrect i.e. more than 10	1. Enter phone number less than 10 digits.
2.Enter all required fields.
3.Click on Register Button	91901122445566	It should show the validation error message for phone number length.
19	TC-019	Password Validation	Verify if the password required rules are not satisfied in the password	1. Enter the password which not satisfactory	passw	It should display error with required rules for password value(like it should contain a special character, a small case, a number)

