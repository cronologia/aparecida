# aparecida — Nossa Senhora Aparecida, a chronology

An open, source-referenced chronology of **Nossa Senhora Aparecida** — the
terracotta image of Our Lady of the Conception reportedly netted from the
Paraíba do Sul river at Guaratinguetá (São Paulo, Brazil) in 1717, the
devotion and national shrine that grew around it, and the Church and state
acts that honoured it, from the first chapel (1745) to the tercentenary
(2017). Part of the [cronologia](https://github.com/cronologia) family.

Published site: <https://cronologia.github.io/aparecida/> (en / es / pt).

## Posture

**Honours are not findings.** There is no apparition in this case and no
discernment judgment anywhere in it: what was found in 1717 was a statue —
*Aparecida* names the image, not a vision — and every Church act in this
chronology (the 1904 canonical coronation, the 1908 and 1980 basilica titles,
the 1930 patronage decree, three golden roses, the 1931 and 1980
consecrations) honours or regulates a devotion. Each act is recorded as an
act about a named object — an image, a church, a nation's patronage — and
the dataset never adds them up into a verdict. This repo deliberately ships
**no `approvalLadder`**: there is no discernment case to ladder.

The dating is the dataset's spine of honesty:

- the **earliest surviving account is from August 1757** — forty years after
  the event — the "Notícia" of Pe. João de Morais e Aguiar in Guaratinguetá's
  Livro do Tombo, and it opens **"No ano de 1719, pouco mais ou menos"**
  ("in the year 1719, more or less");
- **1717 is a historians' inference** from the documented October 1717
  passage of the Count of Assumar through Guaratinguetá (Brustoloni, 1979);
- **no day is attested** in any source; 12 October is a twentieth-century
  liturgical and civil convention (Law 6.802/1980 for the holiday).

The finding is therefore recorded as a REPORTED event, the fishermen's names
carry their attestation caveat, and the 1743-vs-1757 attribution tangle in
the secondary literature is recorded, not resolved. Items resting on the
Santuário's own media operation (A12) alone are labeled official-devotional
and flagged; single-source dates are flagged (`dateVerified: false`, rendered
with a `?`), with a `dateNote` naming the disagreement where sources conflict.

## How it works

`data/chronology.json` is the source of truth. A zero-dependency Node script
compiles it into static HTML (`docs/`, served by GitHub Pages) in English
(authoritative), Spanish and Portuguese; the es/pt strings live in
`data/i18n/` as committed dictionaries.

```
node scripts/validate-data.js   # schema + citation check
node build.js                   # regenerate docs/
node --test                     # invariants, i18n completeness, renderers
```

Every data change must pass all three and commit the regenerated `docs/`
together with the data. See `AGENTS.md` and `context.md` before editing.

## License and corrections

Content compiled from public sources, each cited in the site's References
section. Corrections against primary sources are welcome — open an issue.
