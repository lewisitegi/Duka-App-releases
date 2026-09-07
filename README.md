# Duka-App-releases
Public APK releases for Duka Manager

## Downloads
| Version | File | Date |
|---------|------|------|
| v1.3.4 (build 9) | [DukaManager-v1.3.4.apk](./DukaManager-v1.3.4.apk) | 2026-09-07 |

## v1.3.4 Highlights
- Fixed: saving a product could freeze the screen and tapping Save repeatedly added the SAME product several times — now one save, the button can't double-fire, and any failure shows a clear message instead of a stuck spinner
- New: barcodes are scanned TWICE when adding a product — the second scan must match the first (and the barcode must leave the frame in between), so a misread never becomes your product's barcode
- Cart/POS: the camera now stays minimized while you add products from the list — it no longer pops back up after every item, and it pauses while minimized to save battery

## v1.3.3 Highlights
- Start fresh is now far more reliable: the cloud delete retries automatically (up to 3 attempts, 30s each) so a cold server or a weak connection no longer stops it — installs over v1.3.2 fix the "Could not reach the server" error that could appear even while online
- When a delete still fails, the app shows the real reason (e.g. session expired, server error) instead of always blaming the internet connection
- Failed deletes are recorded in the activity log so issues can be traced

## v1.3.2 Highlights
- Start fresh is now available any time from Settings → Import / Restore (previously only right after a reinstall) — permanently delete the cloud copy, all local backups and, if you choose, the shop data currently on this phone
- Pending uploads are cleared before a start-fresh wipe, so queued data can't re-create the cloud copy afterwards
- Cloud wipe is now thorough: rows saved by older app versions without a shop id can no longer resurface after wiping
- New admin action: Revoke License — stops a paid license immediately (~30s while the phone is online) and keeps the remaining paid time so Resume can restore it

## v1.3.1 Highlights
- Backups you control: after a reinstall the app shows exactly what your backup contains (products, stock, sales, customers, debts, logs, notes) and lets you pick what to import — nothing is added automatically anymore
- Start fresh option permanently deletes the previous cloud copy and all local backup files
- Deleted products are now removed from every new backup
- Backups now also include activity logs and notes
- Live totals (KSh) shown for sales and debts before you import

## v1.3.0 Highlights
- Loss-warning guardrail when saving products priced below cost (loss per item + total loss, Edit Price / Save Anyway)
- Cart delete confirmation in POS (undo still available)
- Instant enforcement of admin shop actions (Revoke Trial, Extend Trial, Activate License, Extend License, Resume, Delete Shop) while the phone is online (~30s worst case)
- Resume now restores the previous plan (free trial or paid) with its remaining days

Install: download the APK on the phone and open it (allow installing from unknown sources when prompted).
If you installed the broken build 4, just install this one over it — no need to uninstall.

