# Tachiyomi
### Madilyn Simons

## Project Abstract
Tachiyomi is a free and open source manga reader for Android.  It allows users
to read manga from various online sources, download manga, and organize and
categorize your own library of manga.  The application allows users to explore and browse a variety of manga sources, as well as keeps track of manga a user has already read or plans to read.  The reader itself can be configured and adjusted to the users' liking and personalized with themes.

## Project Relevance
_Object Oriented Programming_ <br />  
Android development requires object-oriented programming.  Android applications use objects and classes to implement activities, widgets, and functionalities.  This particular application is written in Kotlin, an object-oriented programming language.

_Test Driven Development_ <br />  
As we would be implementing new features to the application, it is important to use test driven development to ensure high-quality work and implementations.  By using TDD, we can create reliable and functional code.

_Graphical User Interface_ <br />  
Users interact with Android applications using the graphical user interface.  As such, we would need to implement features using the graphical user interface.  Our function calls would need to ultimately connect to the GUI so that the user may utilize our new features.

_Modern Software Development_ <br />  
Implementing features requires multiple steps and components.  As such, it's good to manage the project in such a way that allows different developers to be able to independently work on respective components that will eventually link together to create a new feature.  Version control will allow developers to work concurrently.  Building, testing, and issue tracking will ensure high-quality and organized code.

_Open Source_ <br />  
Tachiyomi is an open source application.  We will use GitHub to access and modify the source code.  Eventually, we can aim to create a merge request and ultimately contribute our feature to the original project.

## Conceptual Design
As developers, we should always aim to create more accessible and inclusive software.  Tachiyomi allows readers to view pages of manga, but a more accessible version of the app would include a text-to-speech feature.  This feature would be helpful for visually-impaired manga fans as well as young fans who may not know how to read yet.

Tesseract Android Tools is a library of tools that uses Optical Character Recognition (OCR) to convert images of text to actual text.  By utilizing Tesseract Android Tools, we could implement a feature that allows users to click on speech bubbles in order to play an audio reading of the text in the speech bubble.

Such a feature would likely require the following components:
- A function that, given a list of coordinates, would (1) display bounding boxes on the screen and (2) return the coordinates of a bounding box that is selected by the user.
- A function that, given the coordinates of a bounding box, would be able to
crop the image displayed on the screen and return that cropped image.
- A function that, given an image, would pass that image into Tesseract and return the text returned by Tesseract.
- A function that, given text, would play a text-to-speech audio of that text (probably using Android's built-in TextToSpeech class).

## Background
https://github.com/tug34641/tachiyomi

## Required Resources
- Group members
- Android Studio
- Tesseract Android Tools
- Experience in Kotlin
- Experience in Android development

## Project Voting and Feedback
_Oppia_ <br />  
https://github.com/3296f19temple/allprojects-section05-aldwairi-tr-11am/issues/7#issuecomment-541849259 <br />  

I'm interested in this project because it is working for a really good cause. I appreciate open-source projects for social good and it sounds like Oppia could be very helpful for a lot of people.

I'm a strong Python programmer so I would be able to contribute to any back-end issues. I see all of the pinned issues right now have to do with refactoring and testing and I could help with those issues.

_DuckDuckGo_ <br />  
https://github.com/3296f19temple/allprojects-section05-aldwairi-tr-11am/issues/1#issuecomment-541843479 <br />  

I'm interested in this project because I regularly use DuckDuckGo and would love to give back to the developers that work on it. DuckDuckGo is a very reliable search engine and I like having a secure alternative to Google. I am interested in contributing to this project as DuckDuckGo is a reputable product that I use frequently.

I have a good amount of experience with Android development so I could easily assist with any Android-specific issues. Just going through the issues in the repository, I see that there are some issues that look specific to the app's GUI that I could help with:

- duckduckgo/Android#237

There are multiple feature requests in the issues and I'd be happy to work on almost any of those.

## Feature List:
- We will be adding a text-to-speech option for pages of manga in Tachiyomi.  
Essentially, there will be a functionality that allows users to hear a voice
reading the words on whatever page the user is currently reading.  As
the application currently stands, users may only look at pages and read the
text for themselves.  This feature would give them the option to list to
the text out loud.  Such a feature would likely require the following components:
    -  A function that, given a list of coordinates on the screen, would display
    bounding boxes on the screen.
    -  A function that would return the coordinates of the bounding box
    that is selected by the user.
    -  A function that, given the coordinates of a bounding box, would crop the
    image displayed on the screen and return that cropped image.
    -  A function that, given an image, would pass that image into Tesseract
    and return text text returned by Tesseract.
    -  A function that, given text, would play a text-to-speech audio of that
    text (probably using Android's built-in TextToSpeech class).


### (Persona 3) Rose Bud
- Personalization
    -  Rose is a five-year-old kid who loves anime and is interested in
    manga, but hasn't learned how to read yet.
- Education
    - Rose is in kindergarten.  She is relatively tech-savy as she owns her own Android and frequently uses the family computer.  However, as she is very
    young and hasn't had much schooling, she does not yet know how to read.
- Job-Related
    - Rose does not have a job.  She is a young girl and one of her favorite
    ways to spend her free time is by watching anime and drawing pictures.
- Relevance
    -  Rose can't read, but she loves anime, so she would like to extend on her
    interest and start reading manga.  However, she does not yet know how to
    read.  She wants to know what happens to her favorite characters in manga
    and she wants more stories, but she cannot read manga for herself.      Tachiyomi's text-to-speech option is incredibly helpful for Rose, because
    it allows her to enjoy her favorite manga and enjoy stories about her
    favorite anime characters without having to know how to read.

### Insights, Feedbacks, Expectations
- Our proposal is solid.  We are proposing a useful functionality along
with a practical design for it.  This project tackles a few advanced programming
areas, such as mobile development, object oriented programming, and optical
character recognition.  Our project is a really good opportunity
for us to be immerse ourselves in these topics.  This particular project also
lends itself well to being broken into smaller tasks.  This allows us to
approach such a large problem with relative ease and smoothness.
- Each member seems to have a strong understanding of our goal for Tachiyomi and
we have yet to experience any major challenges or road bumps.  I'm glad that
other members have creative ideas for contributions to Tachiyomi or different
ways to tackle our problem.  Going forward, I expect each member to equally
contribute to our project, reach out for help if they need it, and offer advice
to any group member that may need it.