Overview
========

The UoACalendar system consists of a backend, which hosts your calendars, and a frontend which is the calendar displayed in your website.
To facilitate the implementation of your calendar, we provide the bower javascript module **fullcalendar-uoa-ui**, which has the basic calendar functionality and is ready to go.  
Alternatively, you can use this module as a template, and implement your own with extra features.  In this case, you can make use of the base libraries **fullcalendar** and **uoacalendar**.

Getting your API key and making new calendars
---------------------------------------------

First, you need to log into the the backend on your browser:

http://sitcalprd01.its.auckland.ac.nz

with your UPI and password.

Then on the top right corner of the menu bar, click on your email address, and then click "API Key" in the dropdown menu. 
You will see your unique API key, which you should use in your website.

The next step is to create a new calendar.  Click the calendar icon on the top left side of the menu bar, and then click  "+ New calendar" on the dropdown menu.
Type the name for your new calendar, and click "create".  Then the calendar is created, and you will be switch to this new calendar.

On the url field of your web browser, a link to your calendar will be displayed, such as:

http://sitcalprd01.its.auckland.ac.nz/?calendar=20

In the above case, the value of calendar is 20, which is the calendar ID for your new calendar.  Write it down, as you need to specify it in your website.

In the calendar dropdown menu, you can also switch to a different calendar or delete a calendar.

To list all calendars you have, visit:

http://sitcalprd01.its.auckland.ac.nz/calendars/

And to list all events in a given calendar, visit:

http://sitcalprd01.its.auckland.ac.nz/calendars/_____calendar_ID_____/events/

Finally, you can find the API of the backend at:

http://sitcalprd01.its.auckland.ac.nz/docs/


Setting up a calendar in your website
-------------------------------------

After getting your API key and calendar ID, you can start working on your website.
 
First, you need to download and install node.js at:

http://nodejs.org/

Then you need to install bower by running:

```bash
$ npm install -g bower
```

You also need to install git, which can be downloaded at http://git-scm.com 

Now you can change directory to your site, and install the **fullcalendar-uoa-ui** module, which will automatically pull all its dependencies:

```bash
$ bower install fullcalendar-uoa-ui
```

All modules will reside in **bower_components** folder.  Now you can follow the instructions at **bower_components/fullcalendar-uoa-ui/README.md** to
get your calendar working on the website.

If you want to modify the calendar or add functionality, you can consult the **fullcalendar** API:

http://fullcalendar.io/docs/
