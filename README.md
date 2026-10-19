# SANBOLA Secret Mission — updated setup

Files:
- `index.html`: game page with the supplied Apps Script URL already inserted.
- `Code.gs`: Apps Script backend configured for the spreadsheet ID supplied in this chat.

## Important setup
1. In the Apps Script project, replace all contents of `Code.gs` with the included `Code.gs`, then Save.
2. Deploy > Manage deployments > Edit (pencil) > select New version > Deploy. Keep Execute as `Me` and access `Anyone` if available.
3. Replace the existing `index.html` in the GitHub repository with this updated `index.html` and commit the change.
4. Test with your own details first. The first test will create a row in the sheet; remove that test row afterward if needed.

## Privacy and limitations
This is a lightweight prototype, not a fraud-proof contest platform. It prevents a second attempt for the same phone number in the sheet, but does not verify identity. The current browser-to-Apps-Script JSONP flow sends the name and phone in a request URL; URLs may be logged by browser/network services. For a public contest with prizes, prefer a POST-based backend and review privacy/security before launch. Keep the spreadsheet private and do not publish its link.
