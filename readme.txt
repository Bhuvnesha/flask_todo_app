Explanation of the app.py file:
Flask Setup: Flask(__name__) initializes the Flask application.
Routes: We define 3 routes:
/: Displays the to-do list (index.html).
/add: Adds a task (via a POST request).
/delete/<task_id>: Deletes a task based on the task's index in the list.
In-Memory Task List: We use the tasks list to store tasks temporarily.


Explanation of index.html:
Form: The form allows users to add a new task. It submits a POST request to /add.
Tasks List: This part loops through the tasks list and displays each task along with a delete link.
Delete Link: The delete link points to /delete/<task_id>, where the task ID is passed dynamically.

 Test the Application
Add a few tasks in the input box and click "Add Task".
Your new tasks will appear in the list.
Click the "Delete" link next to a task to remove it.