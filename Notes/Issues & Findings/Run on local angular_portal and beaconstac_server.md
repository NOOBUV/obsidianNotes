in angular.json:
remove .qa from line 65
in index.html
comment line 15-199 (to disable content security policy)
angular-portal
comment localhost on 'app.constants.ts'

==Content Security Policy==
It is an added layer of policy for the web page, it helps to detect Cross site scripting (XSS) (basically trapping users of websites on clicking links not meant to be by manipulating frontend with scraping) and data injection. It specifies approved sources of content that the browser should execute.