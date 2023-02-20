# re4-packing-game

Rotate, re-arrange, and relax in this simple 2D packing game. Made using Unity.

❤️ Inspired by Resident Evil 4's inventory. [Here's a quick demo of it by coolkarmact](https://www.youtube.com/watch?v=t8xz5Lcyn94)

## Roadmap

Win Condition: Put back all items into the box.

Player Actions:

- Pick up and put down item
- Rotate selected item by 45 degrees increments

Item Constraints:

- All items have box like dimensions, 1x2, 2x4, 2x6 etc
- Must not overlap with any other item
- Items can be placed in play and staging area

Play Area and Staging Area:

- An X by Y sized grid
- Able to place and items

### MVP

- [ ] Setup 1x1 play area
- [ ] Setup basic item 1x1
  - [ ] Show sprite
  - [ ] Pick up item
  - [ ] Put down item in play area
  - [ ] Put down item in side area
- [ ] Define win logic: all items placed in play area

### V1: Complicate game a bit

- [ ] Expand board to 2x2
  - If I understand enough, try to make board size easily configurable!
- Add a second item, of size 1x2 so we can overlap
- [ ] Extend item
  - [ ] Add colider
  - [ ] Check for overlap
    - Don't allow place item if overlapping.
    - On attempt, keep item selected.
    - Indicate blocked action somehow

### V2: Polish

- [ ] SFX!
  - [ ] Selecting item
  - [ ] Putting down item
  - [ ] Rotate item
- Chill background music
- Snappy/responsive pick up/put down item feel

## Asset Credits

Inventory background - https://opengameart.org/content/golden-ui-bigger-than-ever-edition

## Learnings

- I forgot how to do Tilemaps and how to prep assets for it. [Here's the docs which were pretty clear and straight forward!](https://docs.unity3d.com/Manual/Tilemap-workflow.html)
  - Docs mentions something interesting: set the Pixels per Unit to match the sprite's width, so the sprite fits the grid exactly! Since my asset is `32x32`, I set it to `32`!
