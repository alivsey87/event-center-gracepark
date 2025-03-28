# EVENT CENTER PROJECT: Grace Park
---
---

#### For this project, I decided to make a website for a center called Grace Park that hosts concerts for Christian music artists! Hopefully this README explains a lot of what is going on in the coding and it is organized.

---
---
---


## TABLE OF CONTENTS

1.[Background](#1-background)

2.[Home Page](#2-home-page)

3.[Events](#3-events)

4.[Menu](#4-menu)

5.[Location](#5-location)

6.[Contact Us](#6-contact-us)

## 1. Background

I decided to have an image of a concert be the background for the entire site, but also be a part of the hero image. Through a LOT of trial and error (background-* property experimenting), I figured out how to make the background image stay fixed during scrolling and positioned it to allow the performer in the photo be sort of another part of the hero image.

---
---

## 2. Home Page

### Body

Every page is contained in a flex-box container under the "main-container" class. Will only include this "Body" section once on the README since it applies to all pages.

### Header

Header includes the following:

- #### ANNOUNCEMENT BAR

  - A flex-box with a black (90% opacity) background. The text is a `<p>` with a blinking animation to attract attention to it.

- #### NAVIGATION BAR

  - A flex-box to hold the menu items. The background has a linear gradient to fade from transparent to 60% opacity black. A 6-column grid holding the menu items is the only item in the flex-box and is justified to the right. Everything aligned center.

Will only include this "Header" section once on the README since it applies to all pages.

### Main

Main content holds:

- #### HERO IMAGE/LOGO

  - I designed a basic logo using a font called "Lincoln Electric" to pair with the background image.

- #### FEATURED EVENT

  - Used a flex-box container to hold a main featured image and an "info" block showcasing one of the events, including a button/link to the Events page. There was a good amount of experimenting on the image container and image to get the photo to fade out to the right. This:
    ```css
    mask-image: linear-gradient(to right, black 40%, transparent 70%);
     ```
    accomplished that!

- #### ABOUT US

  - Basic `<h1>` and `<p>` for an "About Us" section.

- #### FOOTER

  - Every page includes the Footer. Just a basic `<p>` with a copyright and name event center. Will only include this "Footer" section once on the README since it applies to all pages.

---
---

## 3. EVENTS

### Main

Main flex-box container that holds:

- #### EVENT CARDS
  - Each card is a flex-box and has an image item with it's own id for specific styling since each image has a different pixel size and I had to fit each into a 250 X 220 box. The other two items are simple `<h3>` items for event info.

---
---

## 4. MENU

### Main

A main flex-box container containing a table with 3 `<th>` elements for the "Food" "Snacks" and "Drinks."

---
---

## 5. LOCATION

### Main

A simple `<div>` with a bunch of `<p>` elements to describe the location and hours. Included an image of a Google Map as well.

---
---

## 6. CONTACT US

### Main

A flex-box (probably could've just used a normal `<div>` here) that includes a another flex-box for the form. Separated the text inputs, textarea and submit input into their own items in the flex-box. Added a nice bit of styling to the Submit button.

---
---

## 7. MISCELLANEOUS CSS

### Theme

The visual theme of the website is centered around the background image of the performer on stage. Because of the colors, I decided to use transparent black elements. The folowing color is used *very* often:
```css
background-color: rgba(0, 0, 0, 0.6);
```
The home page was *TRICKY* for me. I wanted to have the featured section have an image that blended into the background color (the code mentioned [here](#featured-event)) and I kept running into issues sizing the image and cropping it correctly. After some trial and error I came up with this:
```css
.feat-image {
    object-fit: none;
    object-position: -320px -130px;
}
```
The image itself is rather large and I discovered that I had to set negative value positions to get it just right.

I also decided to make the font consistent throughout with this code:
```css
font-family: Arial, Helvetica, sans-serif;
letter-spacing: 0.05rem;
```
Also, setting the color to white.

### Media Queries

I feel like I had to create way too many variations of classes for the viewport sizes, *particularly* the 950px size. Something to consider for future projects.

[back to top](#event-center-project-grace-park)