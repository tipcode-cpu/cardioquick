# CardioQuick PWA V10

Changes:
- Fixed the PREVENT "Copy all" button: it now actually autofills the PREVENT inputs from the calculators above (Age/Sex from eGFR, Total-C/HDL from lipids, BMI, eGFR, UACR) in one click
- Previously the button only copied a text summary to the clipboard, so the inputs never filled — relabeled to "Autofill from above"
- Added a small status line under the section header reporting how many fields were filled
- (from V9) ZIP→SDI lookup moved to external packed file zip-sdi.txt; index.html ~54 KB

After upload, test:
https://tipcode-cpu.github.io/cardioquick/?v=10

Files to deploy: index.html, manifest.json, service-worker.js, icon.svg, zip-sdi.txt
