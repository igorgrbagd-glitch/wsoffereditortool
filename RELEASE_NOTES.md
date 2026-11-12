### New

#### Chain Offers
- Right menu icon: a chain offer can show a character's animated idle pose as its icon in the game's right menu instead of the default art. Pick the character, frame the part of her to show on her whole body (drag the frame, or drag a corner to resize it to any shape while the opposite corner stays put; scrolling zooms the big framing view around the pointer, and it opens zoomed in on the frame; the frame fits inside the icon, centred) and see the icon next to it at its real size (128 x 128). She is drawn at full resolution, straight from her Spine prefab.
- Background: a graphic behind her at the icon's size (a sprite, or a plain Circle placeholder until the art exists), with a tint. Move it to line it up with her (offset fields, nudge arrows, or click the icon preview and use the arrow keys; Shift = 5) and scale it.
- Mask: she is kept inside a shape, by default the background's (like a badge), or the Circle, or any sprite with its own offset and scale. Openings (rectangles or ellipses) let her ears, hair or other pieces show outside of it: add as many as needed, then move and resize them (and an own mask) right on the preview with their handles (corners resize both ways, side handles one side). Ears and other pieces in openings can reach up to a quarter of the icon past its edges, in the game and in the preview.
- Without a frame of your own the game frames her head automatically (shown as a dashed square). Auto (frame the head) goes back to that.
- Glow: the background can glow around its shape like the other glowing right menu icons (the game's UI glow), with its color, size, spread, intensity and animations (Pulse, Heartbeat, Flicker, Color cycle, Orbit, Sweep). The preview shows the glow; its animation plays in the game.

**How to use**

1. In the sidebar, under Popups, click Chain Offers, and pick the chain offer at the top.
2. In the Right menu icon section, pick the girl in Character (None keeps the default icon art). The icon at its real size stays in view at the top right.
3. Frame tab: drag the frame over her body to choose what the icon covers, and drag a corner (or a side handle, for just that side) to change its size and shape; the opposite corner or side stays where it is. The faint square around it shows what the icon really covers. Scroll to zoom the view, or use Zoom to frame and Whole body; the result shows under the fields as you go.
4. Background tab: pick a Background (Circle as a placeholder, or Sprite... for the real art) and line it up on the 2x preview: click it and use the arrow keys, or the nudge buttons and Background scale.
5. Mask tab: keep Same as background, or pick Circle or Sprite... for another shape. Click Add rectangle or Add ellipse, then on the 2x preview drag the dashed opening over her ears and pull its handles until they show outside the mask; it may reach past the top of the icon for tall ears. A Circle or sprite mask gets a yellow box to move and resize the same way.
6. Glow tab (optional): tick Glow, then pick its Color, Size, Spread, Intensity and any Animation.
7. Click Save.

### Improved

#### Chain Offers
- The popup preview is drawn full width above the step list, so it is much bigger (side by side only on a very wide window).

#### Offers
- New offers (New offer, copies, rerun sets, paid chain steps, copied check-ins) now get the current Unix time in seconds as their steamId instead of the highest steamId + 1. Offers made in the same second still get unique ids (the next one up). Existing steamIds are not changed.
