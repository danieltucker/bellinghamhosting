NORTH LINE TOWING — website package
===================================

WHAT'S IN HERE
--------------
index.html                      Start here. Mobile-friendly chooser page
                                linking to the three options.
option-1a-rugged.html           Option 1A — charcoal + safety amber, photo-led.
option-1b-professional.html     Option 1B — navy + brick red, with quote form.
option-1c-urgent.html           Option 1C — black + hazard yellow, minimal.
options-brief.html              Client-facing brief: differences, pros/cons,
                                recommendation, market notes, competitors.
photos/                         Truck photos, cropped to the ratios used,
                                plus the two full-resolution originals.


HOSTING
-------
Upload the whole folder (all HTML files plus the photos/ folder) into
public_html/ on bellinghamhosting.com, keeping the structure intact.
Pages will then be at:

    yoursite.com/                          → the chooser
    yoursite.com/option-1a-rugged.html
    yoursite.com/option-1b-professional.html
    yoursite.com/option-1c-urgent.html
    yoursite.com/options-brief.html

These are plain static HTML files. No build step, no server-side code, no
database, no JavaScript framework. Fonts load from Google Fonts; images
load from the photos/ folder next to the HTML.

Once a direction is chosen, that option becomes index.html and the other
two come out.


ALL THREE ARE FULLY RESPONSIVE
------------------------------
Each option is built mobile-first and tested from 320px up to desktop:

  - Type, spacing and images scale with the screen.
  - Every option has a call bar pinned to the bottom of the screen on
    mobile, so the phone number is always one tap away.
  - Tap targets are at least 44px tall throughout.
  - The phone number is a tel: link (dials on a phone) and the email is
    a mailto: link.
  - Motion respects prefers-reduced-motion.


ONE THING TO WIRE UP: THE FORM IN OPTION 1B
-------------------------------------------
The quote form in option-1b-professional.html is real HTML and will
submit — but it needs a destination. Right now it posts to a placeholder:

    <form action="https://formspree.io/f/YOUR-FORM-ID" method="POST">

Two ways to finish it:

  1. Formspree (easiest, free tier available). Create a form at
     formspree.io pointed at northlinetowingpnw@gmail.com, then replace
     YOUR-FORM-ID with the id it gives you.

  2. Your host's own mail handler. Most cPanel hosts provide a PHP mail
     script — point the action at that instead.

Until then the form will error on submit. If you'd rather not deal with
it at all, delete the <form> block and the "Request a free quote" button;
the page still works, and the phone number carries it.


PHOTOS
------
photos/truck-front.jpg   original, full resolution (3024x4032)
photos/truck-side.jpg    original, full resolution (4284x5712)

Crops generated from those two, used by the pages:
  front-wide.jpg / side-wide.jpg    wide banner crop
  front-43.jpg   / side-43.jpg      landscape crop
  front-tall.jpg / side-tall.jpg    portrait crop

To swap a photo, replace the file with the same name and dimensions, or
edit the src="..." in the HTML to point at a new file.

Worth adding when you can: a night or wet-weather shot (sells 24/7 better
than any sentence), one of the owner with the truck, and a regular car
loaded on the deck.


DETAILS USED THROUGHOUT
-----------------------
North Line Towing
3836 H Street Rd, Blaine, WA 98230
360-778-9869
northlinetowingpnw@gmail.com
USDOT No. 7188992
UBI 606245666-001-0001
$1,000,000 liability insured

Change any of these with a find-and-replace across the HTML files. The
phone number appears both as display text (360-778-9869) and inside the
links (tel:+13607789869), so search for both forms.
