--- 
wordpress_id: 600
layout: post
title: Cucumber Failing Scenarios
wordpress_url: http://frozenplague.net/?p=600
---
I submitted <a href='https://rspec.lighthouseapp.com/projects/16211/tickets/360-console-output-of-failing-scenarios'>a ticket</a> for Cucumber, and I hope that it gets accepted:

<blockquote>I encountered a problem when I was using cucumber today. I changed a small detail in one of my Rails controllers and when I ran the features many of them turned red! Disaster! So I scrolled back up, found one that was failing and copy and pasted the file:line syntax into the cucumber command and made them all work!

What I didn't like about this process was that I had to scroll back up through a mixed mountain of red and green features. I only wanted to know which of my features were failing. Trudging through this mess, I thought "If only cucumber showed me the failing features in the summary, along with all the other useful information it displays there" and then I remembered "Cucumber is an open-source project, I could fork it and add it during my spare time!".

So I did.

My commit that adds this functionality is added here: http://github.com/radar/cucumber... for all to gaze upon, criticise and ideally improve upon. At the moment it does everything but exceptions that are raised during Scenarios, something I intend to look on later this evening or perhaps one of you lovely people could do that.

I'd really love to see this merged into the core since I believe (along with my coworkers and friends) this is "extremely fucking useful".

Thanks for reading!</blockquote>

And now the <a href='http://github.com/aslakhellesoy/cucumber/commit/34bc9bf5f4e4b9de55508086092af097dffc7548'>ticket's been accepted</a> and applied! Thanks to Aslak for this!
