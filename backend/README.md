# Sonastream Backend Takehome

     ___  _____  _  _    __      ___  ____  ____  ____    __    __  __ 
    / __)(  _  )( \( )  /__\    / __)(_  _)(  _ \( ___)  /__\  (  \/  )
    \__ \ )(_)(  )  (  /(__)\   \__ \  )(   )   / )__)  /(__)\  )    ( 
    (___/(_____)(_)\_)(__)(__)  (___/ (__) (_)\_)(____)(__)(__)(_/\/\_)


## Description
The goal of this takehome exercise is to create a URL shortener similar to bitly or dub. We prefer submissions to use Typescript or Golang, but are open to an implementation in any language of your choosing.


## Requirements
- Allow an API caller to submit a url and receive a shortened url 
  - (e.g. http://localhost/eg041x )
- Allow a user to navigate to a shortened url and be immediately taken to their original url 
  - (e.g. http://localhost/eg041x should redirect to https://www.google.com/search?q=bitly+shortener&ei=ZPvSY_yCH9yv5NoPsvuTwAM&ved=0ahUKEwj8xMmjoeb8AhXcF1kFHbL9BDgQ4dUDCBA&uact=5&oq=bitly+shortener)
- Allow an API caller to hit a `/stats` endpoint that returns paginated JSON information corresponding to the database entry. 
  - A stats object should include the shortened url, the original url and the number of times a user has visited the shortened url
  - A user should be able to submit query parameters such as `limit` and `offset` to paginate over the table and retrieve results
- Use a persistent data store/volume (Postgres or Mysql is encouraged, but any data store will suffice)
- Allow an API caller to update the underlying original url given a shortened url slug and reset the redirect count
- Only allow valid urls to be created 
  - (e.g. `https(s)://(domain)/`)
- High throughput. Allow a minimum of 20 shortened link redirects per second. This will be tested on an M1 Macbook pro with 16GB of RAM


## Deliverables
- Implement your solution, including test cases for the application code (integration tests are a plus)
- Include a `README.md` that describes how to set up, run and test your application
- Include any notes for our engineering team that describes your approaches and assumptions
- Email your point of contact that sent you this exercise with a link to a public Github or Gitlab repository.
    - If you are uncomfortable adding this project to your public Github profile, please make a separate account for this submission

## Notes
- The preferred method of running this project is a `Dockerfile` or `docker-compose.yml` that does not require the takehome consumer to install anything to run and evaluate the project
- Please show us strengths of your engineering abilities, technical design and attention to detail. While small/simple, this takehome is the main way we will assess your technical abilities. 