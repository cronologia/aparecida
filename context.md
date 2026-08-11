# Context — cronologia/aparecida

## What this repo is

A source-referenced chronology of **Nossa Senhora Aparecida**: the small
terracotta image of Our Lady of the Conception reportedly netted from the
Paraíba do Sul at Guaratinguetá (SP) in 1717, the devotion that grew around
it, and the acts — ecclesiastical and civil — that honoured it. One of the
Cronologia family of projects; it follows the shared sourcing discipline in
`.claude/skills/sourcing-rules/SKILL.md`.

**The methodological identity of this repo**: there is no apparition and no
discernment judgment anywhere in the case. What was found was a statue, and
every Church act in the chronology — coronation, basilica titles, patronage,
golden roses, consecrations — honours or regulates a devotion ("honours are
not findings", core ADR-0007). That is why this repo has **no
`approvalLadder`**: the canonical rungs (local inquiry → bishop's judgment →
Rome) do not exist here, because nothing was ever alleged that would require
them. The DDF's 2024 *Norms* govern *alleged supernatural phenomena*; the
finding of a man-made image is not one (`ddf-norms-2024`).

## Domain background an agent needs

- **The attestation gap is the central fact.** The earliest surviving
  continuous account is the "Notícia da Aparição da Imagem da Senhora",
  written **August 1757** by the vicar Pe. João de Morais e Aguiar in the
  Primeiro Livro do Tombo of Guaratinguetá (cited variously at f. 77v and
  ff. 98–99) — **~40 years after the event**. It opens "No ano de 1719,
  pouco mais ou menos". **1717 is an inference** fixed by Pe. Júlio
  Brustoloni CSsR (1979) from the Count of Assumar's documented itinerary
  (his commission: Conselho Ultramarino consulta, 22 December 1716). **No
  day is attested**: A12 says "second fortnight of October", Souza (citing
  Pasin) says 17 October, and 12 October is a 20th-century convention
  (holiday by Law 6.802/1980).
- **The 1743/1757 attribution tangle.** Gazeta do Povo labels essentially
  the 1757 text "1743, by Pe. José Alves Vilela"; popular summaries speak of
  two early records (curia archive of Aparecida; Jesuit archive in Rome);
  the Diocese of Piracicaba invokes a ~1725 report. Recorded: 1757 as the
  earliest verified attestation, 1743 (Vilela) as reported-but-unpinned.
  **Open task: check Brustoloni 1979 directly** — he is everyone's ultimate
  source.
- **The honour ladder, correctly labeled.** Canonical coronation 8 Sept 1904
  (grant per A12: Chapter of St Peter's, 21 Dec 1903 — single-source);
  Basílica Menor for the old church 29 Apr 1908, first in Brazil; **principal
  Patroness of Brazil, Pius XI decree, 16 July 1930** — the decree text is
  **offline in the Aparecida curia archive** ("papéis avulsos", per Pasin
  apud Souza); it should be in AAS 22 (1930) — library task open; three
  golden roses (Paul VI 1967, Benedict XVI 12 May 2007 in person, Francis
  2017 delivered 9 Oct by Cardinal Re); JPII consecrates the new basilica
  4 July 1980. All are acts about objects; none adjudicates 1717.
- **The see**: the Archdiocese of Aparecida was erected **19 April 1958 by
  Pius XII (*Sacrorum antistitum*) directly as an archdiocese** — 1964 is
  the first resident archbishop's appointment (Cardinal Vasconcelos Motta),
  not an elevation. Do not repeat the "1958 diocese → 1964 archdiocese"
  error.
- **1978**: image seized and shattered 16 May 1978 (~200 fragments);
  restored at MASP by Maria Helena Chartuni, 28 June – 31 July 1978, under
  Pietro Maria Bardi; the return date (mid-Aug vs 19 Aug) is unpinned, and
  characterizations of the perpetrator are attributed, never asserted.
- **CELAM's "Aparecida Document"** (Fifth General Conference, at the shrine
  13–31 May 2007) is a conference document *drafted at* the shrine, not an
  act *about* the image — a constant conflation this repo disambiguates.
- **Size claims are attributed, dated claims**: "largest Marian shrine in
  the world" (the Santuário's self-description), "second-largest church
  after St Peter's" (Wikipédia-pt) — contested metrics, never in site voice.

## Known source-access quirks (net-access ladder)

- **Biblioteca Nacional (bndigital / BN articles)**: bot-wall — 403 even
  with a browser UA from this egress. **Inconclusive, not dead**; do not
  record its pages as unreachable, and do not cite them unverified.
- **vaticannews.va**: 403 from this egress. vatican.va itself serves fine —
  cite the acts from vatican.va, not from Vatican News summaries.
- **A12.com, cnbb.org.br, agenciabrasil.ebc.com.br, gazetadopovo.com.br,
  saopauloinfoco.com.br, catholic-hierarchy.org, pt.wikipedia.org**: served
  full content to this session (2026-08-11).
- **lopes-anpuh-2016** is served over plain **http** (encontro2016.sp.anpuh.org).
- **diocesedepiracicaba.org.br** uses a legacy ASP path (`capa.asp?p=461`).

## Standing uncertainties (kept honest in the dataset)

- No day attested for the finding; year inferred (see above). The 1717 event
  is `dateVerified: false` with the full dating honesty in its `dateNote`.
- 1743 vs 1757 earliest-text attribution (see above).
- 1904 document trail: Chapter-of-St-Peter's grant, 1901 petition details,
  who presided vs who crowned, and President Rodrigues Alves's presence all
  rest on devotional accounts — A12-only items labeled official-devotional.
- **1983 vs 1984** National Shrine declaration (shrine's page vs most
  secondaries); no primary CNBB act located online.
- Golden rose no. 1 logistics (15 Aug 1967 delivery, legate) are A12-only.
  2013 is **not** a golden rose year for Aparecida.
- 1978 return date (mid-Aug vs 19 Aug); perpetrator characterizations vary.
- 1930 decree text offline (curia archive); AAS 22 (1930) check open.
- 1834 church start, 8 Dec 1888 inauguration, 1868 visit, 2016 cathedral
  month: single-source (Wikipédia-pt or devotional), flagged.

## Current state (2026-08-11, initial authoring)

- 10 facts, 32 events, 10 figures, 6 organizations, 5 disambiguation items,
  24 references (the research's 22 verified URLs + `a12-padroeira`, used in
  the research's event table, + `ddf-norms-2024` for the disambiguation).
- No `approvalLadder` (deliberate — see above); no `threads` taxonomy yet
  (declaring lanes is per-repo editorial work with its own ticket).
- i18n caches (`data/i18n/es.json`, `pt.json`) still hold the template's
  seed-example strings — the es/pt dictionaries for this dataset are **not
  yet authored**, so `test/i18n-completeness.test.js` fails by design until
  they are.
