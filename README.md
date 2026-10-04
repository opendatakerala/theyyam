# Theyyam Calendar Project – website

Files
- index.html – search, calendar and map (reads data/theyyam.geojson)
- submit.html – form for adding a Theyyam event;
- data/theyyam.geojson – the site's data (currently SAMPLE data – replace it)
- images/ – event notices, posters and photos (file names match the JSON)
- assets/logo.png, assets/favicon.png – Muchilottu Theyyam logo

Updating the data
1. Save the JSON files received by email.
2. Open submit.html > "For maintainers: build the website data file".
3. Select the current data/theyyam.geojson plus the new JSON files, click Build.
4. Upload the downloaded theyyam.geojson to data/ (sample entries are dropped automatically).

Links and images
- Add a Wikidata QID to a kavu and the site shows its Wikidata image (P18) and links to
  Wikidata, Malayalam and English Wikipedia.
- Deep links: index.html#date=2026-10-12 opens that day; index.html#kavu=<id> opens a kavu.

Event notices / posters
- Images go in the images/ folder, named exactly as in the JSON "image.file_name"
  (the form already renames them, e.g. images/Theyyam20260001.jpeg).
- They show as thumbnails in search results, the calendar and map popups, and full size in
  the kavu details. If an image file is missing, the site simply hides it.

Languages (English / മലയാളം)
- Both pages have an English / മലയാളം switch at the top. The choice is remembered on the
  visitor's device and carries across pages. Links can force a language: index.html?lang=ml
- All interface text is in the I18N block near the end of index.html and submit.html
  ("en" and "ml"). The block is the same in both files; when you change wording, change both.
- Data is shown as entered: kavu names appear in the chosen language first, the other second;
  ritual types like "Thottam (തോറ്റം)" show the matching half.
