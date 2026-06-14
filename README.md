<h1 align="center">Thistle</h1>

<p align="center">
<img src="https://github.com/Brooklyn-Style/Thistle/blob/main/images/heatmap.png" width="75%">
</p>
<h3>
  
```
                                          p g c d v  ' ^ u o j
                                        q l s t h y  x n e a i ?
                                          b f w m k  z # , . *
                                                  \  ␣ /

                                          \ ^ # * / = Magic Keys
```
</h3>

Thistle is a high inroll layout that uses magic to achieve extremely low SFBs, SFSs, scissors, and outrolls. It was made by hand with magic and alt-fingering in mind and as such, uses columns that normally wouldn't be viable. Thumb keys are recommended but not strictly necessary.

Note: "Magic" is used as a catch-all term for context-dependent outputs.

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

### <ins>*Left Half*
- The `LSTH` home keys setup promotes inrolls. 
  - `L` on the pinky minimizes scissors, as it pairs with every letter.
  - `H` on the index makes for a good magic key due to its location and low amount of conflicts.
- `P`, `G`, `C`, `B`, `F`, and `W` on non-index fingers ensure that their common bigrams are inrolls, either by default or with magic. E.g., `CD` outputs `CL`.
- `V`, `Y`, and `K` on the inner index column keep lateral stretches low.
- `D` on the top index allows for easy alt-fingering of `M`, `V`, `Y`, or `K` before or after it.
- `M` on the bottom index makes for a good second magic key for the same reasons as `H`.
- `Q` on this side avoids the long one-handed rolls that would come from placing it on the other. It outputs `QU` instead of just `Q` since it's almost always followed by `U`.

### <ins>*Combos*
- `L` + `\ Magic` = `N`
- `S` + `\ Magic` = `J`
- `T` + `\ Magic` = `Z`
- `G` + `C` = `QU`

### <ins>*Right Half*
- The `EU, AO, I` vowel block is used for its low redirects and pinky use.
- `N` and `# Magic` maximize rolling.
- `J` and `* Magic` boost inrolls.
- `'`, `X`, and `Z` on the inner index column keep lateral stretches low.
- Punctuation takes the remaining spots.
- `Space` on this side *feels* better for hand balance even though it results in a 40-60 split.

## Magic
- The outputs are almost always 1:1 to retain the feel of normal typing. The only exception is when dealing with `Q`; `QU` will be typed instead for simplicity. Macros
- The outputs are context dependent. E.g., `te#` → `tea`, while `afte#` → `after`
- Multiple magic keys can be chained together for greater usability. E.g., "earthquake" would be typed as `e#lth\ahe`.
- Most of the consonants have magic functions to increase same row rolls and decrease movement. E.g., "function" would be typed as `funwmio\` and "probably" would be `p\o^/h\j`. 
- There are tons of word-specific rules in the AutoHotkey script so only the general ones are listed below.

### <ins>*Rules*

- `\ Magic` outputs `R` by default and generally helps to avoid SFBs, SFSs, and awkward patterns.
- `^ Magic` acts as a one-shot `shift` key by default, sends `M` after `A`, `E`, and `I`, and otherwise reduces SFBs and movement.
- `# Magic` outputs `backspace` by default, `R` after vowels, `repeat` after consonants, and `S` at the end of words for plurals.
- `* Magic` outputs `N` by default and `E` after consonants.
- `/ Magic` is used as a last resort to deal with SFBs, SFSs, and outrolls, as it creates SFSs with `space`.  

