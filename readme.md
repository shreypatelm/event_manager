## Homework10

---

## Closed Issues Documentation

# [Issue #1: Username Validation Bug](https://github.com/shreypatelm/event_manager/issues/2)  
**Title:** Test Fails Due to Incorrect Mocking of render_template in test_send_markdown_email  
**Description:** render_template is mocked to return a MagicMock object, which is then passed as the HTML content to the send_email method. This causes the assert_called_once_with assertion to fail when checking the arguments passed to send_email.   
**Resolution:**  
- The issue with the test_send_markdown_email test has been resolved by properly mocking the render_template method to return a valid HTML string. This ensures that the send_email method receives the correct email content.

---

# [Issue #2: Username Validation Bug](https://github.com/shreypatelm/event_manager/issues/4) 
**Title:** Nickname Generation Logic
**Description:** The nickname generation feature is not functioning as expected. Generated nicknames are either invalid, not unique, or fail to meet the specified criteria.  
**Status:** Closed   
**Resolution:**  
- Fixed the nickname generation as expected

---

# [Issue #3: Username Validation Bug](https://github.com/shreypatelm/event_manager/issues/6)  
**Title:** Email Verification 
**Description:** We use UUIDs for authentication. To enhance user-friendliness and security, we propose replacing the UUID with an email verification as every user has unique email address 
**Resolution:**  
- Enhanced security through email validation.
---

# [Issue #4: Username Validation Bug](https://github.com/shreypatelm/event_manager/issues/8) 
**Title:** Implement Strong Password Validation Logic 
**Description:** Logic for robust password validation mechanism to enhance security
**Resolution:**  
- enforcing strong password requirements like special characters, at least one uppercase & lowercase and at least one numeric value.

---

# [Issue #5: Username Validation Bug](https://github.com/shreypatelm/event_manager/issues/10) 
**Title:** Pagination validation Logic  
**Description:** Negatyive pagination should be handled correctly 
**Status:** Closed  
**Resolution:**  
- Fixed the negative pagination issue

---

## Docker Hub Image

![Docker_Hub_Image](https://github.com/shreypatelm/event_manager/blob/main/dockerimage.png)

---

## Pytest Coverage

![Pytest Coverage Image](https://github.com/shreypatelm/event_manager/blob/main/coverage.png)  

---

## Learnings from the Assignment

Throughout this assignment, I gained valuable insights into both technical skills and collaborative processes involved in software development. One of the most critical aspects of the project was working with REST APIs and understanding how they handle authentication, requests, and responses. This hands-on experience with JWT token-based OAuth2 authentication deepened my understanding of securing user data and managing access in modern web applications.

I also honed my skills in writing and improving test cases to increase test coverage. The challenge of pushing the test coverage towards 90% made me explore various testing strategies, including unit tests, integration tests, and end-to-end tests. It was rewarding to see how automated testing could not only identify potential bugs but also provide confidence in the stability of the system as new features and changes were added.

On the collaborative side, I gained practical experience using Git for version control, managing branches, and engaging in code reviews through pull requests. This process taught me the importance of clear communication and teamwork. I also learned the significance of well-documented issues and the role of GitHub Issues in tracking progress, making it easier to address bugs and enhancements collaboratively.

Finally, debugging complex issues, such as those related to username validation, password hashing, and profile field edge cases, helped me improve my problem-solving skills. Working through these challenges reinforced the importance of thorough validation and edge case handling to ensure the system's reliability and security.
