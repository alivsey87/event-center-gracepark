# EVENT CENTER PROJECT: Grace Park


## 1. Background

I decided to have an image of a concert be the background for the entire site, but also be a part of the hero image. Through a LOT of trial and error (background-* property experimenting), I figured out how to make the background image stay fixed during scrolling and positioned it to allow the performer in the photo be sort of another part of the hero image.

---
---

## 2. Home Page

### BODY

Every page is contained in a flex-box container under the "main-container" class. Will only include this "Body" section once on the README since it applies to all pages.

### HEADER

Header includes the following:

- #### ANNOUNCEMENT BAR

  - A flex-box with a black (90% opacity) background. The text is a `<p>` with a blinking animation to attract attention to it.

- #### NAVIGATION BAR

  - A flex-box to hold the menu items. The background has a linear gradient to fade from transparent to 60% opacity black. A 6-column grid holding the menu items is the only item in the flex-box and is justified to the right. Everything aligned center.

Will only include this "Header" section once on the README since it applies to all pages.

### MAIN

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