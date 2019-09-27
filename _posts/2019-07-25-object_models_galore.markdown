---
layout: post
title:      "CLI Project: Wedding Venues"
date:       2019-07-25 10:06:34 -0400
permalink:  object_models_galore
---


**Prelude of Project**

Before I started on my project I was challenged with another life project, to find a wedding venue for my wedding.
My wedding is 4 months away and I've gotten the escalating pressure of finding a venue for my wedding and reception. On top of that I have been trying to think of what website to scrape for my project .

I was looking for list of reception venues in Northern California, my hometown, but living in Northern Virginia, I needed to heavily rely on my research online. I came across one website that was called Wedding Wire. As I looked through the list, I thought that maybe I can combine my search for wedding venues and my project. I talked with Beth, my project advisor, if this was a scrapable site. We got to take a look at the website but saw that it wasn't scrapable. She told me not to be disheartened but to see the next website, we looked at Wedding Spot, which was absolutely scrapable, and now both my venue search and CLI project was able to begin!

**Beginning of Project**

I began with creating a repository in github and also watching videos on how to create an IDE In Browser. After my repository of wedding-venues was pushed, I got to the files that I needed to edit before I started on my project, such as having a good README.md with a short description of my project, installation instructions, a contributors guide and of course the MIT license.

After I completed the basics I noticed how I had 2 modules that was "wedding" and "venues. I was confused as this wasn't suppose to happen. I asked Beth and she shared with me it's because of the "-" in between "wedding-venues". She showed me how to correct this by combining the modules and editing my binary and library folder. After we ended our conversation, my Sandbox went blank and reset itself. This is when I learned the importance of committing early and often.

I got to fix the folders but I committed often and early.

Now I was ready to compose my code.

I didn't know where to begin so I looked at examples of past projects such as "Eden Events", " Daily-Deals" and "World's Best Resturants". I was able to see the code that they had utilized to make their basic CLI Gem. Their code was straightforward and simple but different depending on variables of the website they were scraping and also depending on what they want their user to experience.

I would start with the basics of having 3 classes:

* The CLI: For the user to interact with the application, this is what is going to be displayed to the user.
* The  Scraper: This is to grab the information from the website I was using, wedding-spot, and add it to my data.
* The Data: This is to list all the data of information I want from the website.

At first I thought I could have my data and scraper combined in one file but it began getting messy so Dustin suggested I separate the Scraper class and the Data class. I created 3 files under my ./lib/wedding-venues folder: 
CLI, Scraper and Venue.

I then created a Notes.md file to organize my thoughts and goals for my CLI. I thought about, what did I want my CLI to do and show to my user, like me who's getting married. I looked at the website and jotted things I wanted to show the user, such as name, location, URL and short description. I wanted it short and sweet for my user.

**Hello World!**

I worked on my CLI file, trying to figure out what I wanted it to say. First I created my file to say "Hello World!" to see if my CLI would work. I typed my class into my console and it displayed back "Hello World!".

I then decided how I wanted to structure my responses as so:

* Welcome!
* Title
* How can I help you?
* Here's the list of venues
* Want more information
* Again?
* Goodbye

I typed in the puts of how it will respond and at what turn, so I created my method "call" and created my list of how it will respond.
The "call" was working.

**Scraper**

However, I can't leave it just so, or it wouldn't be up to date with the new venues that open in Northern California.
This is when I had to start adding my scraper class to have my method to open up wedding-spot website with the parser tool, Nokogiri. 

After including the method to retrieve my website, I proceeded to make a method that would scrape the list of wedding venues, "scrape_venues_index".
After creating that method, I created another method that would send the information to my Venue Class.

**Venue**

The Venue Class is now ready to begin, I started initializing the list of information I wanted to display: name, location, description, and URL.
After a long struggle of trying to locate the information and utilizing my terminal to see if the code was valid and return the information, I included it to the index page I've created. I added the setter and getters for each information as well and was now ready for my CLI to take that information.

**Going back to CLI**

Now that my data is set and retrieving the information, I went back to my CLI class and included the methods to call the information based on how I wanted the CLI to interact with the user. I created the list of methods that I wanted to go in order and then I included what the methods will each do.
The struggle was the amount of venues would be displayed so I would go back to my venues class and limit it to just 10.
I also had the struggle of input, where if I included anything that is above the number that was listed it would create an error. Dustin helped me to see that I can aslo include that into my if statement so that the method would not create an error. Finally, I used the time to make the CLI look nice and changed wording so that it would be fun for my user.

**Conclusion of Project**

I am amazed that I actually created an application by myself. Although creating the interactive Tic Tac Toe game was harder and I needed a lot of help, creating my own application for something that I need made the experience worthwhile. Helped me to reevalute if I actually am enjoying learning how to code. I really do and its with a lot of struggle and asking for help but if its to help some harried woman finding a venue it is very worthwhile.

