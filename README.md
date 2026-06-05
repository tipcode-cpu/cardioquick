# CardioQuick PWA V13

Changes:
- Fixed dropdown (select) overflow in the PREVENT 5-column grid: "Statin use" / "BP treatment" etc. were spilling outside the card border on desktop
- Cause: selects had width:100% but no min-width:0, so their default content width pushed them past the grid cell. Added min-width:0 + box-sizing:border-box (and same on grid cells)
- (from V12) responsive layout for screens <= 640px (1-col cards, 2-col PREVENT grid)
- (from V11) individual per-field "copy" buttons restored
- (from V10) "Autofill from above" actually fills the PREVENT inputs
- (from V9) ZIP->SDI lookup in external packed file zip-sdi.txt

After upload, test (hard-refresh / clear site data if the old service worker is cached):
https://tipcode-cpu.github.io/cardioquick/?v=13

Files to deploy: index.html, manifest.json, service-worker.js, icon.svg, zip-sdi.txt
