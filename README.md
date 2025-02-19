- Name: Ahmad Zaydan
- Student ID: 2702358393
- Class: B4CC

# Rethinking the frontend with HTMX

- HTMX is a tiny javascript library which basically allows you to trigger Ajax calls and deal with the responses using attributes set in html tags. The big thing is that it expects the responses to be html snippets, which it can then place in the current page.

- So a simple usecase is that an ajax call is triggered and the response is html that is used to replace the element that triggered the call. I looked that this and tried it out. My first thought was WHY!! A second look, then a third and I began to see why HTMX could possibly change Front end in a huge way, especially if your using a good backend with a powerful templating engine.

- HTMX requires you to rethink how you do front end coding. For a long time we have worked on the idea that the front end does Ajax calls that return json, which we then render into templates, or make changes to elements in the dom. HTMX basically says that all rendering is done by the backend instead. No more sending JSON, and altering elements with Javascript, instead we get HTML back and just replace/add to elements on the front end. We basically shift away from Javascript on the front end doing most of the work, to using the backend and template engines on the backend to deliver ready to use html snippets.

- So all HTMX needs to do is send the Ajax call based on the right event and then decide what is going to happen to the html when its returned.
