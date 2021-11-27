# Challenge 01 - TODO Task Management 📌

This is an application for task management. Is allowed create a **user** and **username**, Too necessari create a CRUD of TODO's list:

- Create a new TODO;
- List all TODO'S;
- Change **title** and **deadline** TODO existing;
- Mark TODO as done;
- Delete a TODO.

All this for each especify user(a **username** will be passed on **header**).

## Routes
POST `/users` - Create new User.
- This route receive `name` and `username` in body of requisition. 

POST `/todos` - Create new TODO.
-  This route receive `title` and `deadline` in body. For this route is necessary username in query header;
- `deadline` field is necessary pass correct date in following format `AGE-MOUNTH-DAY`. 

GET `/todos` - Get All todos.
- This route necessary username in query header. 

PUT `/todos/:id` - Update TODO.
-  This route receive `title` and `deadline` in body. For this route is necessary username in query header;
- `deadline` field is necessary pass correct date in following format `AGE-MOUNTH-DAY`. 

PATCH `/todos/:id/done` - Update Done in TODO.
-  This route receive `id` on query params. For this route is necessary username in query header;

DELETE `/todos/:id` - Delete TODO.
-  This route receive `id` on query params. For this route is necessary username in query header;
