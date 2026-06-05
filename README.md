# CardioQuick PWA V12

Changes:
- Added a responsive layout for narrow screens (<= 640px), the app previously had no media queries and forced the desktop layout onto phones
- Card grid collapses from 2 columns to 1 column on mobile
- PREVENT input grid collapses from 5 columns to 2 columns (inputs were unusably narrow before)
- Inputs/selects now stretch to fit the screen width instead of fixed pixel widths
- "Autofill from above" button goes full-width on mobile for an easier tap target
- (from V11) individual per-field "copy" buttons restored
- (from V10) "Autofill from above" actually fills the PREVENT inputs
- (from V9) ZIP->SDI lookup in external packed file zip-sdi.txt; index.html ~54 KB

After upload, test (hard-refresh / clear site data if the old service worker is cached):
https://tipcode-cpu.github.io/cardioquick/?v=12

Files to deploy: index.html, manifest.json, service-worker.js, icon.svg, zip-sdi.txt
