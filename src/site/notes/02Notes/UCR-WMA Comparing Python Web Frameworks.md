---
{"dg-publish":true,"permalink":"/02-notes/ucr-wma-comparing-python-web-frameworks/","tags":["notes/atomic"]}
---

There are three main web frameworks used in python that being 

1. [[02Notes/Flask\|Flask]]: Lightweight, flexible, highly customizable. It is built in a [[02Notes/Asynchronous Programming\|Synchronous]] nature. It is great for quick, fast, prototyping (this is how I first learned web development so it has a special place in my heart)
2. [[Django\|Django]] : Used to build complex web applications such as routing, authentication etc. and offers a variety of built in tools. 
3. [[02Notes/UCR-WMA FastAPI Intro\|FastAPI]] : Modern Framework, built in [[02Notes/Asynchronous Programming\|asynchronous nature]], gaining a lot of popularity (to the point where it is the highest GitHub star count of all 3 which was not the case when I first learned FastAPI)


**For more in-depth comparison**:
- [FastAPI, Flask or Django - Which Should You Use?] (https://www.youtube.com/watch?v=cNlJCQHSmbE )


## Who is using what?

The following is just some examples of companies that use specific frameworks. 

A thing to note is that none of these companies use just **one** tool. Usually it is a collection of different tools, and when developing anything take into account what is most applicable to the goal of the project. 

As of the end of October 2025, here are the GitHub star counts: 
- Django: 86 thousand 
- Flask: 70.8 thousand 
- FastAPI: 92 thousand

### Django
An article on companies that use Django [15 Famous Sites that Use Django](https://intellisoft.io/15-famous-sites-built-with-django-that-you-probably-know/?utm_source=chatgpt.com) read it if you are interested, here are some of the highlights
- Instagram
- Spotify
- Pinterest
### Flask
An article on companies that use Flask [Companies that use Flask](https://careerkarma.com/blog/companies-that-use-flask/?utm_source=chatgpt.com) 

- Reddit
- Uber
- Netflix
### FastAPI
[Companies that use FastAPI](https://www.planeks.net/companies-using-fastapi/?utm_source=chatgpt.com)

- Microsoft
- Netflix
- Uber

## Micro Framework vs Built In Tools

Both Flask and FastAPI are considered **micro-frameworks** because it does not include many of the built in features that other frameworks like [[Django\|Django]] have.  

Being a microframework does not mean it is less capable, instead it provides the essentials to get a web application up and running.

Allowing the developer to pick and choose the **extension** as needed creating a lean stack with no bloat and exactly what you need.

Finally working on a lighter weight framework has its advantages as many of the skills are easily transferable and you get a deeper understanding of how things operate. You can think of larger framework essentially getting a lot of the initial building for you. 