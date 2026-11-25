### New

#### News
- Send to sheet in the Save dialog (next to Copy rows) puts texts straight into the localization spreadsheet, so nothing has to be pasted: news titles and texts go to the News tab, the other listed keys (offers, popups, categories, chain offers) to the Offers tab. New keys are added below the last row, changed texts are replaced, and texts that are already the same are left alone. The line under the buttons lists what was added and updated.
- Sheet setup... in the Save dialog connects the editor to the spreadsheet once per computer (web app URL, token and the names of the News and Offers tabs). The connection is kept in the editor settings of that computer, not in the project.
- A key with no English text typed is added with the key itself as its text (what the game shows for it now), and only when the tab does not have that key yet. News texts are sent on every Send to sheet, also the ones that are already in Localization_en.json.
