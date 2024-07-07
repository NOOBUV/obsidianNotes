If you have a class Question and it has choices which is also a class
to get all question objects:
Question.objects.all()
Question.objects.filter(using some function or field)
Question.objects.filter(pub_date__year == current_year) (current_year = timezone.now().year)
q = Question.objects.get(id=1/pk=1)
q.choice_set.all()
q.choice_set.create(choice_text="Not much", votes = 0)
c = q.choice_set.filter(choice_text__startswith = "something")
c.delete()