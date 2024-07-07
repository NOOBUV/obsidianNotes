Was assigned to refactor email sent to clients to new branding with new email.
#### Learnings
- Email has several clients , hence html written need to be checked upon all of them, try using mailtrap.
- Email has one more container in which it renders our html hence we only have some limited available html tags.
#### Important:
Alone \<br> tag can create confusion to gmail, like it can think that the text below are replies to upper email hence it gives them "im" tag which has purplish color. Hence use \<br style="box-sizing:border-box">. Try to use lesser \<br> tag and try to use multiple \<p> tags with color enforced on them so even if gmail introduces span with "im" class p tags color overrides them.
Use Inline css many email clients doesn't support \<style> tag.