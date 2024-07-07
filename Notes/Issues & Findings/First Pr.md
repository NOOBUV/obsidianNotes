#### Issue: Number field was throwing error even if not required
#### Solution:
##### Findings:
The library used to handle real time validation is [Yup](https://www.npmjs.com/package/yup#stringmatchesregex-regex-message-string--function-schema).

Issue was in number() it was typecasting "" to NaN(not a number) hence it was considering empty value as NaN just like "a" or "\*".

Hence used transform to control the typecasting and adding custom check for "".
[Issue](https://github.com/mobstac-private/beaconstac-forms-app/tree/fix--Number-field-shows-error-even-if-not-mandatory).