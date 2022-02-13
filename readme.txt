Application URL to work with: https://courses.letskodeit.com/register

Test Scenario:
                        . Open the web app in Chrome browser
                        . Sign up into the application
                        . Sign in with the registered user
                        . Check that you are logged in
                        . Navigate to “All Courses”
                        . Search the “Selenium” word
                        . Log search result count, result’s titles and prices in a file


TODO:                   pip install selenium webdriver

Impotred Libraries:     webdriver_manager.chrome, selenium, logging, selenium.webdriver.support,
                        selenium.webdriver.support.ui, selenium.webdriver.common.keys, 
                        selenium.webdriver.common.by, string, random, time  

Design Pattern:         Page Object Model (modular structure) 

Selector:               XPATH

Project Modules:        Lib --> drivers.py  (includes driver initilisation method)
                                helpers.py  (includes all common methods which are used in 'Pages')
                                        Designed Methods: -->  

                                                'go_to_page'
                                                'find_and_click' 
                                                'find_and_send_keys'
                                                'find'
                                                'switch_window'
                                                'switch_to_alert' 
                                                

                                log_file.py (includes method 'create_log_file')                              
                        Pages --> 

                                google_page.py
                                        
                                practice_page.py 
                                        
                                sign_in_page.py
                                        

                        Test_Data --> 

                                test_data.py (includes test data, which are used in tests)
Test Runer:                               
                        Tests: --> 
                                lesson6_test.py (includes method test_lets_kodeit which calls methods from Pages)

Run result files:       test_run.txt
                        

Tests should be run in Python. 