```
┌───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┬───────────┐
│  pg → ps  │  gc → gs  │  cd → cl  │  dv → dk  │           │           │           │           │           │           │
│  pc → pt  │  gd → gl  │  cd → ct  │  dy → dw  │           │           │           │           │           │           │
│  pd → pl  │  gm → gf  │  cv → cqu │  dk → dy  │           │           │           │  uh → ur  │  oh → or  │           │
│  pm → pb  │  gy → gn  │  cm → cw  │           │           │           │           │  u\ → uh  │  o\ → oh  │           │
│  py → pn  │  g\ → gm  │  cm → ck  │    d\     │           │           │           │  u' → um  │  o' → om  │  jn → ji  │
│  p\ → pm  │           │           │     ↓     │           │           │           │  ux → ua  │  ox → oi  │  ₡j → ₡y  │
│           │           │           │ [d] hmvyk │           │           │           │  u^ → ue  │  o# → or  │           │
│ p_h → p_l │ g_h → g_s │ c_h → c_t │           │           │           │           │  u# → ur  │ _oe → _oa │           │
│ p_m → p_b │ g_m → g_f │ c_m → c_w │           │           │           │           │           │           │           │
│ p_\ → p_m │ g_\ → g_m │ c_\ → c_m │           │           │           │           │           │           │           │
├───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┤
│  lh → lp  │  sl → squ │  tm → tw  │           │           │           │           │  eb → ex  │           │           │
│  lm → lb  │  sd → sp  │  t\ → tc  │           │           │           │           │  eh → er  │  ah → ar  │           │
│  l\ → lm  │  sh → sg  │  tn → tc  │  ¶h → ¶"  │           │           │           │  e\ → eh  │  a\ → ah  │  ih → ir  │
│  l\ → lq  │  sm → sf  │           │           │           │           │  nh → nx  │ _ez → _ei │  ax → ao  │  i\ → ih  │
│           │  sy → sn  │           │    h\     │  ₡y → ₡@  │  ₡x → ₡y  │  nm → nz  │  ez → er  │  a^ → am  │  ix → i'  │
│           │  s\ → sl  │           │     ↓     │           │           │  ₡n → ₡y  │  e^ → em  │  a# → ar  │  ix → ij  │
│           │           │           │ [h] dmvy  │           │           │           │  e^ → eu  │  a# → ao  │  i^ → im  │
│ l_h → l_p │ s_h → s_g │ t_h → t_c │           │           │           │           │  e# → ea  │  ae → ai  │  i# → ir  │
│ l_m → l_b │ s_m → s_f │ t_m → t_w │           │           │           │           │  e# → er  │ _a, → _ao │           │
│ l_\ → l_m │ s_\ → s_m │ t_\ → t_m │           │           │           │           │  e/ → eu  │           │           │
├───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┼───────────┤───────────│
│  bh → bb  │  fw → ft  │  wh → wt  │           │           │           │           │           │           │           │
│  bm → bl  │  fh → ff  │  wh → wk  │           │           │           │  #m → #n  │           │           │           │
│  by → bp  │  fm → fl  │  wm → wc  │           │           │  uz → u,  │  #\ → #n  │           │           │           │
│  b\ → bm  │  fy → fg  │  wm → wh  │           │           │  ez → e,  │  ₡# → ₡@  │           │           │           │
│  bn → by  │  f# → fs  │           │    m\     │  kj → kn  │  oz → o.  │  ₡# → ₡s  │ _*u → _nu │ _*. → _no │  _* → _n  │
│           │           │           │     ↓     │           │  az → a.  │ ₡,# → ₡ui │  ₡, → ₡u  │ ₡*. → ₡eo │  ₡* → ₡e  │
│           │           │           │  [m] hvy  │           │  jz → j?  │₡.e# → ₡oar│₡*., → ₡eou│  ₡. → ₡o  │           │
│ b_h → b_l │ f_h → f_s │ w_h → w_t │           │           │  iz → i?  │₡.,# → ₡oin│ ₡*, → ₡ei │ ₡.e → ₡oa │           │
│ b_m → b_p │ f_m → f_g │ w_m → w_c │           │           │           │ _*# → _ni │ ₡., → ₡oi │           │           │
│ b_\ → b_m │ f_\ → f_m │ w_\ → w_m │           │           │           │           │           │           │           │
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

### *<ins>Tools Used*
- The [Keyboard Layouts Google Doc](https://docs.google.com/document/d/1W0jhfqJI2ueJ2FNseR4YAFpNfsUM-_FlREHbpNGmC2o "Keyboard Layouts Google Doc") for design knowledge
- The [Layout Playground](https://oxey.dev/playground/index.html "Layout Playground") analyzer for drag and drop letter swaps and their resulting stats
- [Cyanophage's](https://cyanophage.github.io "Cyanophage Analyzer") analyzer for more stats
- Merriam-Webster's [Word Finder](https://www.merriam-webster.com/wordfinder "Merriam-Webster Word Finder") to filter by specific letters to check for conflicts in the magic rules
