# Zuri Chat Core API (Calender plugin ) (1.0.0)
Zuri Chat is an open source slack clone. However, it offers a lot more functionality via a plugin system where each room can be provided by a different plugin provider.

# CREATE REMINDER: 	
The reminder is an endpoint in the zuri calender plug in feature, it helps the user create and set reminders to remind to be reminded of events at a particular time in a calender widget. It is not unique to any event, you can decide to set it or not to set it on an event and it will not display any error.
# HOW IT WORKS: 
The reminder is used to remind the user of a particular event of the selected day, month or year selected.
# HOW TO SET UP THE END POINT:
Copy the URL 
```
https://calendar.zuri.chat/api/v1/reminder
```
Then paste the URL where the endpoint is being required.
# NAVIGATION STEPS:
1.	 Click on the reminder button.
1.	Select the date you want to be reminded.
1.	Fill in the require field the event-ID to be reminded of.
# CODING PROCESS: 
* Firstly, import the serializers.py file.
* Then import all needed modules.
Importing modules
from django.contrib.staticfiles.urls import urlpatterns
from django.urls import path
from views import *

* the path for the reminder endpoint in the urlpatterns should be coded in this form;
```
path(‘create-reminder/’, CreateReminder.as_view(), name=’createReminders’),
```
* Create input and selection fields in the reminder container (div).
* Events can be searched by reminder ID, so create reminder ID (in another div or a class).
* All of then should be defined in the serializer.py file.
