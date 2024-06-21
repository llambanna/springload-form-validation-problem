# Form validation problem - my thoughts

### decisions
i glanced through the github history and copied and pasted the html from the deleted index.html because it saved me typing it all out.
i looked around at free styles and found one that was simple and did much of what was needed and used that because i implment other peoples styles rather than creating my own and that was the quickest way of doing it.

i didn't go with create react app or anything fancy like that because i felt taking a break from react and seeing what plain js dev was like for a change.
additionally, without anywhere for the content of the form to go, simple and plain js was fine - if it wasn't an interview question, it would need to be added into an app with react or some other framework anyway, so least effort was valid.

i went with the browser default validation because it's come a long way and it works although differently - in production would style validation so it looks the same in all browsers rather than use browser defaults.

### accessiblity
i went with html that is descriptive and simple colours.

Your objective is to produce this form with as much or as little sophistication as you see fit, explaining what informed your decisions.

### progressive enhancement
it can be modified easily and because there's very little js, easy enough to move into a react provider structure, or whatever framework is required.

### browser support
being plain plain js it will work in any browser.
style of validation text is different in each browser which is not productino ready, as discussed above.

### testing
about the only thing going with plain js rather than a react app misses out on that matters is testing.
i'd use jest or some other testing library to add tests for:
- invalid input - what happens when invalid email, too short password
- valid input - make sure structure of what's submitted is correct
- without tiger selected - make sure you can't see the tiger type
- with tiger - make sure you can see the tiger type

### documentation
it's pretty simple but i've added a few comments - and this.
