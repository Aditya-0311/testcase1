BDD Format.

Feature: Compose Email in Gmail

  Scenario: Sending email successfully
    Given the user is logged into Gmail
    When the user clicks on the compose button
    And fills in the subject "Incubyte"
    And writes the body "Automation QA test for Incubyte"
    And clicks on the send button
    Then the email should be sent successfully

  Scenario: Error handling for empty subject field
    Given the user is composing a new email
    When the user tries to send the email without filling in the subject field
    Then an error message should be displayed prompting the user to fill in the subject field

  Scenario: Error handling for empty body field
    Given the user is composing a new email
    When the user tries to send the email without filling in the body field
    Then an error message should be displayed prompting the user to fill in the body field

  Scenario: Handling subject within character limit
    Given the user is composing a new email
    When the subject is within the character limit
    Then the email should be sent successfully

  Scenario: Handling body within character limit
    Given the user is composing a new email
    When the body is within the character limit
    Then the email should be sent successfully

  Scenario: Error handling for subject exceeding character limit
    Given the user is composing a new email
    When the subject exceeds the character limit
    Then an error message should be displayed prompting the user to shorten the subject

  Scenario: Error handling for body exceeding character limit
    Given the user is composing a new email
    When the body exceeds the character limit
    Then an error message should be displayed prompting the user to shorten the body

  Scenario: Error handling for special characters in subject
    Given the user is composing a new email
    When the subject contains special characters
    Then an error message should be displayed prompting the user to remove special characters from the subject

  Scenario: Error handling for special characters in body
    Given the user is composing a new email
    When the body contains special characters
    Then an error message should be displayed prompting the user to remove special characters from the body

  Scenario: Sending email with attachments
    Given the user is composing a new email
    When the user attaches files
    And sends the email
    Then the email should be sent successfully with the attachments

  Scenario: Handling attachment size limit
    Given the user is composing a new email
    When the attached file exceeds the size limit
    Then an error message should be displayed prompting the user to attach a smaller file

  Scenario: Sending email to multiple recipients
    Given the user is composing a new email
    When the user adds multiple recipients
    And sends the email
    Then the email should be sent successfully to all recipients

  Scenario: Error handling for invalid email address
    Given the user is composing a new email
    When the recipient's email address is invalid
    And tries to send the email
    Then an error message should be displayed prompting the user to enter a valid email address

  Scenario: Error handling for no internet connection
    Given the user is composing a new email
    When the user tries to send the email without internet connection
    Then an error message should be displayed prompting the user to check internet connection.
