**Hello World**

The clocks were ticking, the heart beats were racing. Finally, it was time. After months of development, it all came down to
this. The results were live. Tried opening the GSoC portal. It crashed. Expected. Gave it few more trials. Finally, it logged in
and there it was. My proposal was now a GSoC Project. The emotions went high and gave way to unbounded joy.

The Open Event Project offers event managers a platform to organize all kinds of events including concerts, conferences, summits and regular meetups. The components support organizers in all stages from event planning to publishing, marketing and ticket sales. Automated web and mobile apps help attendees to get information easily. There are four components of the project:

1. The Open Event Format Definition [JSON Schema Sample]

2. The Open Event Orga Server [Repository]

3. The Open Event Android App Generator [Repository]

4. The Open Event Web App Generator [Repository]

Actual events can be created very easily on the server. The data of these events can
then be extacted in the form of JSON zip and fed into the other components - open-event-webapp and the open-event-android
who will generate the event app on both the platforms. Every event can also be accessed through the server API.

I will be working on the improvement and enhancement of the open-
event-webapp. Being involved in the development process for a while, I had some ideas in mind about what can be
done to improve it further. One thing which has been pending from a long time is the integration of the webapp with
the orga server. We want the organizer to give the facility to generate the webapp for an event directly on the server itself
with the click of a button. I made a diagram demonstrating how this could be done:


Speed is one factor which is common across all the areas. No one likes slugginess. No one likes latency. The webpages generated
by the open-event-webapp are static in nature and can be hosted on any server like ftp or Github Pages. It provides an ideal
scenario to apply caching with the help of serivce workers. Service workers are the heart of the Progressive web apps and are
basically JS scrips which run in the background and intercept the network requests and can respond with custom tailor
made responses. With the help of them, we can implement caching of assets and resources. When there is request for an asset,
we check our cache for that asset and if it exists, then it is directly returned instead of fetching it from the network.
When the cached assets increases, the dependecy on the network decreases to the point where no internet is required for the
app to run. That's the power of service workers.

We need to think of ways to increase our
user retention. What essential featuers are missing that should be provided in a
event based app? One thing which was the most glaring was the lack of notifications about the bookmared sessions. This feature
is available on the android app and has been missing from the webapp. I think it would be a fantastic addition to the
webapp. It will help the users/speakers to receive notifications before the commencement of a session and remind them about it.
session. At the end of the summer, I hope we can show a notification similar to this:


Presently, my end-semester exams are going on. It's difficult to take out some spare time when you haven't studied anything
for the whole semester and just get by studying the whole syllabus in a day or two. Needless to say, I will be more consistent
with my contributions in the upcoming weeks.
