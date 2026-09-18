# BFI-2 Test Italiano

Implementazione web interattiva e pronta all'uso della versione italiana ufficiale del **Big Five Inventory-2 (BFI-2)**, questionario scientificamente validato per la valutazione dei cinque grandi fattori della personalità e delle relative 15 sfaccettature gerarchiche (facets).

---

## Stato del Progetto

- **Funzionante e autonomo**: applicazione web single-page (`index.html`) pura (HTML5, CSS3, Vanilla JavaScript), priva di framework o librerie esterne e senza alcuna dipendenza lato server.
- **Questionario standard a 60 item**: tutti i 60 quesiti del BFI-2 sono implementati con l'adattamento linguistico italiano ufficiale.
- **Calcolo psicometrico standard**:
  - Calcolo del punteggio medio (scala Likert 1–5) per i **5 macro-tratti** (Big Five).
  - Calcolo del punteggio medio (scala Likert 1–5) per ciascuna delle **15 sfaccettature** (3 sfaccettature per ogni dominio).
  - Gestione dell'inversione di polarità (*reverse-keyed items*) per gli item formulati in direzione opposta (`punteggio = 6 - risposta`).
- **Esperienza utente**:
  - Indicatore di avanzamento compilazione in tempo reale.
  - Verifica automatica di completezza: avviso contestuale se uno o più item non sono stati compilati.
  - Visualizzazione immediata dei risultati con grafici a barre percentuali e schede dettagliate delle sfaccettature.
- **Pronto per il deploy statico**: configurazione inclusa (`statichost.yml`) per pubblicazione diretta su GitHub Pages, Statichost o qualsiasi hosting di file statici.

---

## Riferimenti Bibliografici e Fonti

Il presente lavoro si fonda direttamente sui contributi scientifici originali e sul relativo studio di validazione e adattamento per il contesto italiano:

### 1. Studio Fondativo e Modello Originale (BFI-2)
- **Autori**: Christopher J. Soto (Colby College) & Oliver P. John (University of California, Berkeley).
- **Titolo**: *The next Big Five Inventory (BFI-2): Developing and assessing a hierarchical model with 15 facets to enhance bandwidth, fidelity, and predictive power*.
- **Rivista**: *Journal of Personality and Social Psychology*, 2017, Vol. 113, No. 1, pp. 117–143.
- **DOI**: [10.1037/pspp0000096](https://doi.org/10.1037/pspp0000096)
- **Versione online di riferimento**: [The Personality Lab - BFI-2 Self-Report](https://www.personalitylab.org/tests/bfi2_self_pol.htm)

### 2. Validazione e Adattamento Italiano (BFI-2-R)
- **Autori**: Roberto Burro, Ivana Bianchi & Daniela Raccanello (Dipartimento di Scienze Umane, Università degli Studi di Verona).
- **Titolo**: *Improving the Big Five Inventory-2 in an Italian context using Rasch Analysis (BFI-2-R)*.
- **Rivista**: *Current Psychology*, 2025.
- **DOI**: [10.1007/s12144-025-07584-7](https://doi.org/10.1007/s12144-025-07584-7)
- **Archivio istituzionale IRIS (Open Access)**: [BFI-2-R.pdf - Università di Verona](https://iris.univr.it/retrieve/238d2aab-52d6-4702-bbfa-d4193577ac01/BFI-2-R.pdf)

---

## Struttura del Test (Domini e Sfaccettature)

Il questionario valuta 5 macro-domini, ciascuno articolato in 3 sfaccettature specifiche (4 item per sfaccettatura, per un totale di 12 item a dominio):

| Dominio | Sfaccettature (Facets) | Codice |
| :--- | :--- | :---: |
| **Estroversione** *(Extraversion)* | Sociabilità (*Sociability*), Assertività (*Assertiveness*), Energia / Vitalità (*Energy*) | `E` |
| **Gradevolezza** *(Agreeableness)* | Compassione (*Compassion*), Rispettosità (*Respectfulness*), Fiducia (*Trust*) | `A` |
| **Coscienziosità** *(Conscientiousness)* | Organizzazione (*Organization*), Produttività (*Productivity*), Responsabilità (*Responsibility*) | `C` |
| **Emotività Negativa** *(Negative Emotionality)* | Ansia (*Anxiety*), Depressione / Tono dell'umore (*Depression*), Volatilità Emotiva (*Emotional Volatility*) | `N` |
| **Apertura Mentale** *(Open-Mindedness)* | Curiosità Intellettuale (*Intellectual Curiosity*), Sensibilità Estetica (*Aesthetic Sensitivity*), Creatività / Immaginazione (*Creative Imagination*) | `O` |

---

## Scelte Metodologiche e Adattamenti Applicativi

Rispetto ai documenti di ricerca, sono state adottate le seguenti scelte di implementazione:

- **Estrazione della forma standard a 60 item dal pool di ricerca esteso**:
  Il documento di validazione italiana dell'Università di Verona include un pool sperimentale di 125 elementi. Per questa implementazione interattiva sono stati isolati ed estratti esclusivamente i **60 item ufficiali** selezionati nello studio per la versione standard BFI-2. Questo garantisce il rispetto del disegno psicometrico originale, in cui ogni sfaccettatura comprende esattamente 2 item con formulazione diretta e 2 item a polarità invertita per prevenire il bias di acquiescenza.

- **Armonizzazione sintattica dell'incipit**:
  In accordo con le istruzioni standard per l'autovalutazione, le domande sono introdotte dall'indicazione:
  > *"Ci si vede come una persona che..."*
  Il testo dei 60 item è stato raccordato grammaticalmente per garantire una lettura fluida e naturale in lingua italiana senza alterare il significato psicometrico originario.

- **Ordinamento standardizzato delle sfaccettature**:
  Nel report di calcolo finale le sfaccettature sono raggruppate e presentate sempre nel medesimo ordine canonico per facilitare la lettura, la comparazione con la letteratura scientifica e il confronto con i dati normativi.

---

## Utilizzo in Locale

Per testare o eseguire il questionario localmente sul proprio computer:

1. Clonare o scaricare il repository.
2. Aprire direttamente il file `index.html` con un qualsiasi browser web (Chrome, Firefox, Safari, Edge). Non sono necessarie installazioni, server locali o comandi da terminale.

---

## Note su Copyright e Licenza

- Il modello e gli item originali del BFI-2 sono protetti da copyright © 2015 di Christopher J. Soto e Oliver P. John. Il loro impiego è liberamente consentito per scopi di ricerca, clinici, accademici ed educativi non commerciali.
- L'adattamento psicometrico e linguistico per il contesto italiano fa riferimento allo studio di Roberto Burro, Ivana Bianchi e Daniela Raccanello (Università di Verona, 2025).
