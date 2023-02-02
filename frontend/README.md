# Sonastream Frontend Takehome
     ___  _____  _  _    __      ___  ____  ____  ____    __    __  __ 
    / __)(  _  )( \( )  /__\    / __)(_  _)(  _ \( ___)  /__\  (  \/  )
    \__ \ )(_)(  )  (  /(__)\   \__ \  )(   )   / )__)  /(__)\  )    ( 
    (___/(_____)(_)\_)(__)(__)  (___/ (__) (_)\_)(____)(__)(__)(_/\/\_)

## Description
The goal of this takehome excercise is to create a simple dashboard for a link shortener similar to bitly or dub. We prefer submissions to use Typescript, React and Tailwind, but are open to any implementation library or framework or css framework you are most comfortable with.

This nested repository `frontend`  contains `./links.json` which is a local array of links returned from a database with the following shape:

| Key | Description |
|---------|-------------|
| id | id for the sql row |
| scheme | original uri scheme |
| path | original uri path |
| raw_shortened_path_id | slug for the shortened uri |
| root | original uri root |
| shortened_path | path of the shortened uri (/ + slug) |
| shortened_uri | full shortened uri |
| uri | original uri |
| count | number of times the shortened uri has been visited and caused a redirect |
| created_date | ISO-8601 date the entry was created |

## Requirements
  - Create a form that allows a user to submit a url and get shortened url back (local storage or appending to the `links.json` is sufficent)
    - Only allow valid urls to be shortened (e.g. https(s)://(domain)/ )
  - Create a list view that displays all of the link objects 
  - Allow a user to navigate to the shortened link, be redirected to the original uri and append to the current count
  - Allow a user to filter the list view by count in ascending or descending order and created date
  - Create individual pages that allow a user to click on any link in the list view and open a page view that displays more information about the link
  - Allow a user to download the entire json array/list view as a CSV to their local machine with a download button

## Deliverables
- Implement your solution, including test cases for the application code (integration tests are a plus)
- Include a `README.md` that describes how to set up, run and test your application
- Include any notes for our engineering team that describes your approaches and assumptions
- Email your point of contact that sent you this excercise with a link to a public Github or Gitlab repository.
    - If you are uncomfortable adding this project to your public Github profile, please make a separate account for this submission

## Notes
- Please show us strengths of your engineering abilities, technical design and attention to detail. While small/simple, this takehome is the main way we will assess your technical abilities. 