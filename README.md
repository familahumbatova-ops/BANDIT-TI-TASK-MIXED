# Object Learning Task (web version)

Browser version of `TI_bandit_task.py`. Same design: 3 blocks (linear positive, linear negative, random) in a random order for each participant, 5 rounds per block. In each round: pick 3 of 7 objects to see their rewards, then judge which of two objects is bigger (21 pairs), then recall the left-to-right order of the objects.

## Folder structure

```
my-repo/
  index.html
  images/
    block1/  stim1.jpg ... stim7.jpg
    block2/  stim1.jpg ... stim7.jpg
    block3/  stim1.jpg ... stim7.jpg
```

- Names must be `stim1` to `stim7` in every block folder (`.jpg`, `.png` or `.jpeg`).
- Missing images are replaced by coloured placeholder shapes, so the task also works without images.

## How to play

1. Open the link on a computer.
2. Type a participant ID (letters or numbers, e.g. `anna`) and press **Start**.
3. Follow the on-screen instructions. Continue with the **SPACE** key or the button.
   - **Choose:** click 3 of the 7 objects to see their reward.
   - **Which one is bigger?:** click the object you think is bigger, based on the rewards you saw.
   - **Order recall:** click the objects from left to right in the order they appeared on the choosing screen.
4. Play in one go (about 20-30 minutes) and do not close the tab.
5. At the end click **Download all 4 files** and send the files to the experimenter. If you must stop early, use **Quit & save data** (top right).

## Data

Four CSV files per session: `_bandit.csv`, `_ti.csv`, `_recall.csv` and `_hierarchy.csv`. Nothing is sent to a server: the data stay in the browser until the participant downloads them.
