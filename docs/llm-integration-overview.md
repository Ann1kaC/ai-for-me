# LLM integratsiooni ülevaade: ChatGPT, Claude, Gemini + GitHub

Eesmärk: luua ühtne süsteem, kus kolm LLM-i (ChatGPT, Claude, Gemini) töötavad koos ühe keskse GitHub repo (`Ann1kaC/ai-for-me`) ümber, et toetada programmi **AI for Workflows** loomist ja arendamist.

## Rollid

### ChatGPT
- Põhifookus: arhitektuur, süsteemidisain, strateegia.
- Kasutus:
  - GitHubi struktuuri kavandamine (docs, systems, promptlibrary, gpt-powerteam, automations).
  - Süsteemipromptide, blueprintide ja SOP-de loomine.
  - LLM-ide rollijaotuse ja töövoogude defineerimine.
- ChatGPT projekt: **“AI for Workflows OS – GitHub & LLM Hub”** (soovituslik nimi).

### Claude
- Põhifookus: pikad, süvitsi minevad tekstid ja blueprintid.
- Kasutus:
  - detailsete AI employee blueprintide kirjutamine (v2, v3 jne),
  - põhjalike metoodika- ja programmiülevaadete loomine,
  - keerukamate süsteemi- ja kontseptsioonitekstide arendamine.
- Claude projekt: **“AI for Workflows – Blueprint Lab (GitHub-linked)”**.

### Gemini
- Põhifookus: Google Workspace ja automatsioonid.
- Kasutus:
  - töö Google Drive’i, Docs’i, Sheets’i ja Calendariga,
  - automatsioonide ja integratsioonide kavandamine (nt n8n, Zapier, Google Apps Script),
  - vajadusel dokumentide algversioonide loomine, mis hiljem tuuakse GitHubi Markdown-kujul.
- Gemini projekt: **“AI for Workflows – Workspace & Automations Hub”**.

## GitHubi roll

GitHub on “Single Source of Truth”:

- hoiab kõiki ametlikke blueprint’e, SOP-sid, struktureid ja dokumente;
- on ühine allikas kõigile LLM-idele;
- kõik olulisemad versioonid salvestatakse siia Markdown-failidena;
- versioonihaldus võimaldab näha, kuidas süsteem ajas areneb.

Kaustad:
- `docs/` – üldine dokumentatsioon ja ülevaated;
- `systems/` – AI süsteemid ja AI employee blueprintid;
- `promptlibrary/` – promptikogud ja struktuurid;
- `gpt-powerteam/` – GPT töötajate kirjeldused ja konfiguratsioon;
- `automations/` – automatsioonide ja integratsioonide skeemid.

## Tüüpiline töövoog

1. **Idee / vajadus** tekib (nt uus AI employee, uus moodul, uus automatsioon).
2. Vestlus algab **ChatGPT projekti** sees (AI for Workflows OS – GitHub & LLM Hub).
3. Vajadusel:
   - detailsemad blueprintid kirjutatakse **Claude’is**;
   - Google’i ökosüsteemiga seotud automatsioonid ja töövood kavandatakse **Geminis**.
4. Kui tekstid/blueprintid on valmis:
   - need tuuakse tagasi ChatGPT vestlusesse või otse Markdown-kujul,
   - salvestatakse GitHubi vastavasse kausta.
5. GitHubi versioon on edaspidi **ametlik** – kõik LLM-id kasutavad seda kui lähtedokumentatsiooni.

## Põhireeglid

1. **Üks tõepunkt:**  
   Ametlik dokumentatsioon elab GitHubis. Drive’i, Notioni või muude keskkondade versioonid on mustandid, kuni need pole GitHubi viidud.

2. **Üks projekt ChatGPT-s ühe süsteemi kohta:**  
   AI for Workflows OS saab ühe keskse projekti. Uute brändide või klientide jaoks luuakse eraldi projektid, mitte iga GitHubi repo jaoks.

3. **Rolle ei dubleerita:**  
   - ChatGPT = süsteemi/strateegia arhitekt.  
   - Claude = süvitsi minev tekst ja blueprint.  
   - Gemini = Workspace ja automatsioonid.  

4. **Kõik olulised muutused logitakse commit’idega:**  
   Igal suuremal muudatusel GitHubis lisatakse selge commit message, et arenduslugu jääks jälgitavaks.

