# rbs-assignment

Technical design:
 To get a list of users, use the fake api https://jsonplaceholder.typicode.com/users and
design cards/tiles based on the response. Each card / tile should have “name”, “email”,
“phone number” and this card/tile should be clickable
 To get user’s specific to-do list, use the fake api
https://jsonplaceholder.typicode.com/users/1/todos and design a to-do list in a tabular
form. The table should consist of 3 columns such as “Title”, “Status” and “Action” and a
“Back” button to go back to “Users” page
To-do list mapping with response as below:

 “title” = “Title”
 “completed” = “Status”

 When the “completed” value is TRUE, the status should read as “Closed”, the appropriate
row’s action button should read as “Open” and the background colour of that row should be
in “GREEN”
 When the “completed” value is FALSE, the status should read as “Open”, the appropriate
row’s action button should read as “Close” and the background colour of that row should be
in “AMBER/YELLOW”
 Avoid calling multiple API calls for same reason instead use cached data from store (NgRx)
 On click of any action (Open / Close), the respective todo’s status should get updated (flip
the status) in the store
 Good to have unit test coverage
