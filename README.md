Site van dndStudentsLeuven

Static HTML site built with Hugo ,https://gohugo.io/documentation/, based on the https://hugoloveit.com/ theme
Check their docs for more info

Hosted with pages, so the main branch is the code that gets converted into HTML, be careful pushing to the main branch as this is what people see when they get on the site.

To build locally and with drafts, use "hugo serve -D --disableFastRender" and go to localhost:1313.
After any change make sure the site is still good with draft enabled And disabled. 

-dateOn is belangrijk, daarmee kunnen we controleren wanneer events op de site komen, zonder dateOn kunnen we geen events op de website hebben die nog niet gebeurd zijn

Adding content:

To add an event with name example_event, add a folder and index.md like the other events, or run "hugo new content events/example_event/index.md"
Afterwards, make sure to fill out the metadata with correct info (dateOn, etc) as the command doesn't autofill these.
Add the content of the event
Now build locally with the -D tag to enable the drafts, check if the new event page is to your liking
Finally, if the page is good, set the draft tag to false (draft = false).

If the page isnt showing up while building, set the date to be like a week ago, If Hugo sees that the date is in the future it doesnt render the page, sometimes if the date was only ~10 minutes ago hugo just doesnt render it so set it to 2023 or something 
