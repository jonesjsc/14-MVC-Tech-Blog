# 14-MVC-Tech-Blog

Due Date:P 5/1/2021 @ 11:59 PM
Homework #14: Model-View-Controller (MVC): Tech Blog

# Objectives

The primary objectives of this exercise were to demonstrate the following:

- practical implementation using express and routing (get, post, put, delete)
- practical implementation using Sequalize
- practical implementation using a front end framework (handlebars)
- deployment of complete application to heroku
- github repo management

# Dependencies

This exercise requires the following npm modules

- express
- sequalize

# Links

| Description       | Link                                               |
| ----------------- | -------------------------------------------------- |
| github repo       | https://github.com/jonesjsc/13-E-Commerce-Back-End |
| walkthrough video | https://youtu.be/-gwsvU9YaCA                       |

# Routes

| Method | Route            | Description                                                                                                                                                                                                                                 |
| :----- | :--------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| get    | /api/user        | Display all users                                                                                                                                                                                                                           |
| get    | /api/user/:id    | Display all posts and comments by a particular user id                                                                                                                                                                                      |
| post   | /api/user        | Creates a user with username and password and sets user to logged in - expects JSON object formatted: <br>`{`<br>`"username": "`<em>`USERNAME`</em>`",`<br>`"email": "`<em>`EMAIL`</em>`",`<br>`"password": "`<em>`PASSWORD`</em>`"`<br>`}` |
| post   | /api/user/login  | Logs user in - expects JSON object formatted: <br>`{`<br>`"username": "`<em>`USERNAME`</em>`",`<br>`"password": "`<em>`PASSWORD`</em>`"`<br>`}`                                                                                             |
| post   | /api/user/login  | Logs user out - expects JSON object formatted: <br>`{`<br>`"username": "`<em>`USERNAME`</em>`"`<br>`}`                                                                                                                                      |
| get    | /api/post        | Display all posts and comments                                                                                                                                                                                                              |
| get    | /api/post/:id    | Display a single post and all comment                                                                                                                                                                                                       |
| post   | /api/post        | Creates a new post - expects JSON object formatted: <br>`{`<br>`"title": "`<em>`TITLE`</em>`",`<br>`"content": "`<em>`CONTENT`</em>`"`<br>`}`                                                                                               |
| delete | /api/post/:id    | Deletes a post by post id                                                                                                                                                                                                                   |
| get    | /api/comment     | Get all Comments                                                                                                                                                                                                                            |
| get    | /api/comment/:id | Get Comment by ID                                                                                                                                                                                                                           |
| post   | /api/comment     | Create a new comment - expects JSON object formatted: <br>`{`<br>`"comment_text": "`<em>`COMMENT_TEXT`</em>`",`<br>`"post_id": "`<em>`POST_ID`</em>`"`<br>`}`                                                                               |
| put    | /api/comment/:id | Update a comment by ID - expects JSON object formatted:<br>`{`<br>`"comment_text": "`<em>`COMMENT_TEXT`</em>`"`<br>`}`                                                                                                                      |
| delete | /api/comment/:id | Deletes a commend by ID                                                                                                                                                                                                                     |
