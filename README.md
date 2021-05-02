# 14-MVC-Tech-Blog

Homework #14: Model-View-Controller (MVC): Tech Blog

| Method | Route           | Description                                                                                                                                                                                                                                 |
| :----- | :-------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| get    | /api/user       | Display all users                                                                                                                                                                                                                           |
| get    | /api/user/:id   | Display all posts and comments by a particular user id                                                                                                                                                                                      |
| post   | /api/user       | Creates a user with username and password and sets user to logged in - expects JSON object formatted: <br>`{`<br>`"username": "`<em>`USERNAME`</em>`",`<br>`"email": "`<em>`EMAIL`</em>`",`<br>`"password": "`<em>`PASSWORD`</em>`"`<br>`}` |
| post   | /api/user/login | Logs user in - expects JSON object formatted: <br>`{`<br>`"username": "`<em>`USERNAME`</em>`",`<br>`"password": "`<em>`PASSWORD`</em>`"`<br>`}`                                                                                             |
| post   | /api/user/login | Logs user out - expects JSON object formatted: <br>`{`<br>`"username": "`<em>`USERNAME`</em>`"`<br>`}`                                                                                                                                      |
