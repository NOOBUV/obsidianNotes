##### Issue: On keeping rating field mandatory in forms if next was clicked without any response whole app was breaking and Internal Error was thrown.

##### Findings:
- Multiple error were thrown.
- Read the errors keywords and filename which are throwing the error.
- One of the error was showing problem in Rating.tsx.
- Then look up is there error thrown by Rating.tsx.
- If there is try to solve that.
##### Solution:
The error was Language wasn't defined, so in this codebase they have defined text for different languages and if language wasn't defined than the error wasn't fetching any text and the code was breaking.
Just after setting language = "en", the code was working.
[Issue](https://github.com/mobstac-private/beaconstac-forms-app/tree/rating-issue-fixed)

