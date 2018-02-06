# Entry for Feb. 5, 2018

#### Day 1 of project time

### Code I wrote today:

Today I focused on creating my database schema, and wrote quite a bit in my model.py file.

Classes/tables created:

- users
- friendships
- books
- reviews
- shelves
- shelfbooks
- challenges
- challengepoints
- formats
- editions

I was able to get started on my server.py file as well, although creating routes will have to wait until tomorrow.

### Problems I encountered:

While working on my models, I realized I was unsure about how to set up two-way friendships and to create a backref to the users table.
Also unsure about how to link from a user to a book/review to a challenge-point

^ Katie B. helped me work this out!  See first commit for my solutions.

While meeting with mentor Kelsey Hawley after class, realized that I needed to account for exclusive shelves in my schema, and also talked about other ways to manage future changes to my challenge points.  She brought up using an ENUM for book formats instead of creating a separate table, which I am thinking about.

###People that helped me:

Katie Vinton helped me talk through when/where any middle/association tables might need to include backrefs

Katie Byers helped me with setting up the secondary joins and did a code review of my initial version.

Kelsey Hawley reminded me about exclusive shelves and brought up some good points related to challenges that I will do my best to implement in version 2.

Carissa Blossom at Uber encouraged me to use the best possible API data so that I can focus on building features that I care about, and not just fight with someone else's code.

### Resources I found/used:

python goodreads oauth example: [here](https://gist.github.com/gpiancastelli/537923)

xml parser for python: [xmltodict](https://pypi.python.org/pypi/xmltodict)

oauth explanation article (from Kelsey): [oath2 simplified](https://aaronparecki.com/oauth-2-simplified/#web-server-apps)

### Other notes:

My mentor Chris Adams arranged for me to have lunch with some Hackbright and other bootcamp alums working at Uber today, it was great to get their insights on the pros and cons of working after a bootcamp.  They also gave me some great tips for items to focus on when prepping for interviews.

One source of anxiety for me is that I haven't really figured out how to get data from GR yet.  I want to do some practice API calls tomorrow so I feel more prepared when it comes to implementing those pieces.

I also feel stressed out by the changes that Kelsey suggested to my model, and will bring it up in scrum tomorrow.



