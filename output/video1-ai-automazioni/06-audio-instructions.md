# GUIDA COMPLETA GENERAZIONE AUDIO
## Video 1: "5 Automazioni AI che Ti Fanno Risparmiare 10 Ore a Settimana"

---

## SEZIONE 1: GENERAZIONE AUDIO CON NOTEBOOKLM

### 1.1 Preparazione del Documento Sorgente

Il file `02-notebooklm-source.md` e' gia' ottimizzato per NotebookLM. Contiene:
- Dati strutturati con numeri e statistiche conversazionali
- Comparazioni prima/dopo per facilitare la discussione
- Guida alla pronuncia dei termini tecnici
- Esempi pratici per rendere i concetti tangibili

### 1.2 Accesso a NotebookLM

1. Vai su: https://notebooklm.google.com
2. Accedi con il tuo account Google
3. Clicca su "New Notebook" (Nuovo Notebook)

### 1.3 Caricamento del Documento

1. Clicca su "Add Source" (Aggiungi Fonte)
2. Seleziona "Upload" e carica il file `02-notebooklm-source.md`
3. Attendi l'elaborazione del documento (circa 30-60 secondi)
4. Verifica che il documento sia stato analizzato correttamente

### 1.4 Generazione Audio Overview (Deep Dive)

1. Una volta caricato il documento, cerca l'opzione "Audio Overview" nel pannello destro
2. Clicca su "Generate" per avviare la generazione
3. Tempo di elaborazione: 5-15 minuti per audio di 10-15 minuti
4. NotebookLM generera' una conversazione tra due "host" che discutono il contenuto

### 1.5 Personalizzazione della Generazione

Prima di generare, puoi aggiungere istruzioni personalizzate:

```
Focus on:
- Practical applications for Italian small businesses
- Cost-benefit analysis for each automation
- Real-world examples and case studies
- Pronunciation of technical terms in Italian context
- Conversational but professional tone

Avoid:
- Overly technical jargon
- Abstract theoretical discussions
- English-only explanations without Italian context
```

### 1.6 Lingua e Localizzazione

**IMPORTANTE:** NotebookLM genera audio principalmente in inglese. Per contenuti in italiano:

**Opzione A - Post-produzione con Doppiaggio:**
1. Genera l'audio in inglese
2. Usa il testo trascritto come base per il doppiaggio italiano
3. Registra il voice-over con uno speaker italiano

**Opzione B - ElevenLabs Voice Cloning (Consigliato):**
1. Esporta la trascrizione da NotebookLM
2. Traduci il testo in italiano (o usa la versione italiana del source)
3. Usa ElevenLabs per generare la voce con tono conversazionale

**Opzione C - Registrazione Diretta:**
1. Usa il documento sorgente come script
2. Registra direttamente la narrazione con uno speaker

---

## SEZIONE 2: ALTERNATIVE PER AUDIO IN ITALIANO

### 2.1 ElevenLabs (Consigliato per Qualita')

**Sito:** https://elevenlabs.io

**Voci Italiane Disponibili:**
- Giovanni (maschile, professionale)
- Marco (maschile, caldo)
- Francesca (femminile, naturale)
- Custom voice cloning (con 3 minuti di sample audio)

**Impostazioni Ottimali per Narrazione:**
```
Voice Settings:
- Stability: 0.50 (per naturalezza)
- Clarity + Similarity: 0.75 (per chiarezza)
- Style Exaggeration: 0.30 (leggera espressivita')

Model: Eleven Multilingual v2
```

**Costi:**
- Free: 10.000 caratteri/mese
- Starter: $5/mese - 30.000 caratteri
- Creator: $22/mese - 100.000 caratteri
- Per script completo (15 min): circa 15.000-20.000 caratteri

### 2.2 Azure Neural TTS

**Voci Italiane di Alta Qualita':**
- it-IT-DiegoNeural (maschile)
- it-IT-ElsaNeural (femminile)
- it-IT-GiuseppeNeural (maschile, professionale)

**Vantaggi:**
- Qualita' audio professionale
- SSML per controllo avanzato di pausa e intonazione
- Pay-as-you-go economico

### 2.3 Google Cloud TTS

**Voci Italiane WaveNet:**
- it-IT-Wavenet-A/B/C/D

**Impostazioni:**
```
Speaking Rate: 0.9-1.0 (leggermente rallentato per chiarezza)
Pitch: 0 (naturale)
Volume Gain: 0 dB
```

---

## SEZIONE 3: REQUISITI TECNICI AUDIO FINALE

### 3.1 Specifiche per YouTube

| Parametro | Valore Raccomandato |
|-----------|---------------------|
| Formato | AAC o MP3 |
| Bitrate | 320 kbps (MP3) / 256 kbps (AAC) |
| Sample Rate | 48 kHz |
| Canali | Stereo (2.0) o Mono |
| Loudness | -14 LUFS (standard YouTube) |
| True Peak | -1 dB max |

### 3.2 Formato File di Lavoro

