# Sp-rgeskemaUnders-gelseProjekt2
# Spørgeskemaundersøgelse for Turistbureauets Hjemmesidedesigns

## Projektbeskrivelse
Dette projekt er en platform, der præsenterer en række hjemmesidedesigns for brugere i tilfældig rækkefølge med henblik på at indsamle feedback via en spørgeskemaundersøgelse. Formålet er at evaluere brugernes holdning til forskellige designs for et turistbureau.

## Funktionaliteter
- **Visning af hjemmesidedesigns:** Designene præsenteres i tilfældig rækkefølge.
- **Interaktivt spørgeskema:** Brugeren aktiverer selv spørgeskemaet via en tydelig (men ikke for fremtrædende) knap.
- **Datahåndtering:** Svar gemmes anonymt i individuelle JSON-filer.
- **Adminpanel:** Admin kan via et JWT-sikret login:
  - Uploade XML-filen med spørgsmål.
  - Downloade JSON-filer med svar.
  - Se status over antal besvarelser og tilgange.
- **Responsivt Design:** Platformen fungerer på tværs af desktop, tablet og mobil.

## Teknologier
- **Back-end:** Node.js med Express
- **Front-end:** HTML5, CSS3 (plain CSS), JavaScript
- **Datahåndtering:** XML (spørgsmål) og JSON (svar)
- **Sikkerhed:** JWT-token til admin-login

## Installation
1. **Klon dette repository:**
   ```bash
   git clone <repository-url>
   ```
2. **Naviger til projektmappen:**
   ```bash
   cd <project-folder>
   ```
3. **Installer afhængigheder:**
   ```bash
   npm install
   ```
4. **Start serveren:**
   ```bash
   node server.js
   ```

## Brugervejledning
### **For Informanter (Brugere):**
1. Åbn platformen via det medsendte link.
2. Læs introduktionsteksten og klik "Start" for at begynde.
3. Naviger mellem testsiderne og klik på knappen "Besvar spørgeskema" for at udfylde feedback.
4. Besvar spørgeskemaet, og klik "Næste" for at gå videre.

### **For Administratorer:**
1. Log ind på adminpanelet via `admin/login`.
2. Upload XML-filen med spørgsmål.
3. Download JSON-filer med indsamlede svar.
4. Se oversigt over antal besvarelser og tilgange.

## Struktur
```
├── public
│   ├── css
│   ├── images
│   ├── js
│   └── index.html
├── data
│   ├── responses
│   └── questions.xml
├── routes
│   ├── admin.js
│   └── survey.js
├── server.js
├── package.json
└── README.md
```

## Test og Validering
- XML-filen valideres for velformethed ved upload.
- Funktionaliteten testes på tværs af enheder og browsere.
- Admin-login sikres med JWT-token for at forhindre uautoriseret adgang.

## Forbedringsmuligheder
- Udvidelse med statistikvisning for mere detaljeret dataindsigt.
- Implementering af flere spørgeskemaformater for avanceret dataindsamling.

## Kontakt
For spørgsmål eller support, kontakt [dit navn eller din e-mail].
