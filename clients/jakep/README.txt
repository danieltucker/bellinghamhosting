NORTH LINE TOWING — website design package
==========================================

WHAT'S IN HERE
--------------
index.html          The three design directions (1A, 1B, 1C), each shown
                    at desktop width and at 390px mobile width.
options-brief.html  The client-facing brief: differences, pros and cons,
                    recommendation, market notes, competitor landscape,
                    and positioning.
photos/             The truck photos, cropped to the ratios used in the
                    designs, plus the two originals.


HOSTING THESE
-------------
Both HTML files are fully self-contained — fonts, images, scripts and
styles are all embedded. Upload them anywhere and they work. No build
step, no server-side anything, no dependencies.

On bellinghamhosting.com (or any cPanel-style host), drop both files into
public_html/ and they'll be reachable at:

    yoursite.com/index.html
    yoursite.com/options-brief.html

First load takes a second while the page unpacks itself; you'll see a
small placeholder tile until it does. That's normal.


IMPORTANT — THESE ARE DESIGN PRESENTATIONS, NOT THE FINISHED SITE
-----------------------------------------------------------------
index.html is a comparison canvas showing three options side by side. It
is not the live website. Once a direction is chosen, that one option gets
built as a real standalone page.

Two things that are visual only in these files and need wiring up on the
real site:

  1. The quote-request form in option 1B. Right now it's a mockup. On the
     live site it needs to actually send — either a mail handler on the
     host, or a form service like Formspree / Basin.

  2. The nav links (Services, Coverage, About) don't scroll anywhere yet.

Everything else is real: the phone number is a tel: link that dials on a
phone, and the email is a mailto: link.


PHOTOS
------
photos/truck-front.jpg   original, full resolution
photos/truck-side.jpg    original, full resolution

The rest are crops generated from those two:
  *-wide.jpg   wide banner crop
  *-43.jpg     landscape crop
  *-tall.jpg   portrait crop (used in the mobile heroes)

To swap a photo, replace the file and re-generate the bundle — or, in the
design tool, drag a new image straight onto any photo area.


CONTACT DETAILS USED THROUGHOUT
-------------------------------
North Line Towing
3836 H Street Rd, Blaine, WA 98230
360-778-9869
northlinetowingpnw@gmail.com
USDOT No. 7188992
UBI 606245666-001-0001
$1,000,000 liability insured
