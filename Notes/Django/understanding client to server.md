- django alone can't serve response to each request it requires an interface that responds as django responds in python objects which can be converted by wsgi (uWsgi or gunicorn).
- Nginx is fully featured web server like gunicorn , but nginx is good at handling files as compared to gunicorn it can cache static files and if user uploads a big file it will buffer that file and hand off to gunicorn.

![[nginx python.png]]

### resources
- [video](https://youtu.be/WqrCnVAkLIo?feature=shared).