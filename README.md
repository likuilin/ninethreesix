# ninethreesix

I bought a [Twiddler 4](https://www.mytwiddler.com/) and tried out the default layout and then Backspice. Then, I decided to create my own layout.

### Motivation

My main motivation is twofold:

* I want Ctrl and Shift on finger keys. I don't like pushing the thumb keys or the zero-row keys at all - and when I use my computer, I mostly am either typing words or using Ctrl shortcuts. This decision costs a lot of chords, unfortunately.

* I don't see the need for two-character chords where the constituent keys are their own characters. For instance, I think hitting e and t in sequence is no worse than hitting e and t simultaneously to get et. And I think with sufficient practice, I can avoid accidentally chording et when I mean to type e t - so, the chord that would have become et can mean something completely different. This frees us a lot of chords, to pay for the first motivation.

This layout is called 936 (ninethreesix) because it maps the single characters to pages of size 9+6+6+6=27. The third finger is used to switch between the single-character pages, leaving the fourth finger row free to use as modifiers. 4R is Ctrl, 4M is Shift, and 4L is a pseudo-modifier that enables us to have a 3x3 grid for the numbers - otherwise, this would not be possible, since the rest of the pages (see the combinatorics below!) are all 2x3 or 1x3.

### Chart

In the chart below, each box is a page, and • represents a key held down to access the page. Also, for the first row of pages, SHIFT/CTRL are optional modifiers. This is not really a formal chart, it's more of an image of my mental map of where everything is.

```
.---------------.---------------.---------------.---------------.---------------.
|BCKSP SPC   s  |  a    h    s  |  g    b    j  |  p    d    z  |  x    y    m  |
|               |               |               |               |               |
|  n    t    r  |  n    t    r  |  l    k    q  |  v    c    u  | (1)   w    f  | Just (1): Ctrl-SPC
|               |               |               |               |               | SHFT-(1): DEL
|  i    e    o  |  i    e    o  |  •            |       •       |            •  | CTRL-(1): Ctrl-V
|               |               |               |               |               | RRLM: Shift-DEL
|  a    h   TAB |CTRL• SHFT•    | CTRL SHFT     | CTRL SHFT     | CTRL SHFT     |
'---------------'---------------'---------------'---------------'---------------'
.---------------.---------------.---------------.---------------.
|  1    4    7  | (2)  (3)  (4) | sHOM s↑  sEND | HOM   ↑   END | (2) PrintScreen/SysRq
|   0           |               |               |               | (3) Scroll Lock
|  2    5    8  | CapsL INS NumL|  s←  s↓   s→  |  ←    ↓    →  | (4) Pause/Break
|               |               |               |               |
|  3    6    9  |  •            |       •       |            •  |
|               |               |               |               | Note: The numbers are not numpad keys,
|            •  |            •  |(s=Shift)   •  |            •  |      they are standard keyboard nums
'---------------------------------------------------------------'
                .---------------.---------------.---------------.
                |  •            |       •       |            •  |
                |               |               |               |
                |  -   PDN  PUP | (5) ENTR  (6) |  :    ,    .  | (5) Alt-←
                |               |               |               | (6) Alt-→
                |               |               |               |
                |               |               |               |
                |               |               |               |
                |---------------+---------------+---------------|
                |  •            |       •       |            •  |
                |               |               |               |
                |  •            |  •            |  •            | (x) = not assigned
                |               |               |               |
                |  /    #   (7) |  *    @   (x) |  ju  (x)  (x) | (7) Ctrl-Alt-Del
                |   (8)  (9)    |               |               | (8) Ctrl-Z
                |  \    ~    0  |  +    ^    %  | (x)  (x)  (x) | (9) Ctrl-\
                |---------------+---------------+---------------|
                |  •            |       •       |            •  | (Think of $ and % as diagonal chords
                |               |               |               |  on the numpad rather than down here)
                |       •       |       •       |       •       |
                |               |               |               |
                |  !=   '    ?  |  =    ;    ly |  !    "    ?! |
                |   F1   F2   F3|   F4   F5   F6|   F7   F8   F9|
                |  ion  `    $  | (10) (11) (12)|  (    )   (13)| (10) Ctrl-Shift-T
                |---------------+---------------+---------------| (11) Shift-Enter
                |  •            |       •       |            •  | (12) Shift-Tab
                |               |               |               | (13) Alt-Shift-5
                |            •  |            •  |            •  |           (Google Docs strikethrough)
                |               |               |               |
                |  fg   cl   fl | (x)  iou   ou |  &    |   ESC |
                |               |               |   F10  F11  F12 devtools :)
                |  {    }   (x) |  [    ]   (15)|  <    >    _  | (15) Alt-Tab (no holding)
                '---------------'---------------'---------------'

Extra:
* MRMR: Ctrl-Shift-V

