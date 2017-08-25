# ask-me-anything
[Ask questions](https://github.com/designfrontier/ask-me-anything/issues/new) get answers... about stuff. [To ask](https://github.com/designfrontier/ask-me-anything/issues/new) click on issues and then open an issue with the question you want answered!

## What is the biggest technical mistake you have made in your career?

Ok... so I've probably made a bigger one but the one that comes to mind immediately is the time that I was working at NASA and writing a mass emailer. It was supposed to read in the alumni to a student program and then send each of them an email. Simple.

As an aside this was back when we wrote code directly on production servers. I know. The horror! But it's what we used to do and so the code I was writing and testing was running on the real production server.

Except that the loop that I had written was an `infinite` loop.

Luckily I had been testing and had my email address hard coded into the to field, and knew the server admin. By the time she got the server hard restarted my inbox had over 120,000 emails in it and outlook crashed everytime I tried to open it and delete them. It took me a good chunck of a day in the outlook web client deleting pages and pages of emails to get to the point I could recieve email again. Plus I essentially crashed the 20+ other sites that were running on the same server as they all got restarted with our server.

Luckily it was a small team with a pretty wildcat perspective on development because everyone else pretty much laughed it off. I was pretty shook up though. Took me a bit to get back in the groove mentally.

Dang... just remembered another good one. But I'll save it for later. Maybe if someone asks about times my servers have been hacked I'll use it.
