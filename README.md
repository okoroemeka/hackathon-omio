# Fern & Nah — affiliate demo

A fictional German travel blog for demonstrating the AI Widget Builder outside
the portal. Static HTML and CSS only, with an inline SVG illustration. No external
assets, dependencies, tracking, API calls, or booking requests.

## Open locally

Open `index.html` in your browser, or serve this folder:

```sh
cd /Users/emeka.okoro/Desktop/b2b/hackathon-omio
python3 -m http.server 8088 --bind 127.0.0.1
```

Visit http://localhost:8088. Stop with Ctrl+C.

## Embed the widget

1. Generate a German train widget from Munich to Salzburg, departing 6 November
   2026 and returning 8 November 2026. Use cream `#FFF4DF`, navy `#123456`, and
   purple `#8040C0`. Update dates if recording after them.
2. Apply and copy the portal's complete Code Example.
3. Ensure the loader, CSS, location services, and search destination all use
   approved QA or local/mock services. The portal currently generates production
   bundle URLs: **do not paste that snippet unchanged**. Changing only the loader
   URL is insufficient if the bundle still calls production APIs.
4. In `index.html`, replace the entire `div.embed-placeholder` inside
   `div#affiliate-widget` with the approved snippet, including its script and
   `data-omio-widget` element. Keep the outer `div#affiliate-widget`.
5. Reload. Verify the route, dates, colours, and browser Network panel. Do not
   submit a real booking search. Update the disclosure once the placeholder has
   been replaced to accurately describe the QA/mock widget.

Until then, the page shows a labeled, non-interactive placeholder, not a live
Omio widget. No production dependencies are loaded by this page.

## Demo sequence

Show article → generate in portal → review → apply → copy QA-approved snippet →
embed here → reload the blog.

The German article supports automatic language detection. For branding, append
this sentence when pasting into the builder: “Die Verbindungssuche soll zu unserem
Magazin passen: cremefarbener Hintergrund (#FFF4DF), dunkelblauer Text (#123456)
und violette Schaltflächen (#8040C0).”
