# Thistle
<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/final3.png" width="75%">

```
  p g c d v  ' r u o j
q l s t h y  x n e a i ?
  b f w m k  z @ , . *
          \  ␣ /

\ = Left Magic | / = Right Magic
@ = Repeat     | * = Pinky Magic
```
Thistle is a high inroll layout that uses repeat, magic, two R keys and two N keys to achieve low SFBs, scissors, and outrolls.

You can try it [here](https://keyboard-layout-try-out.pages.dev/?l0r0=q+w+e+r+t++y+u+i+o+p&l0r1=a+s+d+f+g++h+j+k+l+%3B+%27&l0r2=z+x+c+v+b++n+m+%2C+.+%2F&l1r0=j+o+u+r+%27++v+d+c+g+p&l1r1=i+a+e+n+x++y+h+t+s+l+q&l1r2=r+.+%2C+%3B+z++k+m+w+f+b&z=z). Select your layout (or input your own), then scroll down and click "convert words", then "type words".

## Table of Contents
- [Glossary](glossary.md)
- [Stats](#stats)
- [Design](#design)
  - [Left Half](#left-half)
  - [Right Half](#right-half)
  - [Magic](#magic)
    - [Magic Rules](#rules) 
- [Tools Used](#tools-used)
---
<details>
  <summary><h2>Stats</h2></summary>
Without repeat or magic

[Layout Playground](https://oxey.dev/playground/index.html "Layout Playground"):

<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/stats 2.jpg" width="70%">

[Cyanophage](https://cyanophage.github.io/playground.html?layout=jour%27vdcgp-iaenxyhtslq%24.%2C%3Bzkmwfb%5C%5E%2F&mode=ergo&lan=english&thumb=l "View on Cyanophage"):

<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/stats.jpg" width="80%">

[KeySolve](https://luminespire.github.io/keysolve-web/ "Keysolve"):

<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/keysolve.jpg" width="100%">

</details>

---

## Design
### *<ins>Left Half*
The home keys are arranged for inrolls, with `L` specifically taking a spot to minimize scissors. `VYK` makes up the inner index column to keep lateral stretches low, while `Q` on this side avoids the long one-handed rolls that would come from placing it on the other. It also causes less SFSs.

The top and bottom rows were set up around the idea that `P`, `G`, `C`, `B`, `F`, and `W` each have a couple consonants that they commonly pair with, and that magic keys on the index can turn those bigrams into inrolls.

For example, `CD` outputs `CR`. In the word "crane", four of its five letters are typed with just one hand. If magic is used, that can be lowered to three, thus shortening the roll, keeping your left hand on home row, and improving comfort.

|   Input   | Magic | Output |
|   :---:   | :---: | :---:  |
|  P G C    |   D   |   R    |
| P G C B F |   M   |   L    |
|   W       |   M   |   H    |
|  B F      |   H   |   R    |

### *<ins>Right Half*
The `EU, AO, I` vowel block is used for its low redirects and pinky use. `N` and `R` serve to maximize rolling, while `J` and a second `R` key boost inrolls. `'XZ` fill the inner index column to keep lateral stretches low, with punctuation and repeat taking the remaining spots.

`Repeat` is basically just another magic key, as it does more than simply repeat the previous letter. Here are the general rules:

At the start of a word:

| Input | Output |
| :---: |  :---: |
|   I   |   '    |
|   A   |   R    |
|   E   |   A    |
|   Я   |   I    |
|   ₡   |   Y    |

`₡` = any consonant

In the middle of a word: `repeat`

At the end of a word:

| Input | Output |
| :---: | :---:  |
|   E   |   R    |
|   H   |   T    |
|   K   |   Y    |
|. ? !  |   "    |

It acts as backspace in all other situations.

Conflicts have also been accounted for so words like "tea" and "after" can both be typed with "e@" at the end.

<details>
 <summary><h3>Thistle went through a number of revisions which you can see here:</h3></summary>
The changes are highlighted on the right

```
  j o u r ~  k d l f b
? i a e n ~  w h t c s q
  ' . , x z  y m p g v
```
```
  j o u r z  k d l b f       ~ ~ ~ ~ z  ~ ~ ~ b f
? i a e n x  w h t c s q   ~ ~ ~ ~ ~ x  ~ ~ ~ ~ ~ ~
  ' . , @ ~  y m p g v       ~ ~ ~ @ ~  ~ ~ ~ ~ ~
```
```
j o u r '  v w l d b     ~ ~ ~ ~ '  v w ~ d b
i a e n x  y h t c s q   ~ ~ ~ ~ x  y ~ ~ ~ ~ ~
? . , @ z  k m p f g     ? ~ ~ ~ z  k ~ ~ f g
```
```
j o u r '  k w c f b     ~ ~ ~ ~ ~  k ~ c f ~
i a e n x  y h t l s q   ~ ~ ~ ~ ~  ~ ~ ~ l ~ ~ 
? . , @ z  v m d p g     ~ ~ ~ ~ ~  v ~ d p ~
```
```
j o u r '  v d c p w     ~ ~ ~ ~ ~  v d ~ p w
i a e n x  y h t l s q   ~ ~ ~ ~ ~  ~ ~ ~ ~ ~ ~ 
? . , @ z  k m g f b     ~ ~ ~ ~ ~  k ~ g f b
```
```
  j o u r '  v d c p b       ~ ~ ~ ~ ~  ~ ~ ~ ~ b
? i a e n x  y h t l s q   ? ~ ~ ~ ~ ~  ~ ~ ~ ~ ~ ~ 
  , . ~ @ z  k m w f g       , . ~ ~ ~  ~ ~ w ~ g
```
```
  , o u @ '  v d c p g       , ~ ~ @ ~  ~ ~ ~ ~ g
? i a e n x  y h t s l q   ~ ~ ~ ~ ~ ~  ~ ~ ~ s l ~ 
  j . ~ r z  k m w f b       j ~ ~ r ~  ~ ~ ~ ~ b
```
```
  j o u r '  v d c g p       j ~ ~ r ~  ~ ~ ~ g p
? i a e n x  y h t s l q   ~ ~ ~ ~ ~ ~  ~ ~ ~ ~ ~ ~ 
  Я . , @ z  k m w f b       Я ~ , @ ~  ~ ~ ~ ~ ~
```
```
  p g c d v  ' r u o j
q l s t h y  x n e a i ?
  b f w m k  z @ , . Я
```
</details>

## Magic

The outputs are strictly 1:1 to retain the feel of normal typing and ensure that you won't get banned on typing websites. They're also context dependent and can be chained together for greater usability. E.g. `A\` → `AO` while `WA\` → `WAY`. "earthquake" would be typed as `e@\th/u\he`.

In general, the thumbs will output the key above or below the previous key to avoid SFBs. E.g. `E\` → `EU`. `U\` → `UE`. Depending on the word though, it'll fix outrolls, redirects or SFSs.

The alphas do more of the same but also help to increase same row rolls and decrease movement. E.g. "cranky" would be typed as `cdandn` and "programming" would be `pdogdanhing`. There are tons of word-specific rules but they've been left out since it would be impractical to list them all.

<details>
  <summary><h2>Rules</h2></summary>
  
```
-------------------------------------------------------------------------------------------------------
| jn → ji     | o\ → oa | u\ → ue | r\ → rn   | vj → vl | dn → dy | c@ → cy   | gd → gr   | p@ → py   |
| thj → thr   | o' → o. | u' → u, | r\ → rx   | vn/→ vy | d@ → dy | cv → cq   | gh → gf   | pd → pr   |
|             | oh → or | uh → ur |           | v@ → vy | d/ → dm | cd → cr   | gm → gl   | pm → pl   |
|             |         |         |           |         | d/ → dk | cd → ct   | gc → gs   | p/ pb     |
|             |         |         |           |         | dc → dh | cm → cl   | gcd → gst |           |
|             |         |         |           |         | dc → dw | cm → ck   |           |           |
|             |         |         |           |         |         | c/ → cw   |           |           |
|-----------------------------------------------------------------------------------------------------|
| i@ → i'     | a\ → ae | e\ → er | neЯ → nee | y/ → yh | h@ → hy | tЯ → tw   | sЯ → sw   |           |
| i\ → ij     | a\ → ao | e\ → eu | n\ → nr   | y/ → ym | h/ → hv | tm → tr   | s@ → sy   | lh → lp   |
| i\ → i?     | a\ → ay | ex → eo | n\ → nz   |         | h/ → hd | tm → tc   | s@\ → syn | ly → lb   |
| ih → ir     | a' → a. | e' → e, | nh → nx   |         | h/ → hh | tmn → tch | s@h → syr |           |
|             | ae → ai | e@ → ea | nh → nz   |         | h/ → hm | t/ → tc   | sv → sq   |           |
|             | a@ → ar | eh → er | nl → n'   |         |         |           | sy → sg   | qh → qu   |
|             | ah → ar |         |           |         |         |           | sd → sp   | qi@ → qui |
|             |         |         |           |         |         |           | s/ → sf   |           |
|-----------------------------------------------------------------------------------------------------|
| Я@ → ri     |     ₡, → ₡e       |           | kn → ky | mn → my | wm → wh   | fh → fr   | bh → br   |
| Яex → reo   |     ₡,@ → ₡ee     |           | k@ → ky | m@ → my | wm → wt   | fm → fl   | bm → bl   |
| Яe\ → ree   |     ₡,\ → ₡ei     |           |         | m/ → mv | w/ → wc   | fw → ft   | b/ bp     |
| Я,@ → rei   |     ₡y → ₡@       |           |         | m/ → mh |           | f/ → fg   |           |
| Я,@\ → rein |     ₡k → ₡@       |           |         | mk → mm |           |           |           |
| Я,\ → reu   | ₡ = any consonant |           |         |         |           |           |           |
-------------------------------------------------------------------------------------------------------
```
</details>

---

## Tools Used
- The [Keyboard Layouts Google Doc](https://docs.google.com/document/d/1W0jhfqJI2ueJ2FNseR4YAFpNfsUM-_FlREHbpNGmC2o "Keyboard Layouts Google Doc") for design knowledge
- The [Layout Playground](https://oxey.dev/playground/index.html "Layout Playground") analyzer for drag and drop letter swaps and their resulting stats
- [Cyanophage's](https://cyanophage.github.io "Cyanophage Analyzer") analyzer for more stats
- Merriam-Webster's [Word Finder](https://www.merriam-webster.com/wordfinder "Merriam-Webster Word Finder") to filter by specific letters to check for conflicts in the magic rules
