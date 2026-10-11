# Soccer Analytics with StatsBomb Data

Exploring professional soccer event data in Python, using StatsBomb's free open data.
This is an ongoing project; part 1 focuses on **shots**.

## What's done so far (part 1)

- Loaded competitions, matches and full event data for a match with
  [`statsbombpy`](https://github.com/statsbomb/statsbombpy)
- Explored the event types in a match (passes, carries, shots, duels, pressures, ...)
- Filtered the events down to shots and picked out the useful details for each one:
  - **xG** (`shot_statsbomb_xg`): how likely the shot was to be a goal
  - outcome, shot type, body part, play pattern, and whether the shooter was under pressure
  - shot location, and the **freeze frame** (where every nearby player was at the moment of the shot)
- Built a clean shots table to analyse in the next part

## Next

<!-- TODO: say in your own words what you want to find out, e.g. "visualise every shot
on a pitch, coloured by xG" or "compare a team's xG with the goals they actually scored" -->

## How to run

```bash
pip install statsbombpy pandas numpy matplotlib
```

Then open `part 1.ipynb` in Jupyter or VS Code and run the cells top to bottom.
No account or API key is needed: the open data is free.

## Tools

Python · pandas · NumPy · Matplotlib · statsbombpy

## Data

Data provided by [StatsBomb](https://statsbomb.com) through their free
[Open Data](https://github.com/statsbomb/open-data) repository.
