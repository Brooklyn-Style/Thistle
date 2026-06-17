<h1 align="center">Thistle</h1>

<p align="center">
<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/heatmap.png" width="60%">
</p>

```
  p g c d v  z ' u o j
q l s t h y  ^ n e a i ?
  b f w m k  x # , . *
          \  ␣ /

\ ^ # * / = Magic Keys
```

Thistle is a high inroll layout that uses magic to achieve extremely low SFBs, SFSs, scissors, and outrolls. It was made by hand with magic and alt-fingering in mind and as such, uses columns that normally wouldn't be viable. Thumb keys are recommended but not strictly necessary.

Note: "Magic" is used as a catch-all term for any context-dependent output.

You can try it [here](https://keyboard-layout-try-out.pages.dev/?l0r0=q+w+e+r+t++y+u+i+o+p&l0r1=a+s+d+f+g++h+j+k+l+%3B+%27&l0r2=z+x+c+v+b++n+m+%2C+.+%2F&l1r0=p+g+c+d+v++%27+%5E+u+o+j&l1r1=l+s+t+h+y++x+n+e+a+i+%3F&l1r2=b+f+w+m+k++z+r+%2C+.&z=z) (without magic). Select your layout (or input your own), then scroll down and click "convert words", then "type words".

## Table of Contents
- [Glossary](glossary.md)
- [Stats](#stats)
- [Design](#design)
  - [Left Half](#left-half)
    - [Combos](#combos)
  - [Right Half](#right-half)
  - [Magic](#magic)
    - [Rules](#rules) 
- [Tools Used](#tools-used)

---

<details>
  <summary><h2>Stats</h2></summary>
Without repeat or magic

[Layout Playground](https://oxey.dev/playground "Layout Playground"):

<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/stats 2.jpg" width="70%">

[Cyanophage](https://cyanophage.github.io/playground.html?layout=pgcdv%27ruoj-lsthyxneai%2Fbfwmkz%3B%2C.%3D%5C*q&mode=ergo&lan=english&thumb=l "View on Cyanophage"):

<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/stats.jpg" width="80%">

[KeySolve](https://va1orance.github.io/keysolve-web/ "Keysolve"):

<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/keysolve.jpg" width="100%">

</details>

---

## Design

### *<ins>Left Half*
- The `LSTH` home keys setup promotes inrolls. 
  - `L` on the pinky minimizes scissors, as it pairs with every letter.
  - `H` on the index makes for a good magic key due to its location and low amount of conflicts.
- `P`, `G`, `C`, `B`, `F`, and `W` on non-index fingers ensure that their common bigrams are inrolls, either by default or with magic. E.g., `CD` outputs `CL`.
- `V`, `Y`, and `K` on the inner index column keep lateral stretches low.
- `D` on the top index allows for easy alt-fingering of `M`, `V`, `Y`, or `K` before or after it.
- `M` on the bottom index makes for a good second magic key for the same reasons as `H`.
- `Q` on this side avoids the long one-handed rolls that would come from placing it on the other. It outputs `QU` instead of just `Q` since it's almost always followed by `U`.
- `\ Magic` outputs `R` by default and is used to avoid SFBs, SFSs, and redirects.

#### Combos
- `L` + `\ Magic` = `N`
- `S` + `\ Magic` = `J`
- `T` + `\ Magic` = `Z`
- `G` + `C` = `QU`

### *<ins>Right Half*
- The `EU, AO, I` vowel block is used for the `OU` inroll and low pinky use.
- `'` on the top index makes `OU'` a 3roll and keeps this position's usage relatively low.
- `N` and `# Magic` maximize rolling.
  - `# Magic` outputs `backspace` by default, `R` after vowels, `repeat` after consonants, and `S` at the end of words for plurals. Placing it on the bottom row avoids scissors.
- `J` and `* Magic` on the pinky boost inrolls.
  - `* Magic` outputs `N` by default and `E` after consonants.
- `^ Magic` outputs a one-shot `shift` by default, `M` after vowels, `Y` at the end of words, and reduces movement otherwise.
- `X` and `Z` on the inner index column keep lateral stretches low.
- `,` and `.` maintain their QWERTY locations, with `?` being moved to the outer pinky column to make room for `* Magic`.
- `Space` on this side *feels* better for hand balance even though it results in a 40-60 split.
- `/ Magic` outputs `escape` by default and is used as a last resort to deal with SFBs, SFSs, and outrolls, as it creates SFSs with `space`. 

### *<ins>Magic*
- The outputs are almost always 1:1 to retain the feel of normal typing. The only exception is when dealing with `Q`; `QU` will be typed instead for simplicity.
- The outputs are context dependent. E.g., `te#` → `tea`, while `afte#` → `after`
- Multiple magic keys can be chained together for greater usability. E.g., "earthquake" would be typed as `e#lth\ahe`.
- Most of the consonants have magic functions to increase same row rolls and decrease movement. E.g., "function" would be typed as `funwmio\` and "probably" would be `p\o^/h\j`. 
- There are tons of word-specific rules in the AutoHotkey script so only the general ones are listed below.

<details>
  <summary><h2>Rules</h2></summary> 

- `\ Magic` outputs `R` by default.
- `^ Magic` outputs `shift` by default and `M` after vowels.
- `# Magic` outputs `backspace` by default, `R` after vowels, `repeat` after consonants, and `S` at the end of words.
- `* Magic` outputs `N` by default and `E` after consonants.
- `/ Magic` outputs `escape` by default.

```
┌───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┐
│  pg → ps  │  gc → gs  │  cg → cqu │  dv → dk  │           │           │           │           │           │           │
│  pc → pt  │  gd → gl  │  cd → ct  │  dy → dw  │           │           │           │           │           │           │
│  pd → pl  │  gm → gf  │  cd → cl  │  dk → dy  │           │           │  uz → u,  │  uh → ur  │  oh → or  │           │
│  pm → pb  │  gy → gn  │  cm → cw  │           │           │           │  ez → e,  │  u\ → uh  │  o\ → oh  │  \j → rh  │
│  py → pn  │  g\ → gm  │  cm → ck  │    d\     │           │           │  oz → o.  │  u' → um  │  o' → om  │  jn → ji  │
│  p\ → pm  │  g# → gs  │  cv → cqu │     ↓     │           │           │  az → a.  │  ux → ua  │  ox → oi  │  ₡j → ₡y  │
│           │           │           │ [d] hmvyk │           │           │  jz → j?  │  u^ → ue  │  o# → or  │           │
│ p_h → p_l │ g_h → g_s │ c_h → c_t │           │           │           │  iz → i?  │  u# → ur  │ _oe → _oa │           │
│ p_m → p_b │ g_m → g_f │ c_m → c_w │           │           │           │           │           │           │           │
│ p_y → p_m │ g_y → g_m │ c_y → c_m │           │           │           │           │           │           │           │
│ p_\ → p_y │ g_\ → g_y │ c_\ → c_y │           │           │           │           │           │           │           │
├───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┤
│  lh → lp  │  sl → squ │  th → tw  │           │           │           │           │  eb → ex  │           │           │
│  lm → lb  │  sd → sp  │ _tm → _tw │           │           │           │           │  eh → er  │  ah → ar  │           │
│  l\ → lm  │  sh → sg  │  tm → tt  │  ¶h → ¶"  │           │           │           │  e\ → eh  │  a\ → ah  │  ih → ir  │
│  l\ → lq  │  sm → sf  │  t\ → tc  │           │           │           │  nh → nx  │  e^ → em  │  a^ → am  │  i\ → ih  │
│           │  sy → sn  │  tn → tc  │    h\     │  ₡y → ₡@  │  ₡^ → ₡y  │  nm → nz  │  ex → er  │  ax → ao  │  i^ → im  │
│           │  s\ → sl  │           │     ↓     │           │           │  ₡n → ₡y  │ _ez → _ei │  a# → ar  │  ix → i'  │
│           │           │           │ [h] dmvy  │           │           │           │  ez → eu  │  a# → ao  │  ix → ij  │
│ l_h → l_p │ s_h → s_g │ t_h → t_c │           │           │           │           │  e# → ea  │  ae → ai  │  i# → ir  │
│ l_m → l_b │ s_m → s_f │ t_m → t_w │           │           │           │           │  e# → er  │ _a, → _ao │           │
│ l_y → l_m │ s_y → s_m │ t_y → t_m │           │           │           │           │  e/ → eu  │           │           │
│ l_y → l_y │ s_\ → s_y │ t_\ → t_y │           │           │           │           │           │           │           │
├───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┤───────────│
│  bh → bb  │  fw → ft  │  wh → wt  │           │           │           │           │           │           │           │
│  bm → bl  │  fh → ff  │  wh → wk  │           │           │           │  #m → #n  │           │           │           │
│  by → bp  │  fm → fl  │  wm → wc  │           │           │           │  #\ → #n  │           │           │           │
│  b\ → bm  │  fy → fg  │  wm → wh  │           │           │           │  ₡# → ₡@  │ _*u → _nu │ _*. → _no │           │
│  bn → by  │  f# → fs  │           │    m\     │  kj → kn  │           │  ₡# → ₡s  │  ₡, → ₡u  │ ₡*. → ₡eo │  _* → _n  │
│           │           │           │     ↓     │           │           │ ₡,# → ₡ui │₡*., → ₡eou│  ₡. → ₡o  │  ₡* → ₡e  │
│           │           │           │  [m] hvy  │           │           │₡.e# → ₡oar│ ₡*, → ₡ei │ ₡.e → ₡oa │           │
│ b_h → b_p │ f_h → f_g │ w_h → w_c │           │           │           │₡.,# → ₡oin│ ₡., → ₡oi │           │           │
│ b_m → b_l │ f_m → f_s │ w_m → w_t │           │           │           │ _*# → _ni │           │           │           │
│ b_y → b_m │ f_y → f_m │ w_y → w_m │           │           │           │ ₡*# → ₡ex │           │           │           │
│ b_y → b_y │ f_\ → f_y │ w_\ → w_y │           │           │           │           │           │           │           │
└───────────┴───────────┴───────────┴───────────┴───────────┴───────────┴───────────┴───────────┴───────────┴───────────┘
                                     p g c d v  ' ^ u o j     @ = Repeat
                                   q l s t h y  x n e a i ?   ₡ = Any Consonant
                                     b f w m k  z # , . *     ¶ = Any Punctuation Mark
                                             \  ␣ /           
```
</details>

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
  ' . , # ~  y m p g v       ~ ~ ~ # ~  ~ ~ ~ ~ ~
```
```
j o u r '  v w l d b     ~ ~ ~ ~ '  v w ~ d b
i a e n x  y h t c s q   ~ ~ ~ ~ x  y ~ ~ ~ ~ ~
? . , # z  k m p f g     ? ~ ~ ~ z  k ~ ~ f g
```
```
j o u r '  k w c f b     ~ ~ ~ ~ ~  k ~ c f ~
i a e n x  y h t l s q   ~ ~ ~ ~ ~  ~ ~ ~ l ~ ~ 
? . , # z  v m d p g     ~ ~ ~ ~ ~  v ~ d p ~
```
```
j o u r '  v d c p w     ~ ~ ~ ~ ~  v d ~ p w
i a e n x  y h t l s q   ~ ~ ~ ~ ~  ~ ~ ~ ~ ~ ~ 
? . , # z  k m g f b     ~ ~ ~ ~ ~  k ~ g f b
```
```
  j o u r '  v d c p b       ~ ~ ~ ~ ~  ~ ~ ~ ~ b
? i a e n x  y h t l s q   ? ~ ~ ~ ~ ~  ~ ~ ~ ~ ~ ~ 
  , . ~ # z  k m w f g       , . ~ ~ ~  ~ ~ w ~ g
```
```
  , o u # '  v d c p g       , ~ ~ # ~  ~ ~ ~ ~ g
? i a e n x  y h t s l q   ~ ~ ~ ~ ~ ~  ~ ~ ~ s l ~ 
  j . ~ r z  k m w f b       j ~ ~ r ~  ~ ~ ~ ~ b
```
```
  j o u r '  v d c g p       j ~ ~ r ~  ~ ~ ~ g p
? i a e n x  y h t s l q   ~ ~ ~ ~ ~ ~  ~ ~ ~ ~ ~ ~ 
  * . , # z  k m w f b       * ~ , # ~  ~ ~ ~ ~ ~
```
```
  p g c d v  ' r u o j
q l s t h y  x n e a i ?          [mirrored]
  b f w m k  z # , . * 
```

```
  p g c d v  ' ^ u o j       ~ ~ ~ ~ ~  ~ ^ ~ ~ ~
q l s t h y  x n e a i ?   ~ ~ ~ ~ ~ ~  ~ ~ ~ ~ ~ ~
  b f w m k  z # , . *       ~ ~ ~ ~ ~  ~ # ~ ~ ~
```
</details>

---

## Tools Used
- The [Keyboard Layouts Google Doc](https://docs.google.com/document/d/1W0jhfqJI2ueJ2FNseR4YAFpNfsUM-_FlREHbpNGmC2o "Keyboard Layouts Google Doc") for design knowledge
- The [Layout Playground](https://oxey.dev/playground/index.html "Layout Playground") analyzer for drag and drop letter swaps and their resulting stats
- [Cyanophage's](https://cyanophage.github.io "Cyanophage Analyzer") analyzer for more stats
- Merriam-Webster's [Word Finder](https://www.merriam-webster.com/wordfinder "Merriam-Webster Word Finder") to filter by specific letters to check for conflicts in the magic rules