Per editing:
- WAV 48kHz 24-bit (qualita' massima)
- AIFF 48kHz 24-bit (alternativa Mac)

Per esportazione finale:
- AAC 256kbps (migliore compressione)
- MP3 320kbps (compatibilita' universale)

### 3.3 Loudness e Normalizzazione

**Strumenti Consigliati:**
- Youlean Loudness Meter (gratuito, plugin DAW)
- Audacity con plugin loudness (gratuito)
- Adobe Audition Match Loudness

**Processo:**
1. Analizza loudness attuale del file audio
2. Normalizza a -14 LUFS integrato
3. Verifica che i picchi non superino -1 dB
4. Esporta con le specifiche corrette

---

## SEZIONE 4: STRUTTURA AUDIO PER SEZIONI VIDEO

### 4.1 Breakdown Temporale

| Sezione | Inizio | Fine | Durata | Note Audio |
|---------|--------|------|--------|------------|
| Hook | 0:00 | 0:30 | 30s | Energia alta, gancio immediato |
| Intro | 0:30 | 1:30 | 60s | Tono confidenziale, posizionamento |
| Auto #1 Email | 1:30 | 3:45 | 135s | Ritmo moderato, esempi pratici |
| Auto #2 Fatture | 3:45 | 6:00 | 135s | Numeri chiari, pause per grafiche |
| Auto #3 Social | 6:00 | 8:15 | 135s | Energia crescente, workflow |
| Auto #4 Riunioni | 8:15 | 10:30 | 135s | Tono problem-solution |
| Auto #5 WhatsApp | 10:30 | 12:30 | 120s | Esempi conversazionali |
| Riepilogo | 12:30 | 13:00 | 30s | Riassunto energico |
| CTA | 13:00 | 13:30+ | 30s+ | Chiamata all'azione chiara |

### 4.2 Indicazioni per Tono e Ritmo

**Hook (0:00-0:30):**
- Voce energica ma non urlata
- Pausa breve dopo il gancio iniziale
- Articolazione chiara dei numeri

**Sezioni Automazioni:**
- Ritmo narrativo costante
- Enfasi su parole chiave (risparmio, automatico, gratuito)
- Pause naturali per transizioni

**Riepilogo e CTA:**
- Energia crescente
- Tono diretto e personale
- Chiusura calorosa

---

## SEZIONE 5: POST-PRODUZIONE AUDIO

### 5.1 Editing Consigliato

1. **Rimozione Silenzi Lunghi:** Taglia pause superiori a 0.5 secondi
2. **Noise Reduction:** Applica riduzione rumore se necessario (Audacity: Noise Reduction -12dB)
3. **EQ Voice Enhancement:**
   - High-pass filter a 80Hz (rimuove rumble)
   - Boost leggero a 2-4kHz (+2dB per presenza)
   - De-essing se necessario (6-8kHz)

4. **Compressione:**
   - Ratio: 3:1
   - Threshold: -18dB
   - Attack: 10ms
   - Release: 100ms

### 5.2 Aggiunta Musica di Sottofondo

**Fonti Royalty-Free Consigliate:**
- Epidemic Sound (abbonamento, alta qualita')
- Artlist (abbonamento, ampia libreria)
- YouTube Audio Library (gratuito)
- Pixabay Music (gratuito)

**Mix Consigliato:**
- Voce: -6 dB
- Musica di sottofondo: -24 dB (ducking a -30 dB durante parlato)

**Stile Musicale per il Video:**
- Genere: Corporate/Motivational/Technology
- Tempo: 100-120 BPM
- Mood: Ottimista, progressivo, professionale
- Evitare: Musica troppo drammatica o generica "upbeat"

### 5.3 Sound Effects

Effetti sonori consigliati per transizioni:
- Whoosh leggero per cambio sezione
- Soft click/tap per punti elenco
- Subtle chime per highlights
- Typing sounds per screen recording

**Fonti:**
- Freesound.org (gratuito, Creative Commons)
- Zapsplat (gratuito con attribuzione)
- SoundSnap (premium)

---

## SEZIONE 6: CHECKLIST FINALE AUDIO

### Pre-Produzione
- [ ] File sorgente `02-notebooklm-source.md` caricato su NotebookLM
- [ ] Istruzioni personalizzate aggiunte (opzionale)
- [ ] Scelta tra generazione automatica o registrazione diretta

### Generazione
- [ ] Audio generato/registrato per intero
- [ ] Durata target: 12-15 minuti
- [ ] Tutti i termini tecnici pronunciati correttamente

### Post-Produzione
- [ ] Noise reduction applicata
- [ ] EQ ottimizzata per voce
- [ ] Compressione applicata
- [ ] Loudness normalizzata a -14 LUFS
- [ ] Picchi sotto -1 dB

### Esportazione
- [ ] Formato: WAV 48kHz 24-bit (per editing video)
- [ ] Backup: MP3 320kbps (per archivio)
- [ ] File nominato: `video1-audio-final.wav`

### Integrazione
- [ ] Audio sincronizzato con timeline video
- [ ] Musica di sottofondo aggiunta
- [ ] Sound effects per transizioni

---

## SEZIONE 7: OUTPUT FILE ATTESI

Al termine del processo, avrai:

1. **File Audio Principale:**
   - Nome: `video1-audio-narration.wav`
   - Durata: 12-15 minuti
   - Formato: WAV 48kHz 24-bit

2. **File Audio con Musica:**
   - Nome: `video1-audio-mixed.wav`
   - Include narrazione + sottofondo musicale

3. **File Audio Esportato:**
   - Nome: `video1-audio-final.mp3`
   - Formato: MP3 320kbps
   - Pronto per backup/archivio

---

*Documento generato da MediaSynth Core per tube-forge-agents-team*
*Versione: 1.0 | Data: 2025-12-15*
