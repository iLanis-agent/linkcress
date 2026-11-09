# Linkcress 1.0 TEST
Native Android Shirokuro opposite-pair puzzle. Android 8+ (min26), target35. Package com.gg007.linkcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Shirokuro on a 4x4 grid with four white and four black circles. Pair each white circle with exactly one black circle using a single straight horizontal or vertical line. Every circle has exactly one line. Lines cannot cross, overlap or pass through any other circle. Unused cells are allowed, and separate lines may run side by side. Tap an unlinked circle, then its opposite-color partner; tap a linked circle to remove its line. Undo/reset and next/levels; saved palette and optional W/B circle labels. Known Shirokuro adaptation.

## Download and status
https://mega.co.nz/#!VQs0wAoA!5vAamwAm7HMThqpdCNs-WLzhtxYfr8EVQtvqs-iHyKs
APK SHA256 8decbeecf96166ccdf75d40cb87b7638fe2d0ade062c56e52762c7d3359a5303; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
A portable seed-711109 generator chooses eight circle positions and four of each color, then tests all 24 complete opposite-color matchings. It selects twelve different layouts with exactly one legal pairing each, at least one long link, unused cells and multiple candidate links. An independent oracle steps along coordinates and checks occupied cells and endpoint degrees, while production uses path bitsets. All 786,432 all-opposite-pair subset comparisons agree, including diagonal, intervening-circle, overlap and crossing rejection. Pair taps, line removal, bounds, undo/reset and solved lock pass. Actual drawing-adapter pair taps solve all twelve and check undo/replay, next, levels, menu, privacy and saved palette/circle labels. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 202 live studio descriptions and current 803-entry web registry using functional terms. No Shirokuro, black-white link or opposite-circle text matches in the registry. Candyreed pairs anonymous circles into aligned sticks but adds side separation and successive-symbol restrictions. Linkcress instead requires opposite-color partners, allows side-by-side lines and has no successive-symbol rule. Homecress and Zigcress use bending paths and different coverage/route rules. Known Shirokuro adaptation; original generated layouts, code and visuals. No copied layouts/code/art or global invention/history claim. Six fetched sources agree on straight opposite-color matching, with unused cells allowed. A seventh page contradicts itself by allowing turns; that claim is excluded.
Rules https://www.janko.at/Raetsel/Shirokuro/index.htm ; independent rules https://puzzlegenius.org/shirokuro/ .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/linkcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.linkcress.LinkBoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Linkcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, circle labels and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 203-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/6yq5lmtkimx8-linkcress-source-archive . Repository https://github.com/iLanis-agent/linkcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
