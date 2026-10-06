# Tímaverkefni – Kaffi Kóði ☕

**Tími:** um 35 mínútur, klárað í tímanum
**Vinna:** ein/einn eða tvö saman
**Skil:** `style.css` – [skilastaður og frestur, t.d. Canvas/Moodle fyrir lok tíma]

Kaffihúsið _Kaffi Kóði_ er komið með HTML fyrir nýju vefsíðuna sína en hún er alveg óstíluð.
Þitt verkefni er að skrifa **style.css** svo síðan verði snyrtileg og læsileg.

> ⚠️ Þú mátt **ekki** breyta `index.html`. Allt er gert með selectors í CSS.

---

## Kröfur

### A. Selectors

| #   | Krafa                                                                              | Selector-gerð |
| --- | ---------------------------------------------------------------------------------- | ------------- |
| 1   | `body` fær leturgerð, textalit og bakgrunnslit                                     | element       |
| 2   | `h1`, `h2` og `h3` fá sömu leturgerð **í einni reglu**                             | hópun         |
| 3   | `.verd` er feitletrað og í áherslulit · `.merki` er lítill „miði“ með bakgrunnslit | class         |
| 4   | `#opnunartimi` fær sérstakan bakgrunnslit                                          | id            |
| 5   | Tenglarnir í `nav` eru án undirstrikunar (notaðu **afkomenda-selector**, `nav a`)  | afkomendur    |
| 6   | Málsgreinin sem kemur **beint á eftir** hverri `h2` er skáletruð (`h2 + p`)        | systkini      |
| 7   | Tenglar skipta um lit þegar músin fer yfir þá (`:hover`)                           | pseudo-class  |
| 8   | Annar hver dagur í opnunartímanum fær bakgrunn (`:nth-child`)                      | pseudo-class  |
| 9   | Aðeins email-reiturinn fær ramma (`input[type="email"]`)                           | attribute     |
| 10  | Skrifaðu **specificity** (t.d. `0-1-1`) í athugasemd við þrjár af reglunum þínum   | specificity   |

### B. Box-model

| #   | Krafa                                                                                            |
| --- | ------------------------------------------------------------------------------------------------ |
| 11  | `* { box-sizing: border-box; }` efst í skránni                                                   |
| 12  | `main` er að hámarki 900px breitt og **í miðjunni** (`max-width` + `margin: 0 auto`)             |
| 13  | Hver `.rettur` er „kort“: bakgrunnur, `border`, `padding` og `margin` á milli korta              |
| 14  | `.vinsaelt` kortin fá **þykkari** eða öðruvísi litaðan ramma en hin                              |
| 15  | `nav li` liðirnir eru hlið við hlið (`display: inline-block`) með `padding` eða `margin` á milli |
| 16  | `header` og `footer` fá `padding` svo textinn klessist ekki upp við brúnina                      |

---

## Bónus (fyrir þau sem klára snemma)

- Settu kortin í `.flokkur` **þrjú hlið við hlið** með `display: inline-block` og reiknaðu út breiddina svo þau passi (skrifaðu útreikninginn í athugasemd).
- `.rettur:hover` fær `box-shadow`.
- `border-radius` á kortum, takka og miða.
- Notaðu `:first-child` eða `:last-child` einhvers staðar á skynsamlegan hátt.
- Búðu til þitt eigið litaþema – en haltu góðum læsileika (dökkur texti á ljósum grunni eða öfugt).

---

## Gátlisti áður en þú skilar

- [ ] Ég breytti ekki `index.html`
- [ ] Ég nota element-, class-, id-, afkomenda-, systkina-, pseudo- og attribute-selectors
- [ ] Ég skrifaði specificity við þrjár reglur
- [ ] `main` er í miðjunni og kortin eru með padding, border og margin
- [ ] Ég skoðaði eitt kort í DevTools og veit hvað það er breitt í raun
- [ ] Nafnið mitt er efst í `style.css`

## Ráð

- Vistaðu og reloadaðu oft (Cmd/Ctrl + R).
- Ef eitthvað virkar ekki: opnaðu DevTools → **Elements** → **Styles**. Yfirstrikuð regla = önnur regla vann (specificity eða röð!).
- Gleymdirðu `;` eða `}`? Það er algengasta villan.
