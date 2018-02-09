# Entry for Feb. 8, 2018

#### Day 4 of project time

### Code I wrote today:

Did a little refactoring in server.py today to find out why my session-based
logic wasn't working in the "/" route.

Wrote a new route for book_search!! (in server.py)

Wrote a working function to create a list of book dictionaries in xml_parse.py,
using input data from postman saved in galore.xml

Added code to index.html to display books under the search bar after a user
inputs the title of a book (this hasn't been tested yet, because it's not
technically working)

### Problems I encountered:

I had some logic on the homepage that checks for a key called "user" in the session,
and if a user was present, it would display the index.html.  Otherwise, it would reroute
the user to the signup form.  This logic wasn't working and I couldn't find any
evidence that the user key/value was being added to the session at all.  Likewise,
the user creation process doesn't seem to be updating my database for some reason.

on the API side, I tried implementing search today.  When using data from Postman,
I did a little reading on the untangle library and was able to create a list of book
dictionaries based on the feedback.  However, when I tried to implement this into
Flask, using a python requests library, something seems to be wrong, and I was unable
to get at the data.

Summary:
Still can't update DB.
Still can't save user in session.
Search works, but only through reading a text file, not an API response.

### People that helped me:

Rachel TG did a ton of work to help me with debugging the session variable problems
I was encountering.  We are still not sure what happened, but I suspect that the
OAuth request process somehow clears out the session temporarily, and will do some
research on this tomorrow.

Sarah also helped me with rubber ducking today.  Taking a walk and going to
Starbucks around 4PM may have saved my sanity.

### Resources I found:

Got [Postman](https://www.getpostman.com/) working to test out some book search routes

used [untangle](http://untangle.readthedocs.io/en/latest/#) to parse the xml

experimented with python [requests library](http://docs.python-requests.org/en/master/) to make
a get request from the app


