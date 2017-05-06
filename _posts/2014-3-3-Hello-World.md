**Hello World**

The clocks were ticking, the heart beats were racing. Finally, it was time. After months of development, it all came down to
this. The results were live. Tried opening the GSoC portal. It crashed. Expected. Gave it few more trials. Finally, it logged in
and there it was. My proposal was now a GSoC Project. The emotions went high and gave way to unbounded joy.

Enough with the emotions, let's move on to the concrete stuff. A bit of a background about the project first before describing
what will be the actual work that I will be doing. Open-Event is a project dealing with the one stop open source solution to the
event management. The event organizers can easily generate an event(on the orga server) and then generate a webapp and also an
android app based on it. It gives almost all the features that the other event management systems like xxxxxx provides. It has
three components: server which deals with the creating of events and plethora of other activities. The data of these events could
then be extacted in the form of json zip and fed into the other components - open-event-webapp and the open-event-android app
which will generate the corresponding web app for the event on both the platforms: web and android. Every event can also be
accessed through the server API which can also be used for the generation of the events.

I will be working on the improvement and enhancement of the open-
event-webapp. I have alredy invested myself in this project for quite some time and had some ideas in mind about what could be
done to improve the webapp further. One thing which had been pending from a long time was the integration of the webapp with
the orga server. Now the thing is, events are generated on the orga-server. We can import these events in the form of JSON zip
file which can be then fed to the generator server of the webapp to generate the event website. Now, we want to combine the
facility. We want to give the user a option through which he can directly generate the webapp of a event from the orga server
itself instead of following a two step process. I made a diagram showing how this could be done:


One thing which I wanted to improve was the interaction between the user and the site. We need to think of ways to increase our
user retention. How can be improve the experience of the user? What essential featuers are missing that should be provided in a
event based app. One thing which was the most glaring was the lack of notifications about the bookmared sessions. This feature
was available on the android app and had been missing from the webapp. I think it would be a fantastic feature to add to the
webapp. It will help the users to get the notifications before the start of the session to remind them about the upcoming
session.At the end of the summer, I hope we can show a notification similar to this:

Speed is one factor which is common across all the areas. No body likes slugginess. No body likes latency. The webpages generated
by the open-event-webapp are static in nature and can be hosted on any server like ftp or Github Pages. It provides an ideal
scenario to apply caching with the help of serivce workers. Service workers are the heart of the Progressive web apps which are
basically javascript scrips which run in the background and intercept the network requests and can respond with custom tailor
made responses. With the help of them, we can implement caching of assets and resources. When there is request for an asset,
we check our cache for that asset and if it exists, then it is directly returned instead of fetching it from the internet.
When the cached assets increases, the dependecy on the network decreases to the point where no internet is required for the
app to run. That's the power of service workers.

Presently, my end-semester exams are going on. It's difficult to take out some spare time when you haven't studied anything
for the whole semester and just get by studying the whole syllabus in a day or two. Needless to say, I will be more consistent
with my contributions in the upcoming weeks.
