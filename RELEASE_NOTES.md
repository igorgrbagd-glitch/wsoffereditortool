### New
- Quest Simulator (Quests on the left): pick a quest, its level, a normal run or the boss fight and a boost, fill a party of up to 5 heroes, and see party power against the thresholds, success chance, rewards, run time, and each hero's injury, gear break, experience and rest. Set each hero's level, skills, power boost and gear on the right. A Monte Carlo run and a "Clearing level" estimate show how long a quest level takes. Uses Customers.json as it is in the editor, unsaved changes included.
- Quest Simulator, Tune: edit the selected quest level (power steps, boss steps, rewards, experience, wins to boss, quest time) and the success chance per step, with Undo and the normal Save to Quest.json and QuestSystem.json. A table shows the party's results on disk next to the edited ones.
- Quest Simulator, Balance grid: the hero level your party needs for every quest level, normal and boss, per power step. Spikes and cells that differ from the files on disk are marked; click a cell to open it.
- Quest Simulator, Economy: components and gold per hour (quest time plus rest), components lost to full storage, crystals to rush the quest or heal the party, and repair costs per run. Set the player's storage and class building levels; heroes above their building's cap are marked, and the Heroes table shows the runs to each hero's next level.
- Quest Simulator, Find a party: the strongest party, or the weakest that still reaches a power step, from every customer at a chosen level, skills and gear quality (filter by rank and class).
- Quest Simulator, Presets: save the quest, party, storage and buildings under a name (e.g. "Day 7 free player"), load them back, and copy or paste them to share with the team.
- Quest Simulator: a chart of how many components the simulated runs gave.
- Quest Simulator, Difficulty curve (top of the Balance grid): every quest level in unlock order with the band of hero levels between its first and last power step (the flow channel), boss markers, and your presets plotted where their players stand, coloured by zone (cannot start, flow, 100% every run). Click a point to open it.

### Improved
- The Quest Simulator's numbers are checked against the game itself: npm run test:unity computes random parties with the real game code in the open Unity Editor and compares hero power, party power and gear break chances (2000 parties match exactly).
