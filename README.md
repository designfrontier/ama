# ask-me-anything
[Ask questions](https://github.com/designfrontier/ask-me-anything/issues/new) get answers... about stuff. [To ask](https://github.com/designfrontier/ask-me-anything/issues/new) click on issues and then open an issue with the question you want answered!

## What is the biggest technical mistake you have made in your career?

Ok... so I've probably made a bigger one but the one that comes to mind immediately is the time that I was working at NASA and writing a mass emailer. It was supposed to read in the alumni to a student program and then send each of them an email. Simple.

As an aside this was back when we wrote code directly on production servers. I know. The horror! But it's what we used to do and so the code I was writing and testing was running on the real production server.

Except that the loop that I had written was an `infinite` loop.

Luckily I had been testing and had my email address hard coded into the to field, and knew the server admin. By the time she got the server hard restarted my inbox had over 120,000 emails in it and outlook crashed everytime I tried to open it and delete them. It took me a good chunck of a day in the outlook web client deleting pages and pages of emails to get to the point I could recieve email again. Plus I essentially crashed the 20+ other sites that were running on the same server as they all got restarted with our server.

Luckily it was a small team with a pretty wildcat perspective on development because everyone else pretty much laughed it off. I was pretty shook up though. Took me a bit to get back in the groove mentally.

Dang... just remembered another good one. But I'll save it for later. Maybe if someone asks about times my servers have been hacked I'll use it.

## I'm interested in learning more about your experiment with site navigation and discoverability. As suggested, my question is...What is your hypothesis and what were you trying to learn from the experiment?

Hang tight... this is going to get a little esoteric.

The expirement really begins with three realizations. 1) That no one seems to agree on the direction that previous and next should be in blog navigation, 2) that no one really goes back and reads a blog's archive, and 3) that the web is both a new age of ephemera and completely permenant.

Ephemera, if you are unfamiliar, are the cheap printed pamphlets that you often recieve from people trying to get your signature on a petition. Or, the cheap signs pasted up for local band's concerts. (More information here: https://en.wikipedia.org/wiki/Ephemera) With the rise of the internet, cheap domains, and cheap hosting, the internet has become the source of most of our ephemera.

Most events, even one time events, have websites now. We crank out brochure sites for marketing campaigns. Manifestos, love letters, political discourse, these all now live on the internet instead of the printed ephemera that they occupied since the printing press was created.

Really the articles that we all churn out on our blogs are ephemera as well. They are popular now and gone tomorrow. Up to date information today and completely out of date six months from now. And yet they are still there. Still present in search engines indices though they have slipped from the collective conscious. They are permenant ephemera, like a concert poster trapped on the corner window of a dillapiated building that somehow sticks around for months after the concert is over.

In thinking about this I realized that the most important thing on any blog is the most recent article. That no one really dives into the archives unless they are directed there from a search engine. So in the pursuit of minimalism in design it felt pretty clear that most navigation could be visually hidden since it is mostly a detractor from the experience of reading which is why people are there in the first place.

Other design decisions have been drawn from this as well. Things like having the root of designfrontier.net redirect to the current article's permenant address. Having swipe gestures for linear navigation through the "timeline" of posts.

This swpie based navigation and the next/previous links at the bottm of the page represent the most obvious forms of navigation. The rest is hidden behind the logo, much like a hamburger menu.

Antoine de Saint Exupéry famously said, "It seems that perfection is attained not when there is nothing more to add, but when there is nothing more to remove." That has been the core design philosophy behind designfrontier.net. That anything not essential, anything that doesn't serve the main reason the user is there should be removed. So nav gets hidden, gestures for touch devices get added, an API for consuming content, and the option to navigate to past articles presented at the bottom once you have finished what you actually came here to do.

I am generally trying to get out of the users way, so they can do what they need to.

There are a few things I am still trying to work out with this approach. The chief being that google doesn't seem to handle the 302 rediret to the permenant URL for the current article nicely. So... I am working on that. There are also a few visual tweaks I'd like to make to the hidden nav and I am playing with the idea of adding a menu button, though that takes away some of the theoretical beauty in exchange for better discoverability. I am not sure if I want to do that yet. The last thing I am working on is a good way to measure the results of this. To identify if usage is going the way that I think it is. Because without measurement this is really more of an artistic manifesto about the internet then it is a design expirment.
