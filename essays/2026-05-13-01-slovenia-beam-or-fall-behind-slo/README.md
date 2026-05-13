# NotebookLM video paket: Slovenija — preklopi ali zaostani

Slovenski paket virov za NotebookLM, namenjen ustvarjanju **kinematografske video predstavitve v slovenskem jeziku** o priložnosti za UI-preobrazbo Slovenije.

## Datoteke

| Datoteka | Opis |
|---|---|
| `01-esej.md` | **Glavni vir.** Slovenski esej »Preklopi ali zaostani«. |
| `02-podatki-statistika.md` | Vsa ključna številčna dejstva (Eurostat, WEF, OECD, Slovenija, Estonija, Finska). |
| `03-panel-kontekst.md` | Kontekst AmCham panela — moderatorka, govorca, vprašanja, ciljna publika. |
| `04-kljucni-koncepti.md` | Šest ključnih konceptov, na katerih sloni naracija (obrestujoči se razkorak, tritedenski prepad, trenutek radosti, …). |
| `05-modela-estonija-finska.md` | Konkretni opisi estonskega AI Leap in finskega fenomenološkega učenja kot referenčna modela. |
| `notebooklm-prompt.md` | **Direktorski brief.** Custom prompt za NotebookLM Video Overview (kinematografski stil, slovenščina). |
| `youtube-description.md` | Pripravljen opis za nalaganje na YouTube. |

## Postopek

1. Pojdi na [NotebookLM](https://notebooklm.google.com/).
2. Ustvari nov zvezek (»notebook«), poimenuj ga **Slovenija — preklopi ali zaostani**.
3. V vire (»sources«) naloži: `01-esej.md`, `02-podatki-statistika.md`, `03-panel-kontekst.md`, `04-kljucni-koncepti.md`, `05-modela-estonija-finska.md`. *(`01-esej.md` je sidrišče — NotebookLM mu daj največji pomen.)*
4. Generiraj **Video Overview** (deep dive video). V polje »Customize« vstavi vsebino datoteke `notebooklm-prompt.md`.
5. Po generaciji preveri narečje/izgovorjavo lastnih imen (Ajša, Godnov, Horvat, Murska Sobota, Pomurje, Velenje, Anthropic, AmCham). Po potrebi regeneriraj z dopolnjenim promptom.
6. Naloži na YouTube z opisom iz `youtube-description.md`. Časovne oznake (timestamps) dopolni po dejanskem rezu.

## Ciljni stil

- **Jezik:** slovenščina (knjižni jezik, brez slenga, brez tujk, kjer ima slovenščina ustaljen izraz).
- **Stil:** kinematografski — dokumentaren v slogu prestižnih kratkih filmov, ne ležeren podcast.
- **Dolžina:** 7–9 minut.
- **Tempo:** trije akti — diagnoza, manjkajoča izkušnja, načrt. Vsak akt z lastnim ritmom in dramaturško krivuljo.

## Ciljna publika

Slovenski poslovni voditelji, ravnatelji in pedagoški delavci, državni sekretarji in svetovalci ministrov, podjetniki MSP-jev, člani gospodarskih zbornic in skupnosti AmCham Slovenija — torej ljudje, ki so o UI že nekaj slišali, niso pa še sami preklopili.
