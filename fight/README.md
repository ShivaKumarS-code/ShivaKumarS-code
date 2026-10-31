# the fight

The top of the profile README looks like plain text. It isn't. `fight-light.svg` and
`fight-dark.svg` are 31-second animated SVGs (pure SMIL, no JavaScript) that GitHub renders
as-is. `make_fight.py` generates both; edit `PARAS` near the top to change the copy, then:

```
pip install pillow
python make_fight.py
```

Every word is its own `<text>` with a fixed `textLength`, so the fight can kick, slice and
stand on individual words while the layout stays identical on every OS.

The fight picks these words out by name (punctuation included):
`code,` is kicked apart, `make.` is the hole the bug climbs out of, and
`what`, `tech.` and `ideas,` are sliced in half.