Thumbs:
* T0 is left click
* T1 is GUI/Win
* T2 is Ctrl, used to hit Ctrl-Shift keys and keys like Ctrl-+ and Ctrl-0
* T3 is RGUI which is intercepted by Autohotkey in my setup (all others are left keys)
* T4 is Alt

System: (here for convenience, all are default)
* T023 sleep                * T0F1M battery
* T0F4M cycle config        * T0F4L nav mode
* T0F4R cycle bluetooth     * T14F4R reset bluetooth
```

Tip: Since the only four-button chords are function keys and Ctrl-Z, all of which have the same button for fingers 3 and 4, while typing letters, a mis-chord can always be "cancelled" (without releasing all of the buttons in order to hit backspace) by pushing a different key on finger 4 than the one held down on finger 3 to select the page.

### Rationale and combinatorics

Rationale for the page layout:
* I started with Backspice's home page, except with CTRL/SHFT on top of BCKSP/SP at the top, but I quickly realized that I'd rather hold down a pinky key and tap with my first three fingers, than hold down my index finger and tap with my pinky. It doesn't technically matter since it's a chord, but the ordering matters for mental-model reasons. So, I moved CTRL and SHFT to the bottom, displacing a and h while they are held.

* Having the minor letter page selector be on the row with the vowels is important because minor characters usually alternate with vowels, and so it is much less mental load to "import" the vowels into each minor page, than it is to switch to the home page to find the vowel. So, unfortunately, it cannot be on the index finger. I tried it on my middle finger for a while, but having the page switch key being in the middle of the page felt too mentally awkward. So, that is why it is on the ring finger.

The placement of the single minor characters within those pages was determined initially using frequency tables in conjunction with common Ctrl shortcuts, but then I swapped them around as I learned and used the layout. These swaps are not well-documented, and are likely specific to my own hand size and shape (for instance, when I was only looking at this table, I thought 2M 3L was easier to hit than 1R 3L, but no, 1R 3L is far easier). If you are adopting this layout, I would strongly recommend swapping these around if a different layout makes more sense to you, or you keep consistently mis-keying a character a certain way. The only way to figure out what works best for you is to physically try typing on it.

After assigning the single-char pages on the first row, we then assign the 4L pages as if it was a modifier - so, what is available to us is the numpad and each six-char page with the modifier held down. The numpad is sideways because that makes more sense to me - on a physical numpad, the same finger accesses 1, 4, and 7, so that is reflected here. Zero is an exception to the pattern layout described below - it is propagated to the last section. On the six-char pages with a modifier held down, we map the DEL special keys and then the navigation keys. The shifted version of the navigation keys are for selection manipulation.

At this point, combinatorics-wise, a key simplifying insight is that, if X represents a non-omitted key, the set of chords we have assigned up to now is equal to the union of the patterns XOOO, OXOO, OOXO, OOOX (home page) and XOXO, OXXO (minor char pages) and XOOX, OXOX, OOXX, XOXX, OXXX (first and minor char pages with a modifier held down). Therefore, after set subtraction from the set of all such patterns, we just have four (omitting OOOO lol) patterns left for assignment. These four are, exhaustively, XXOO, XXOX, XXXO, XXXX. So, in other words, the rest of the mappings must include the first two fingers held down, and conversely, as long as the first two fingers are held down, all combinations are free to be mapped without collision. With all of those mapped, we will have all the chords visited exactly once. The last part of the chart represents this, with 9+18+18+18 chords left to assign in those smaller pages, plus 81 chords for XXXX.

More formal and concise summary of the combinatorics:

* The first table assigns:
  * 12 = all single-btns
  * 9\*2 = all two-btns where (4R or 4M)
  * 6\*3 = all two-btns where (not 3O (equivalently, 3R or 3M or 3L)) and 4O
  * 6\*3\*2 = all three-btns where (not 3O) and (4R or 4M)
  * For a total of 84 combinations.
* The second table assigns:
  * Note: Zero is an exception and counted in the third table
  * 9 = all two-btns where 4L
  * 6\*3 = all three-btns where (not 3O) and 4L
  * For a total of 27 combinations.
* The third table assigns:
  * 3\*3 = all two-btns where 3O and 4O
  * 3\*3\*6 = all three-btns where (not 1O) and (not 2O)
  * 3^4 = all four-btns
    * Note: Actually we only use a few of the four-btns - some, such as 1L 2R 3L 4R, are not representable as adjacent-button chords, and so this chart is insufficient to display them - which is okay since they are also too hard to hit.
  * For a total of 144 combinations

Which adds up to a grand total of 255, or, 4^4-1 (the one being OOOO).

### Development

I wish the [Twiddler Tuner](https://tuner.mytwiddler.com/) could export config files in a human-readable flat text layout. Since it only exports binary config files, and it does not have good version control features, it is hard to keep track of modifications.

In this git repo, I will try to change this readme as I make any changes to the actual configuration. In the future, after a good third-party reverse-engineered flat format becomes standard, a future me may reconstruct the history of this project in a more human-diffable way.
