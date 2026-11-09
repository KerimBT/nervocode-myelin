# Privacy

NervoCode Myelin does not collect, store or transmit personal data or browsing data. Everything it does
happens inside your browser.

## What is kept, and where

**In the local storage of the browser (never sent anywhere):**
- Your settings: switches, excluded sites and elements you hid by hand (associated with the site name),
  custom rules, theme and language.
- A total number of blocked requests.
- "Privacy report": counts per day (blocked requests, banners removed, warnings shown) and the names of the
  third-party domains blocked most often. No page address and no visited site. It is erased with "Delete data"
  or "Reset" and is not part of the backup.
- "Detected trackers": for third-party domains that behave like trackers, the domain name and a one-way hash of
  the sites on which they appeared (only to count them). No list of visited sites, no page address. These data
  are not part of the backup and are erased with "Reset".
- Sites you marked as trusted for downloads, and sites where you allowed popups, in the settings.

**In the session memory of the browser (erased when the tab or the browser is closed):**
- Counters of blocked items, the names of contacted domains, and the address of the page open in each tab (it is
  needed to show which site was blocked on the warning page).
- The list of what a page did (fingerprinting, sensitive APIs, blocked clipboard commands).

## What is checked locally

- The lists of dangerous sites and the check for lookalike domains are bundled with the extension: no address is
  sent to be checked.
- The text a page tries to copy to the clipboard is examined in the browser to recognise dangerous commands. If
  it is blocked, it is shown to you and never sent anywhere.
- Popups: whether a window opened by a page follows a click of yours is decided in the browser. Only a count of
  stopped windows is kept; nothing about the page is recorded or sent.
- Encrypted backup: the password you choose is used only to encrypt the file in the browser. It is never stored
  or sent.
- Download guard (off by default): if you turn it on, the extension asks for the "Downloads" permission so it can
  warn you when a file that runs commands has been downloaded and let you delete it. It reads only the file
  name, type and originating site.

## The only external request

Quick filter fixes (on by default, can be turned off in the settings): every 6 hours the extension downloads two
public files from GitHub, `raw.githubusercontent.com/KerimBT/nervocode-myelin/main/filters/update.json` and
`update.json.sig`. The request contains only the address of those files, with no cookies and no browsing data. As
with any web request, GitHub receives your IP address. No code is downloaded: the files contain data only and are
accepted only with a valid signature.

## Reports

"Site not working?" → "Yes, report it" opens a pre-filled issue form on GitHub in a new tab, with the site name
(not the full address), the versions of the extension and of the browser, and the active protections. You read it,
you can edit it, and you decide whether to submit it. Nothing is sent automatically.

## Contact

Privacy questions: open an issue on the [public issue tracker](https://github.com/KerimBT/nervocode-myelin/issues).
