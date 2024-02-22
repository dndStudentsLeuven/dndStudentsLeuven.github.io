Site van dndStudentsLeuven

Static HTML site built with Hugo ,https://gohugo.io/documentation/, based on the https://hugoloveit.com/ theme
Check their docs for more info

Hosted with pages, so the main branch is the code that gets converted into HTML, be careful pushing to the main branch as this is what people see when they get on the site.

To build locally and with drafts, use "hugo serve -D --disableFastRender" and go to localhost:1313.
After any change make sure the site is still good with draft enabled And disabled. 


Adding content:

To add an event with name example_event, run "hugo new content events/example_event.md"
Afterwards, make sure to fill out the metadata with correct info (DatePlanned, toc.enable, etc) as the command doesn't autofill these.
Add the content of the event
Now build locally with the -D tag to enable the drafts, check if the new event page is to your liking
Finally, if the page is good, set the draft tag to false (draft = false).
