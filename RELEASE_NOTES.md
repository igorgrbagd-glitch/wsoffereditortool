### New

#### Chain Offers
- Popups on the left, Repository/Offers/ChainOffer.json: a time-limited Chain Offer popup whose paid and free steps unlock in order, in any mix (paid, free, free, paid...). The preview matches the game: Chain Offer title, Expires in timer, close button, collection offer reward tiles, green price and glowing Free buttons, locks, sold out and the arrows between steps. The preview stays in view next to the step list while you edit (stacked on a narrow window). A step strip above it shows the whole chain at once (click a step to jump to it), and Player on 1, 2, 3... Done shows the chain as a player on any step sees it.
- Steps are compact cards (step, paid or free, price, reward chips with their icons); the selected step opens to edit its offer and rewards, and a click on a reward chip edits that reward on the right. Add free or paid steps, make a step paid or free, reorder and remove steps, and edit each step's rewards (plain reward pairs like Offer.json; tile backgrounds come from the reward, like collection offers). A paid step gets its own offer in Offer.json (<chain id>_Step_<n>, next steamId, ChainOfferPremium reward); click it to edit its price on the right.
- With nothing selected, the right panel shows a chain summary: Live, Upcoming or Ended (on the Live on date when set) with the time left, paid and free steps, the price of all paid steps, everything the chain gives (currencies summed), and problems such as missing Localization_en texts, missing step offers and steps without rewards (click one to select the step).
- Hover a step, reward or button to find its card in the step list (and the other way round), click a reward to edit it on the right, click a step or a paid button to select it, and drag the steps up and down (or use the mouse wheel) to scroll them like in the game. Text labels drag and resize like promotion labels.
- New from this... copies a chain offer with the next id and dates, and copies its paid step offers under the new id with new steamIds.

**How to use**

1. In the sidebar, under Popups, click Chain Offers.
2. Start a chain: click New chain offer when there is none, or pick an existing one at the top and click New from this... to copy it with the next id and dates.
3. Set its Id, Start date and End date. Background is optional (empty = the default chain_offers_bg art).
4. Build the steps in order with + Paid step and + Free step. Each paid step gets its own offer in Offer.json.
5. Click a step (its card, its row in the preview or its chip in the strip). Its card opens: use + Add reward to give it rewards, and click a reward chip to edit that reward on the right.
6. For a paid step, set its price on the right (Price, in Nutaku Gold).
7. Use the arrows on a card to reorder steps, Make paid / Make free to switch a step, and X to remove it. Player on 1, 2, 3... Done shows the chain as a player on that step sees it.
8. Click an empty part of the preview to see the Chain summary on the right: when it is live, the total price, everything it gives, and any problems to fix.
9. Click Save.

### Improved

#### Chain Offers
- Chain offer step offers are not orphans, follow a rename of their offer (including the ChainOfferPremium reward), and their labels go to the Save dialog's Localization_en rows.
- Save checks chain offers: step offers and their ChainOfferPremium reward, steps without rewards, one offer per step, reward formats and dates.

#### Popups
- Shortcuts: Esc deselects; on a chain offer, Delete removes the selected reward, step or text and Up / Down move the selected step; arrow keys nudge the selected text of a chain offer or shop promotion (Shift = 10).

#### Quest Simulator
- Tiers tab: switch the simulator between the game's power steps and a success curve on party power / quest rating (steepness, 50% point, highest and lowest chance, start chance), with a chart against the tier targets and Fit to tier targets.
- Tiers tab: difficulty tiers (Easy, Normal, Challenging, Elite, Hardcore) with editable rating bands, success targets and quest shares, a reference player built from your presets, and a tier report that grades every quest level and boss with both success models. The difficulty curve gets a tier strip.
- Generate ratings: proposes a rating and tier for every quest level from the reference player and a pacing pattern (per island, the brief's mix or its example), with boss and island rules, an option to keep each quest's levels rising, a before/after preview, and Apply to Quest.json (one undo step). It writes ratings and tiers only; the power steps the game uses today are left as they are.
- Rewards and failure: tier reward multipliers, partial rewards and shorter rest after a failure, and a pity bonus after failures in a row, with each tier's value per hour against its target and against the game's rules, a solver for the multipliers, and an option to use the rules in Run.
- In the game: shows what QuestSystem.json tells the game about quest success and rewards, and writes the simulator's rules there or loads them back (needs the matching game update).
- Save checks Quest.json ratings and tiers and the new QuestSystem.json settings.
- npm run test:unity also checks the success chance and the files the simulator writes against the game in the open Unity Editor.
