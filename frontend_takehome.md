# Sonastream Frontend Takehome

## Description
The goal of this takehome excercise is to create a URL shortener similar to bitly or dub. We prefer submissions to use Typescript and React, but are open to any implementation library or framework.


## Requirements
- Create a form that allows a user to submit a url and get shortened url
  - Allow a user to override the shortened url slug if available. Throw error states if the desired shortened url is not available
  - Only allow valid urls to be shortened (e.g. `https(s)://(domain)/` )
- Allow a user to add an expiration date on the shortened url with a date picker
- Create a shortened link list page that allows a user to:   
  - View all of their created shortened links
  - Copy a specific link to their clipboard
  - Filter/sort their shortened links by date created or click count
- Create a link analytics page that shows a graph of clicks a specific link has had over time
  - (Bonus: allow a user to view a specific link's clicks by Location or Device)
- Allow a user to navigate to a shortened url and be immediately taken to their original url
  - (e.g. http://localhost/eg041x should redirect to https://www.google.com/search?q=bitly+shortener&ei=ZPvSY_yCH9yv5NoPsvuTwAM&ved=0ahUKEwj8xMmjoeb8AhXcF1kFHbL9BDgQ4dUDCBA&uact=5&oq=bitly+shortener)

## Deliverables
- Implement your solution, including test cases for the application code (integration tests are a plus)
- Include a `README.md` that describes how to set up, run and test your application
- Include any notes for our engineering team that describes your approaches and assumptions
- Email your point of contact that sent you this excercise with a link to a public Github or Gitlab repository.
    - If you are uncomfortable adding this project to your public Github profile, please make a separate account for this submission