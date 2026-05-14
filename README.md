# NextPhase Partners Website

Sito web moderno e responsivo per NextPhase Partners - agenzia di consulenza IT specializzata in cloud, AI e digital transformation.

## 🚀 Tecnologie Utilizzate

- **React 18** - Frontend framework
- **Vite** - Build tool veloce
- **Tailwind CSS** - Utility-first CSS framework
- **Lucide React** - Icon library
- **Formspree** - Form submission handling

## 📋 Prerequisiti

- Node.js (versione 16+)
- npm o yarn

## 🛠️ Setup Locale

### 1. Installazione dipendenze

```bash
cd nextphase-website
npm install
```

### 2. Avvia il server di sviluppo

```bash
npm run dev
```

Il sito sarà disponibile su `http://localhost:3000`

### 3. Build per produzione

```bash
npm run build
```

I file compilati saranno in `dist/`

## 🌐 Deployment su Vercel (Gratuito)

### Opzione 1: Deploy via CLI

```bash
# Installa Vercel CLI
npm i -g vercel

# Deploy
vercel
```

Segui le istruzioni e il sito sarà live in pochi secondi.

### Opzione 2: Deploy via GitHub

1. Carica il progetto su GitHub
2. Vai su [vercel.com](https://vercel.com)
3. Clicca "New Project"
4. Seleziona il repository
5. Vercel farà il deploy automaticamente

**Il sito sarà disponibile su:** `https://nextphasepartners.vercel.app`

**Per usare il dominio nextphasepartners.it:**
- Vai su DNS settings su Vercel
- Aggiungi il dominio
- Aggiorna i DNS dal registrar (Namecheap, GoDaddy, etc.)

## 📧 Form di Contatto

Il form è configurato per funzionare con **Formspree** (gratuito fino a 50 form/mese).

ID Formspree attuale: `mldkokdo`

Per cambiarlo:
1. Vai su [formspree.io](https://formspree.io)
2. Registrati
3. Crea un nuovo form
4. Copia il form ID
5. Modifica in `src/components/Contact.jsx`:
   ```javascript
   fetch('https://formspree.io/f/YOUR_FORM_ID', { ... })
   ```

## 🎨 Personalizzazione

### Colori
I colori principali sono definiti in `tailwind.config.js`:
- Blu Navy: `#001a4d`
- Blu Medio: `#0066cc`
- Azzurro Ciano: `#00d4ff`

### Testo e Contenuti
Modifica i componenti in `src/components/` per aggiornare i testi.

### Case Studies
Modifica l'array `caseStudies` in `src/components/CaseStudies.jsx`

### Team
Modifica l'array `team` in `src/components/About.jsx`

## 📱 Responsiveness

Il sito è completamente responsive:
- Mobile (320px+)
- Tablet (768px+)
- Desktop (1024px+)

## 🔍 SEO

- Meta tags ottimizzati in `index.html`
- Open Graph tags per social media
- Sitemap automatica (aggiungere se necessario)

## 📦 Struttura Progetto

```
nextphase-website/
├── src/
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── Hero.jsx
│   │   ├── Services.jsx
│   │   ├── CaseStudies.jsx
│   │   ├── About.jsx
│   │   ├── Contact.jsx
│   │   └── Footer.jsx
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── package.json
├── vite.config.js
├── tailwind.config.js
└── postcss.config.js
```

## 🚀 Performance

- Vite per compilazione ultra-veloce
- Tailwind CSS per CSS ottimizzato
- Immagini ottimizzate
- Code splitting automatico

Lighthouse Score target: 90+ per Performance, Accessibility, Best Practices, SEO

## 📞 Email Contatti

L'email di contatto è `info@nextphasepartners.it` (vedi in `src/components/Contact.jsx` e `src/components/Footer.jsx`)

## 🔐 Sicurezza

- HTTPS obbligatorio (su Vercel automatico)
- Nessun dato sensibile personale nel sito
- Form dati inviati via Formspree (server sicuro)

## 📝 License

NextPhase Partners © 2024. Tutti i diritti riservati.

## ❓ Problemi Comuni

### Il form non funziona
- Controlla il form ID di Formspree
- Assicurati di aver confermato l'email su formspree.io
- Verifica la console browser per errori

### Build fallisce
```bash
rm -rf node_modules package-lock.json
npm install
npm run build
```

### Sito lento
- Controlla le immagini (devono essere ottimizzate)
- Usa DevTools di Chrome per identificare bottleneck
- Considera l'aggiunta di un CDN per risorse statiche

---

**Domande?** Contatta: info@nextphasepartners.it
