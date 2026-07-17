============================================================
 SLN NAVY LIST - iPhone App Package
============================================================

This folder is a complete installable web app (PWA). Once
installed it opens full screen from its own icon, works
OFFLINE, and parses the Navy List PDF entirely ON THE PHONE.
No Navy data ever leaves the device - the hosted files are
only the empty app itself.

FILES
  index.html            the whole app (pdf.js built in)
  manifest.webmanifest  app name / icon / full-screen config
  sw.js                 offline cache (service worker)
  icon-180/192/512.png  home screen icons

------------------------------------------------------------
 INSTALL AS A NORMAL iPHONE APP  (one-time, ~10 minutes)
------------------------------------------------------------
iPhone home-screen apps must be served from a website (an
Apple rule), so host these files once on any free host.
GitHub Pages is the easiest:

 1. Create a free account at github.com
 2. Click "+" > "New repository"
      - Name: navylist   - Public   - Create
 3. "uploading an existing file" > drag ALL files in this
    folder > Commit changes
 4. Repository Settings > Pages > Branch: main > Save
 5. Wait ~1 minute. Your app URL appears, e.g.:
      https://<your-username>.github.io/navylist/
 6. Open that URL in SAFARI on your iPhone
 7. Tap Share (square-with-arrow) > "Add to Home Screen" > Add

Done. The anchor icon appears on your home screen. It opens
full screen with no browser bars, and after the first visit
it works with no internet at all.

------------------------------------------------------------
 USING THE APP
------------------------------------------------------------
 - Tap "Open Navy List PDF" and pick the PDF from Files
 - First parse of 450 pages takes ~1-2 minutes on the phone;
   after that the same PDF loads instantly (saved on device)
 - Search any mix of: Official No. / Surname / Branch /
   Intake / Retirement Year. Tap a card for the full record.
 - "Export CSV" shares the current results

------------------------------------------------------------
 NO-HOSTING FALLBACK
------------------------------------------------------------
index.html also works on its own: save it to the Files app,
long-press > Share > open in Safari. Everything works the
same; it just won't have its own home-screen icon.
============================================================
