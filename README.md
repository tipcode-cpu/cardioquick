# CardioQuick PWA V11

Changes:
- Restored the individual per-field "copy" buttons in the PREVENT input grid (Age, Sex, Total-C, HDL-C, BMI, eGFR, UACR) — they were only hidden by CSS, now visible again
- They coexist with the "Autofill from above" button, which fills all available fields at once
- Added missing type="button" on the BMI/eGFR copy buttons for safety
- (from V10) "Copy all" / "Autofill from above" now actually fills the PREVENT inputs
- (from V9) ZIP->SDI lookup moved to external packed file zip-sdi.txt; index.html ~54 KB

After upload, test (hard-refresh / clear site data if the old service worker is cached):
https://tipcode-cpu.github.io/cardioquick/?v=11

Files to deploy: index.html, manifest.json, service-worker.js, icon.svg, zip-sdi.txt
