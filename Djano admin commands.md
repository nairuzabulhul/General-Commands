

![Log](http://www.slothparadise.com/wp-content/uploads/2014/11/django.png)

#Reset Admin username and password from the shell

##Username:

```$ python manage.py shell```
```
>>> from django.contrib.auth.models import User

If you can’t remember your username, you can view all users in the system.

>>> for u in User.objects.all():
>>>     print u.username
>>>
```

##Password:
```manage.py changepassword <user_name>```

