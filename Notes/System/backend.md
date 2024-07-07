- We use nginx as webserver with uwsgi as WSGI server which is a middleware to communicate between python application and webserver.
- nginx is generally used for serving static files.
- WSGI and ASGI are Python specifications that define how web servers can communicate with web applications written in Python. They provide a standard interface between web servers and Python applications, allowing them to work together seamlessly.
### useful resources
- [article](https://santoshk.dev/posts/2023/why-use-wsgi-asgi-when-we-have-nginx/#:~:text=By%20deploying%20a%20Python%20application,standard%20interface%2C%20not%20just%20Nginx.) for why should we wsgi protocol evethough nginx can do it's job.
- [article](https://builtin.com/data-science/wsgi) why wsgi (gunicorn vs uwsgi)