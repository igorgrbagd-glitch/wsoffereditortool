### New

#### Shop tabs
- Offers that have ended are taken out of the shop categories (CollectionOffers.json) when the editor opens or you press Reload. A category whose offers have all ended is removed with them.
- The offers themselves stay in Offer.json and move to the Orphan offers list. Nothing is written until you save, and the status bar lists what was removed.
- Kept as they are: offers with dates the game cannot read (they still show as errors), categories that were already empty, and the Time Limited list.

### Fixed

#### Tapping events
- New rerun set: the copied packs now give Tapping event intimacy for the event the set is made for (TappingEvent_26|500 becomes TappingEvent_27|500 on a set for TappingEvent_27) instead of still pointing at the event they were copied from. The amounts stay the same.
- New rerun set now copies the newest packs by default, also when you start it from the newest event itself, instead of the event before it.
- The intimacy reward follows the number of the new offer ids: Lust_Pack_I_Rerun_27 gives intimacy for TappingEvent_27, also when the set is made on TappingEvent_26.
- The new packs go into the pack list of the event with that number when it is in TappingEvent.json: a TappingEvent_27 that still names the _Rerun_26 packs (copied from TappingEvent_26) is updated to the new ids, and a list that already contains them is left untouched.
- An event that already lists its own packs (TappingEvent_26 with the _Rerun_26 packs) is never changed. If the event for the new packs is not in TappingEvent.json yet, the packs are only added to Offer.json and the page shows them under "Packs waiting for TappingEvent_27" until that event is added to the file.
- An event that names packs which are not in Offer.json yet is no longer offered as the set to copy; the newest packs that exist are used.
