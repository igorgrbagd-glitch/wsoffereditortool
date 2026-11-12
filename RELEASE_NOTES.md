### New

#### News
- New News section in the sidebar for the game's News window (StreamingAssets/News/News.json), so news no longer has to be written by hand. The list shows every item in the game's order with its banner, English title, dates and whether it is live, upcoming or ended.
- Add a news item with + New news (you type a short name and the editor makes its `<name>_title` and `<name>_text` keys), copy one with New from this... (same image, link and rewards, dates moved on), drag items to reorder them, or remove one.
- The right panel edits everything the game reads: title and text keys with their English texts, typed in boxes that show the text styled like the game does (bold is bold, red is red, centred lines are centred) instead of tags, with Bold, Italic, Centre, Color and Plain buttons; the tags are written for you, the banner picked from thumbnails of the images in StreamingAssets/News, dates or Timer mode (no start date: a countdown instead of dates), the Details link and the rewards.
- The preview draws the news window like the game: banner with the date or timer pill, title, text, reward tiles with Claim, and the Details button. Drag the window up and down to see a long text, like the Season Pass levels (anywhere, also on the text). The title and the text can be typed right on the preview: click one to edit it, then select part of it for a small menu with bold, italic, position (left, centre, right) and color; press Esc or click outside it to go back to dragging.
- Save checks news too: a missing or repeated title key, dates the game cannot read, a start after the end, a banner that is not in StreamingAssets (or is spelled with different upper/lower case), reward values, plus warnings for keys without an English text and a link that is not a web address.
- Typed English texts can be undone with Undo (Ctrl+Z) like any other edit, and Reload throws away the news texts that were typed but not saved.
- The English texts typed for news are added to StreamingAssets/Localization/Localization_en.json when you save (new keys at the end, changed keys in place), so the game shows them without copying anything by hand. That file is generated from the localization sheet: add the texts to the sheet too before it is generated again, and for the other languages.

**How to use**

1. In the sidebar, click News. The list on the left of the main area is the game's news list, top item first.
2. Click + New news, type a short name (for example winter_event) and click Create. For a follow-up of an existing item, select it and click New from this... instead.
3. Type the English title and the English text, either in the boxes on the right or by clicking the title or the text on the preview. Select part of the text to style it: on the preview a small menu appears over the selection with bold, italic, position and color (Plain removes the styling); the boxes on the right have the same buttons.
4. In Image, click a banner thumbnail. For a new banner, put the image file in StreamingAssets/News first, then click Refresh.
5. In When it shows, set the start and end dates, or switch to Timer (no start) for an item that shows right away with a countdown.
6. Optional: paste a web address in Details button, and add rewards for a Claim button.
7. Drag the item in the list to where it should appear in the game, check the Problems section at the bottom of the right panel, then click Save. The English texts are added to Localization_en.json by the save.
