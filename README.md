[README.md](https://github.com/user-attachments/files/32617539/README.md)
VUP-19 Personnel Readiness Dashboard

Fiscal Year 2026 personnel readiness report with desktop and mobile layouts.

Files

● index.html — complete website, including styles, JavaScript, images, and the bundled 3D aircraft viewer.

● README.md — setup and maintenance instructions.

No installation, build command, API key, or separate asset folder is required.

Open locally

Download index.html and open it in a modern browser. Choose Mobile or Desktop when the report opens. Use Change view to switch later.

The rotating aircraft uses WebGL. The report tables and controls use standard HTML and JavaScript.

Upload to GitHub

1\. Create a repository or open the repository you want to use.

2\. Upload index.html and README.md to the repository root, not inside a subfolder.

3\. Commit the files to your publishing branch, normally main.

Publish with GitHub Pages

1\. Open the repository’s Settings → Pages.

2\. Under Build and deployment, choose Deploy from a branch.

3\. Select main (or your publishing branch) and / (root).

4\. Click Save.

5\. When deployment completes, open the site link shown in Pages settings.

For a standard project repository, the address typically follows https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/.

See GitHub’s publishing-source instructions.

Report pages

1\. Personnel Readiness Summary

2\. Retention / Attrition Report

3\. E4–E5 Advancement Statistics

4\. E5–E6 Advancement Statistics

5\. Education Completion Report

Desktop mode uses sidebar navigation and full tables. Mobile mode uses a report dropdown, labeled table cards, larger touch targets, and resized header visuals.

The summary strength clocks cycle through Command Wide, SEA, and SHORE every 10 seconds. Reduced-motion settings disable automatic cycling. The display buttons also allow manual selection.

Updating the report

Edit index.html, then upload the revised file to the same repository path. GitHub Pages republishes changes committed to its configured source branch.

Search within the file for these data objects:

● commandStrengthData — personnel counts, Not FFD counts, and command-only additions.

● advancementData — advancement and PNA results.

● educationData — degree completion and college participation.

Other report text, retention figures, and some summary cards are embedded directly in the HTML or their related scripts. Update those displays when revising the underlying figures.

Keep unavailable values as null; do not convert them to zero. The internal uic50470\_50471 key is retained for compatibility with the SEA display, which currently uses the supplied UIC 50471 counts.

The SHORE combined degrees-plus-college-participation calculation adds the two supplied counts. The overlap between enrolled Sailors and degree holders has not been supplied; it is not a confirmed unique-person count.

Maintenance checks

After making changes, check both layout choices, all five report pages, the Command Wide/SEA/SHORE filters, and both degree-table display options. If an older version appears after an update, refresh the page or clear its cached copy.

Third-party component

The aircraft viewer includes Three.js r169. Its MIT license notice is retained inside index.html.

