# Kassel Quantitative Research Hub — Stage 5 Build

**Created by Raja Rub Nawaz**

A deploy-ready static website based on the 6 November 2026 V3.0 Kassel SPSS & SmartPLS master catalogue, with **109 resource records**, **12 learning modules**, and **25 steps across three student pathways**.

## What is implemented
- Responsive home page; twelve module detail pages; three ordered research pathways.
- Search and filter 109 records by topic, module, software, resource type, and teaching tier.
- Instructor-priority sorting: James Gaskin; for SPSS gaps, Mike Crowson, Erin Buchanan.
- Decision-support method finder with design caveats, not automated statistical advice.
- Reporting guidance and **newly generated synthetic-only** TPB survey and experimental CSVs.
- Mandatory exact attribution **Created by Raja Rub Nawaz** immediately under the title and in the global footer on **every page**.
- Public JSON/CSV data export, privacy notes, verified-source labels and explicit pending-video review flags.

## Important quality limitation
This Stage 5 build **does not claim to have live-verified all links or watched all videos**. The 109-row catalogue is preserved; publication-quality verification remains a separate manual check. Video links are visibly labeled playback-review pending. Older tutorials may use earlier software interfaces. The synthetic examples are wholly fictional, not derived from the confidential TPB data.

## Deploy to Netlify at no expected initial hosting cost
1. Unzip the downloaded package into a folder.
2. **Option A (easy):** Netlify dashboard → Add new project/site → Deploy manually → drag the **unzipped website folder** (not the ZIP) into Netlify Drop. The folder must contain `index.html` at its top level.
3. **Option B (GitHub):** Create a new GitHub repository; upload the contents of this folder to the repository root. In Netlify choose **Import from Git** and select it. Set **Build command blank** and **Publish directory `.`**. `netlify.toml` includes the configuration.
4. Confirm all primary navigation items and attribution in header/footer on both mobile and desktop.
5. Open 5–10 representative links and validate video instructor, availability and software version. Review the remaining link list before sending the hub to students.

## Local preview
From this folder, run `python -m http.server 8000`, then open `http://localhost:8000` in your browser. **Do not double-click index.html**: the browser blocks local JSON loading in file:// mode.

## Editing the source catalogue
`data/catalogue.json` is generated from V3.0. It is not a live Google Sheet connection. To maintain the website: update the workbook, rebuild/re-export JSON, then redeploy the site. Do not paste any participant records or protected material into the public data folder.

## Site QA checklist
- [ ] Title attribution exact on every page, including mobile and not-found page.
- [ ] Footer attribution exact on every page.
- [ ] 109 resource cards accessible through filters.
- [ ] 12 module pages and 3 pathways function.
- [ ] Method finder combinations produce relevant qualified options.
- [ ] Downloadable CSV files contain synthetic data only.
- [ ] No confidential dataset, passwords, analytics tracking, or copyrighted PDFs.
- [ ] All video links playback-reviewed; broken links fixed before public release.
- [ ] All external resources checked for current availability and correct attribution.

No live deployment or GitHub modification has been performed by this handoff.

## V5.1 visual update

The site now has a larger, more colorful responsive visual system. The public catalogue CSV export links and file were removed intentionally. The website still loads its public JSON catalogue for in-browser searching. Synthetic practice dataset CSV downloads are retained. The exact creator attribution appears in the shared header and footer.
