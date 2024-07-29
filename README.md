# CS50-Project 2 - Commerce 


The aim of this project was to build a E commerce like ebay using Python Django frameworkthat will allow users to post auction listings, place bids on listings, comment on those listings, and add listings to a “watchlist.”


## Youtube short Video
In a brief video: [[https://youtu.be/eS77gFwXCPY](https://www.youtube.com/watch?v=CQIvu1EJshQ&t=5s&ab_channel=Luana)](https://youtu.be/yb9nEL2wU1U)
I will walk you through the essential specifications for the project. This video aims to provide a concise overview of the required elements

## Technologies:
**Back-end:**
SQLite
Python
Django

**Front-end:**
HTML (with Django templating)
CSS (with some Bootstrap Components)

## Project Summary:
This project fulfills the following requirements:

**Models**
The application has at least three models in addition to the User model: one for auction listings, one for bids, and one for comments made on auction listings. Also, I add fields for each model as needed.
Create Listing: Users are able to visit a page to create a new listing. They are able to specify a title for the listing, a text-based description, and what the starting bid should be. Users also are optionally able to provide a URL for an image for the listing and/or a category (e.g. Fashion, Toys, Electronics, Home, etc.).


**Active Listings Page**
The default route of the web application lets users view all of the currently active auction listings. For each active listing, this page should display (at minimum) the title, description, current price, and photo (if one exists for the listing).


**Listing Page**
Clicking on a listing takes users to a page specific to that listing. On that page, users are able to view all details about the listing, including the current price for the listing.
If the user is signed in, the user is able to add the item to their “Watchlist.” If the item is already on the watchlist, the user is able to remove it.
If the user is signed in, the user is able to bid on the item. The bid must be at least as large as the starting bid, and must be greater than any other bids that have been placed (if any). If the bid doesn’t meet those criteria, the user is presented with an error.
If the user is signed in and is the one who created the listing, the user has the ability to “close” the auction from this page, which makes the highest bidder the winner of the auction and makes the listing no longer active.
If a user is signed in on a closed listing page, and the user has won that auction, the page will say so.
Users who are signed in are able to add comments to the listing page. The listing page displays all comments that have been made on the listing.


**Watchlist**
Users who are signed in are able to visit a Watchlist page, which displays all of the listings that a user has added to their watchlist. Clicking on any of those listings takes the user to that listing’s page.


**Categories**
Users are able to visit a page that displays a list of all listing categories. Clicking on the name of any category takes the user to a page that displays all of the active listings in that category.


**Django Admin Interface**
 Via the Django admin interface, a site administrator is able to view, add, edit, and delete any listings, comments, and bids made on the site.

## Usage Instructions:
**Requirements:** Python(3) and the Python Package Installer (pip)

**Installation:** Install requirements (Django4): pip install -r requirements.txt
After cloning the repository, refer to the project folder and:
- Create new migrations based on the changes in models: python3 manage.py makemigrations
- Apply the migrations to the database: python3 manage.py migrate
- Create a superuser to be able to use Django Admin Interface: python3 manage.py createsuperuser
- Run the app locally: python3 manage.py runserver
