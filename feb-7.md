# Entry for Feb 7, 2018

#### Day 3 of project time

### Code I wrote today:

Today I rewrote some logic in the oauth routes, and finally got the connection working!

I also wrote some helper/validation functions to check user credentials on
signin/signup.

### Problems I encountered:

Finding the right process for Oauth took a long time - eventually I used the
recommended python library, rauth, and following the code example very closely,
got it working in Readerboard.  I am still unsure about where to keep the final
authorization tokens - in the db?

I am also unable to add new users to my session and database - or at least,
if they are being added, I'm not able to view them.

I'm a little nervous about next steps, as it seems that populating my database is
going to take many many API calls, and I'm not sure about the best way to
structure them.  My next task is to practice with the book.title() search method
from GR, and see if I can parse the response fast enough to use it in my toolbar.

### People that helped me:

Today Henry helped me talk through the OAuth process and encouraged me to look at
samples with other Flask apps to try implementing it into my app.  Chris (mentor)
also came by for a while and took at look at what I've built so far.  He thinks I
should try to use Celery to manage data collection so that I can collect user data
on the fly when they sign up, instead of as a Chron job.  I am going to look into the documentation to see if that is possible, or if it will require me to give up
other features.

### Resources I found:

    [rauth](https://github.com/litl/rauth)

