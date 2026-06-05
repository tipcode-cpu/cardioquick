# CardioQuick PWA V9

Changes:
- Moved the large embedded ZIP→SDI decile lookup out of index.html into an external file (zip-sdi.txt)
- index.html shrunk from ~404 KB to ~54 KB (parses far faster on load)
- SDI table stored as a packed string (1 char per ZIP slot, base ZIP 1001); decode is O(1) index lookup
- Table is fetched lazily and warmed on idle; cached by the service worker for offline use
- Cache bumped to v9; zip-sdi.txt added to precached assets

After upload, test:
https://tipcode-cpu.github.io/cardioquick/?v=9

Files to deploy: index.html, manifest.json, service-worker.js, icon.svg, zip-sdi.txt
