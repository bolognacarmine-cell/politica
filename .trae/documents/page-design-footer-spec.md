# Page Design — Footer (miglioramento)

## Obiettivo
Riprogettare **solo il footer** per ottenere: meno elementi, più gerarchia e più spazio bianco, con sezioni chiare. Il **layout generale della pagina resta invariato** e l’identità grafica va mantenuta.

## Layout
- **Sistema**: CSS Grid per la struttura del footer (colonne/sezioni) + Flexbox per allineamenti interni (righe di link, baseline, spacing).
- **Desktop-first**:
  - Container footer allineato alla stessa larghezza del contenuto principale (stesso max-width già in uso).
  - 3–5 colonne/sezioni in desktop (in base ai contenuti effettivamente “essenziali”).
- **Responsive**:
  - Tablet: riduzione a 2 colonne.
  - Mobile: 1 colonna, sezioni in stack verticale; spaziature aumentate per tap target.

## Meta Information
- Nessuna modifica SEO richiesta: il footer è un componente condiviso.

## Global Styles (token e coerenza brand)
- **Colori / tipografia**: riusare i token esistenti (colori, font, pesi) per mantenere identità grafica.
- **Gerarchia tipografica consigliata (senza cambiare font family)**:
  - Titolo sezione: peso maggiore (es. 600–700), dimensione leggermente superiore ai link.
  - Link: dimensione standard del sito, con line-height aumentato per leggibilità.
- **Stati interazione**:
  - Hover: underline o cambio colore coerente con brand.
  - Focus: outline visibile (accessibile) e coerente con tema.

## Page Structure (struttura del footer)
Footer composto da due aree logiche (senza alterare il layout generale della pagina):
1. **Footer principale**: griglia di sezioni tematiche.
2. **Barra inferiore**: elementi secondari (es. note/diritti o link di servizio già presenti), visualmente più “quieti”.

## Sections & Components

### 1) Footer principale (sezioni)
- **Obiettivo**: rendere immediata la scansione.
- **Componenti**:
  - Titolo di sezione (testo breve, chiaro).
  - Lista di link essenziali (verticale) con spaziatura tra righe.
- **Regole contenuto**:
  - Ridurre la quantità: mantenere solo link davvero necessari; spostare i secondari nella barra inferiore o rimuovere duplicati.
  - Evitare liste troppo lunghe: preferire raggruppamento per tema.

### 2) Spazio bianco e ritmo
- **Padding esterno**: aumentare aria sopra/sotto il footer (es. 40–64px desktop, in base al sistema spaziature esistente).
- **Gutter tra colonne**: generoso (es. 24–40px).
- **Spacing tra titolo e lista**: evidente (es. 12–16px).
- **Spacing tra link**: sufficiente a evitare densità (es. 8–12px), con area cliccabile minima consigliata ~40px in altezza su mobile.

### 3) Barra inferiore (contenuti secondari)
- **Obiettivo**: separare chiaramente ciò che è “primario” da ciò che è “secondario”.
- **Componenti**:
  - Riga singola o doppia con elementi a bassa enfasi visiva.
  - Separazione dal footer principale tramite spacing o linea sottile (coerente con brand).

## Accessibilità
- Struttura semantica: usare contenitori di sezione con titoli (es. heading coerente nel livello) e liste per i link.
- Contrasto: verificare che testo/link rispettino un contrasto leggibile sul background del footer.
- Navigazione tastiera: ordine logico, focus sempre visibile.

## Vincoli (da rispettare)
- Nessun cambio al layout generale della pagina.
- Mantenere identità grafica (palette, font, stile complessivo).
- Intervento limitato a: riduzione elementi, gerarchia, spaziatura, chiarezza delle sezioni.