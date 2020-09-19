# Class Project Links

Due to the liability of current and/or future students copying my work, my actual code files are in a private repository. I am more than happy to give access to this repository upon request, as long as you will not use or allow others to use this code (intentionally or not) for CSE courses offered at my school.

**Note:** The EC2 instance hosting these websites has been shut down, so the links are no longer active.


## Calendar

### Description

This project allows a user to register for an account and make events for any date they choose. It includes a dark mode that saves the preference for each registered user, alerts that appear when the user logs in for every event within 3 days, and important events are colored red. Usernames and passwords are salted and hashed for security (there were other security measures taken but this one was especially important). This was an opportunity to learn JavaScript and how to integrate it with PHP (and MySQL). My partner and I made this in roughly 28 hours. 

### Room for Improvement

Many, if not all, of these items were a necesseray calamity due to the time restriction for creating this project. Also there are certainly many more ways to improve, but these are ones that I find to be very noticable to the user and not requiring a fundamental change to the design of the code.
* Visuals show that shouldn't when the page first loads, but quickly disappear.
* Better user feedback (e.g. user doesn't know if they were registered unless they have the console pulled up).







## News Sharing Site

### Description

This project allows a user to view stories and comments posted by registered users. If a user wants to get access to these *awesome* features, they can register and login. Once logged in, the user can create, edit, and delete their posts. Each story has a title, content, and optional URL. Logged in users can also like stories and order the list of stories by date posted or likes. This was my first project integrating MySQL with PHP. Usernames and passwords are salted and hashed for security (there were other security measures taken but this one was especially important).

### Room for Impovement

* The general look and layout could be greatly improved (but visuals were not the goal of this project).
* The text boxes for creating/editing titles, content, and comments could be increased in size for user readability.
* There are no client-side scripts so all updates are done by changing or refreshing pages, but again, the goal of this project was integrating MySQL with PHP. Ideally this overhaul would be made in future updates.




## Movie Searching iPhone App

### Description

This project allows the user to search for movies contained on The Movie Database. The can also select each movie to view more details and save them to their favorites. Additionally, they can search their favorites, as well as delete movies from their favorites. This project's goals were to use multithreading to keep the user interface from locking up during API requests, as well as learning about some of the common features of iPhone applications, such as Tab Bars and Collection Views. It was also an introduction to the plist so that favorites can be maintained between app launches.

### Room for Improvement

* There's some overcomplicated logic used to allow movies to be added and deleted from the favorites tab while a search (filter) function is in place. This stems from storing my movies in the plist by id when it would be much easier to encode the date and archive it so that I could use data structures like dictionaries in favorites.
* The searching takes too long in my opinion which is due to a variety of reasons, but one in particular is that it makes multiple API requests for the same page to account for posters that TMDB doesn't upload on the first try. Optionals could have been safely unwrapped to allow this to be okay, but there was a grade in my class associated with the same display appearing for the same search. Points would have been lost here since a poster could only be delivered for certain movies after usually at most three tries. There is a better description of this in a comment above the function that makes these requests. I'd prefer to miss the picture on the first load but have the movies load quicker.
