📌 Test Scope — Trello Web App


You can download the excel file either in "trello_board_test_cases.xlsx" or in "web-app-testing/test-cases/trello_board_test_cases.xlsx
"



This project evaluates the core functionality of the Trello Web Application using manual testing techniques.
The objective is to demonstrate my ability to design test cases, perform exploratory testing, identify defects, and document them clearly.

Functional areas covered:

User authentication (login & signup)

Board creation and deletion

List creation

Card creation, editing, moving, and deletion

UI/UX consistency

Basic navigation and account settings

Non-functional considerations:

Usability

Input validation

Error handling

Basic performance observations


✔️ Test Cases — Board Creation
🧪 TC01 — Create a new board successfully

Objective: Verify that the user can create a new board.
Preconditions: User is logged in.
Steps:

Click “Create” in the top navigation.

Select “Create Board.”

Enter a valid board name.

Click “Create.”

Expected Result:
A new board is created and displayed on the workspace.

🧪 TC02 — Board creation with empty board name

Objective: Verify that Trello prevents board creation without a name.
Preconditions: User is logged in.
Steps:

Click “Create.”

Select “Create Board.”

Leave the board name field empty.

Click “Create.”

Expected Result:
An error message appears, and no board is created.

🧪 TC03 — Board name maximum character limit

Objective: Check how Trello handles very long board names.
Preconditions: User is logged in.
Steps:

Click “Create.”

Select “Create Board.”

Enter a name longer than 100 characters.

Click “Create.”

Expected Result:
Board is created successfully OR Trello shows a validation message (depends on actual behavior; we will test and record).

🧪 TC04 — Create board with special characters

Objective: Ensure the app allows typical special characters in board names.
Steps: Create a board named @@@ !!! ### ??? TrelloTest123
Expected Result:
Board is created normally (unless Trello blocks some characters).

🧪 TC05 — Cancel board creation

Objective: Verify that clicking “Cancel” stops the process.
Expected Result:
No board is created.
