# task_master

A to-do list app where users can list their daily tasks and can apply CRUD operations (Create, Read, Update, Delete) on that data.
By default, the app will launch on your local machine at **http://127.0.0.1:5000/**. (Make sure port number 5000 is free on your machine)

If you want to run on a different port, you can configure the endpoints in the **app.py** script inside the **app.run()** method. e.g:
app.run(host='127.0.0.1', port=8080, debug=True)

**Steps to run app:**
1. git clone https://github.com/moharora8/task_master.git
2. pip install flask flask_sqlalchemy
3. python3 task_master/app.py

**Steps to access test.db**:
- Check whether test.db is created or not in parent folder **task_master/**. If not created, something went wrong with the above steps and you need to restry above steps.
- Download DB browser tool for checking data insider test.db
  <a href="https://sqlitebrowser.org/dl/"><img width="799" height="148" alt="image" src="https://github.com/user-attachments/assets/ab5b1d83-6b63-4fe5-811c-2a67d46cc4b0" /> </a>
- Open test.db inside DB Browser window
- You can run different sql queries on the data now e.g:
  1. SELECT name FROM sqlite_master WHERE type='table';
  2. SELECT * FROM todo;
  3. UPDATE todo SET content = 'Buy groceries' WHERE id = 1;
  4. DELETE FROM todo WHERE id = 1;
