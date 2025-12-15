# GUIDA COMPLETA PRODUZIONE VIDEO
## Video 1: "5 Automazioni AI che Ti Fanno Risparmiare 10 Ore a Settimana"

---

## PANORAMICA PRODUZIONE

| Fase | Descrizione | Tempo Stimato |
|------|-------------|---------------|
| 1 | Pre-Produzione | 2-3 ore |
| 2 | Generazione Asset AI | 4-6 ore |
| 3 | Screen Recording | 2-3 ore |
| 4 | Registrazione Audio | 1-2 ore |
| 5 | Editing Video | 4-6 ore |
| 6 | Color Grading & VFX | 2-3 ore |
| 7 | Audio Mixing | 1-2 ore |
| 8 | Export & Upload | 1 ora |
| **TOTALE** | | **17-26 ore** |

---

## FASE 1: PRE-PRODUZIONE

### 1.1 Preparazione Workspace

Crea la seguente struttura cartelle:

```
video1-ai-automazioni/
    01-script/
        script-completo.md
        timestamps.txt
    02-audio/
        raw/
        processed/
        music/
        sfx/
    03-video/
        ai-generated/
            scene01/
            scene02/
            ...
        screen-recordings/
        stock-footage/
        graphics/
    04-project/
        davinci/
        capcut/
    05-export/
        drafts/
        final/
    06-thumbnails/
```

### 1.2 Raccolta Asset Necessari

**Materiali Obbligatori:**
- [ ] Script finale approvato (`01-script-completo.md`)
- [ ] Audio narrazione completato
- [ ] Clip AI generate (8 scene)
- [ ] Screen recording dei tool
- [ ] Musica di sottofondo
- [ ] Sound effects
- [ ] Logo canale
- [ ] Font del brand

**Materiali Opzionali:**
- [ ] B-roll stock footage
- [ ] Lower thirds template
- [ ] Transizioni personalizzate
- [ ] Intro/Outro pre-renderizzati

---

## FASE 2: GENERAZIONE ASSET AI

### 2.1 Ordine di Generazione Consigliato

1. **Scene Critiche Prima:**
   - Scena 1 (Hook) - Prima impressione
   - Scena 8 (Outro) - Ultima impressione
   - Genera 3-4 varianti ciascuna

2. **Scene B-Roll Dopo:**
   - Scene 3-7 (automazioni)
   - 1-2 varianti sufficienti

3. **Thumbnail Alla Fine:**
   - Dopo aver definito stile visivo
   - 3 opzioni per A/B testing

### 2.2 Quality Control Asset

Per ogni clip AI generata, verifica:
- [ ] Risoluzione corretta (1080p minimo)
- [ ] Aspect ratio 16:9
- [ ] Nessun artefatto visivo evidente
- [ ] Movimento fluido (no jitter)
- [ ] Coerenza con brief creativo
- [ ] Durata adeguata

---

## FASE 3: SCREEN RECORDING

### 3.1 Software Consigliati

| Software | Pro | Contro | Costo |
|----------|-----|--------|-------|
| OBS Studio | Gratuito, potente | Curva apprendimento | Free |
| ScreenFlow | Facile, editing integrato | Solo Mac | $169 |
| Camtasia | Professionale, effetti | Costoso | $299 |
| Loom | Veloce, cloud | Qualita' limitata | Freemium |

### 3.2 Impostazioni Recording

```
Resolution: 1920x1080 (match output)
Frame Rate: 30 fps
Encoder: x264 o GPU (NVENC/QuickSync)
Bitrate: 20-30 Mbps (alta qualita')
Audio: Sistema + Microfono separati
Cursor: Evidenziato, ingrandito
```

### 3.3 Checklist Screen Recording

**Preparazione:**
- [ ] Chiudi applicazioni non necessarie
- [ ] Disattiva notifiche (Focus Mode)
- [ ] Pulisci desktop
- [ ] Prepara account demo (senza dati reali)
- [ ] Testa audio prima di iniziare

**Durante Recording:**
- [ ] Movimenti mouse lenti e deliberati
- [ ] Pause di 2-3 secondi su elementi importanti
- [ ] Click chiari e visibili
- [ ] Evita scroll veloci

**Clip Necessarie:**
1. [ ] Gmail inbox con email che arrivano
2. [ ] Zapier automation builder
3. [ ] ChatGPT generazione risposta email
4. [ ] Fatture in Cloud dashboard
5. [ ] Fatture in Cloud ricorrente setup
6. [ ] Canva editor con Magic Write
7. [ ] Canva Content Planner
8. [ ] Otter.ai trascrizione live
9. [ ] ManyChat flow builder
10. [ ] WhatsApp Business con bot attivo

---

## FASE 4: EDITING VIDEO

### 4.1 Software Consigliati

#### DaVinci Resolve (Consigliato - Gratuito)

**Pro:**
- Professionale e completo
- Color grading eccellente
- Fusion per VFX
- Fairlight per audio

**Setup Progetto:**
```
Timeline Resolution: 1920x1080
Frame Rate: 30 fps (o 24 per look cinematico)
Color Science: DaVinci YRGB Color Managed
Working Color Space: Rec.709
```

#### CapCut (Alternativa Facile)

**Pro:**
- Interfaccia semplice
- Template pronti
- Sottotitoli automatici
- Export diretto social

**Ideale per:**
- Principianti
- Editing veloce
- Mobile-first workflow

### 4.2 Struttura Timeline

```
Video Track 5: Titoli, Lower Thirds, Grafiche
Video Track 4: Overlay, Transizioni
Video Track 3: B-Roll, Clip AI
Video Track 2: Screen Recording
Video Track 1: Main footage (host on camera)
Audio Track 1: Voce Principale
Audio Track 2: Musica Sottofondo
Audio Track 3: Sound Effects
Audio Track 4: Ambiente/Room Tone
```

### 4.3 Ritmo di Editing

**Hook (0:00-0:30):**
- Cut veloci ogni 3-5 secondi
- Movimento dinamico
- Transizioni energiche

**Corpo Video (1:30-12:30):**
- Cut ogni 10-15 secondi
- Alternare host/screen recording/B-roll
- Transizioni pulite (dissolve, wipe)

**Riepilogo e CTA (12:30+):**
- Ritmo moderato
- Focus su call to action
- Grafiche riassuntive

### 4.4 Transizioni Consigliate

| Tipo | Uso | Durata |
|------|-----|--------|
| Cut | Standard, energia | 0 frame |
| Cross Dissolve | Cambio tempo/location | 15-30 frame |
| Wipe | Nuova sezione | 20-30 frame |
| Zoom | Stesso soggetto, enfasi | 10-15 frame |
| Whip Pan | Energia, dinamismo | 8-12 frame |

---

## FASE 5: SINCRONIZZAZIONE AUDIO/VIDEO

### 5.1 Workflow di Sync

1. **Importa Audio Narrazione:**
   - Trascina WAV in timeline
   - Allinea inizio con inizio video

2. **Crea Marker Audio:**
   - Segna inizio ogni sezione (da timestamps)
   - Segna punti chiave per B-roll

3. **Taglia e Posiziona Video:**
   - Allinea clip video ai marker audio
   - B-roll durante spiegazioni lunghe
   - Torna a "host" per punti chiave

4. **Verifica Lip Sync (se host on camera):**
   - Zoom sulla bocca
   - Verifica allineamento parole
   - Regola con shift millisecondi se necessario

### 5.2 Timing Consigliato

```
Narrazione che dice "Guarda questo esempio":
-> 0.5 secondi DOPO: Compare screen recording

Narrazione che dice un numero/dato:
-> CONTEMPORANEAMENTE: Appare grafica con numero

Transizione a nuova automazione:
-> 1 secondo PRIMA: Inizia transizione visiva
-> 0.5 secondi PRIMA: Inizia musica di transizione
```

---

## FASE 6: GRAFICA E LOWER THIRDS

### 6.1 Elementi Grafici Necessari

| Elemento | Quantita' | Template |
|----------|-----------|----------|
| Lower Third (nome tool) | 5+ | Nome Tool + Icona + Costo |
| Numero/Statistica | 10+ | Grande numero + descrizione |
| Checklist animata | 5 | Lista con check che appaiono |
| Divisore sezione | 5 | "Automazione #X" |
| CTA finale | 1 | Subscribe + Like + Link |

### 6.2 Stile Grafico Consigliato

```
Font Titoli: Montserrat Bold o Inter Bold
Font Corpo: Open Sans o Roboto
Colore Primario: #2563EB (blu professionale)
Colore Secondario: #10B981 (verde successo)
Colore Accento: #F59E0B (arancione energia)
Sfondo Grafiche: Semi-trasparente nero/bianco
Animazioni: Ease-in-out, durata 0.3-0.5s
```

### 6.3 Lower Third Template

```
+------------------------------------------+
|  [ICONA]  NOME STRUMENTO                 |
|           Costo: XX EUR/mese  |  Free    |
+------------------------------------------+

Animazione: Slide-in da sinistra, 0.4s ease-out
Durata on-screen: 4-6 secondi
Exit: Fade-out 0.3s
```

---

## FASE 7: COLOR GRADING

### 7.1 Look Consigliato

**Stile:** Professionale ma accessibile, non corporate freddo

**Impostazioni Base (DaVinci):**
```
Lift: Leggero aumento blu nelle ombre
Gamma: Neutro
Gain: Leggero aumento arancione negli highlights
Contrast: +5-10%
Saturation: +5-10%
Skin Tone Qualifier: Proteggi toni pelle
```

### 7.2 LUT Consigliate

| LUT | Uso | Fonte |
|-----|-----|-------|
| Rec709 Clean | Base naturale | DaVinci inclusa |
| Film Look Soft | Cinematico leggero | Ground Control |
| Corporate Bright | Professionale luminoso | Color Grading Central |

### 7.3 Consistenza tra Clip

1. **Applica correzione base a tutto:**
   - Bilancia exposure
   - Correggi white balance

2. **Applica look creativo:**
   - Usa adjustment layer/compound clip
   - Stessa LUT per tutte le clip

3. **Match clip AI:**
   - Potrebbero avere look diverso
   - Usa color match per uniformare

---

## FASE 8: AUDIO MIXING FINALE

### 8.1 Livelli Consigliati

| Traccia | Livello | Note |
|---------|---------|------|
| Voce | -6 dB | Sempre in primo piano |
| Musica (parlato) | -24 dB | Ducking attivo |
| Musica (transizioni) | -12 dB | Piu' presente |
| SFX | -12/-18 dB | Non coprire voce |
| Ambiente | -30 dB | Appena percepibile |

### 8.2 Ducking Automatico

**In DaVinci Fairlight:**
1. Traccia Voce come sidechain
2. Musica: Dynamics -> Sidechain Compressor
3. Threshold: -30 dB
4. Ratio: 4:1
5. Attack: 50ms
6. Release: 300ms

**In CapCut:**
- Usa funzione "Auto Adjust Audio"
- O manualmente abbassa musica sotto voce

### 8.3 Master Bus Processing

```
1. EQ: High-pass 60Hz (rimuovi rumble)
2. Compressor: Ratio 2:1, soft knee
3. Limiter: Ceiling -1 dB
4. Loudness: Target -14 LUFS
```

---

## FASE 9: EXPORT SETTINGS

### 9.1 Per YouTube (Consigliato)

**Risoluzione 1080p:**
```
Codec: H.264 (compatibilita') o H.265 (qualita')
Resolution: 1920x1080
Frame Rate: 30 fps
Bitrate: 12-15 Mbps (CBR o VBR 2-pass)
Audio: AAC 320 kbps, 48kHz, Stereo
Container: MP4
```

**Risoluzione 4K (opzionale):**
```
Codec: H.265 (HEVC) consigliato
Resolution: 3840x2160
Frame Rate: 30 fps
Bitrate: 35-45 Mbps
Audio: AAC 320 kbps, 48kHz, Stereo
Container: MP4
```

### 9.2 DaVinci Resolve Export

```
Render Settings:
- Format: QuickTime o MP4
- Codec: H.264 Master
- Resolution: 1920x1080
- Frame Rate: 30
- Quality: Restrict to 15000 Kb/s
- Encoding Profile: High
- Key Frames: Auto

Audio Settings:
- Codec: AAC
- Data Rate: 320 kbps
```

### 9.3 CapCut Export

```
Resolution: 1080p
Frame Rate: 30fps
Quality: High
Format: MP4
Exported File Size: ~500MB per 15 min
```

---

## FASE 10: UPLOAD E OTTIMIZZAZIONE

### 10.1 Filename Conventions

```
Nome File: video1-5-automazioni-ai-risparmio-tempo-FINAL-v1.mp4
Thumbnail: video1-thumbnail-option-A.png
Sottotitoli: video1-sottotitoli-IT.srt
```

### 10.2 YouTube Upload Checklist

**Prima dell'upload:**
- [ ] Video finale esportato correttamente
- [ ] Preview completa senza problemi
- [ ] File size ragionevole (<5GB per 15min)
- [ ] Thumbnail pronta (1280x720 minimo)

**Durante upload:**
- [ ] Titolo ottimizzato SEO
- [ ] Descrizione completa con link
- [ ] Tag rilevanti (15-20)
- [ ] Playlist assegnata
- [ ] Cards e End Screen
- [ ] Sottotitoli caricati
- [ ] Premiere o Publish schedulato

### 10.3 Metadata Consigliato

**Titolo:**
```
5 Automazioni AI che Ti Fanno Risparmiare 10 Ore a Settimana (Gratis!)
```

**Descrizione (Prime righe):**
```
Scopri 5 automazioni AI gratuite che possono farti risparmiare 10+ ore a settimana.
Perfette per piccole imprese e professionisti italiani che vogliono lavorare
in modo piu' smart, non piu' duro.

SCARICA LA CHECKLIST GRATUITA: [link]

TIMESTAMPS:
0:00 - Hook: Il segreto che i consulenti non ti dicono
0:30 - Introduzione: Perche' questo canale esiste
...
```

**Tag:**
```
automazioni ai, intelligenza artificiale business, zapier tutorial italiano,
chatgpt business, automazione email, fatturazione automatica,
social media automation, otter ai italiano, whatsapp business bot,
produttivita' imprenditori, risparmiare tempo, pmi italiane
```

---

## TROUBLESHOOTING COMUNI

### Problema: Audio fuori sync
**Soluzione:** Verifica frame rate consistente. Se diversi, converti tutto allo stesso fps prima di editare.

### Problema: Clip AI con qualita' bassa
**Soluzione:** Rigenera in modalita' High Quality. Usa upscaling AI (Topaz) se necessario.

### Problema: Export file troppo grande
**Soluzione:** Riduci bitrate a 10-12 Mbps. YouTube ri-comprime comunque.

### Problema: Colori diversi tra clip
**Soluzione:** Usa adjustment layer con LUT unificante. Color match in DaVinci.

### Problema: Audio troppo basso
**Soluzione:** Normalizza a -14 LUFS. Usa limiter per alzare volume senza clipping.

---

## TIMELINE PRODUZIONE REALISTICA

### Giorno 1: Pre-Produzione (4 ore)
- Organizzazione file e cartelle
- Raccolta asset esistenti
- Avvio generazione clip AI (batch)

### Giorno 2: Generazione (6 ore)
- Completamento clip AI
- Screen recording tool
- Registrazione audio (se non fatto)

### Giorno 3: Editing Part 1 (4 ore)
- Import tutti gli asset
- Rough cut con audio
- Posizionamento base clip

### Giorno 4: Editing Part 2 (4 ore)
- Fine cut
- Transizioni
- Grafiche e lower thirds

### Giorno 5: Finalizzazione (4 ore)
- Color grading
- Audio mixing
- Export e review
- Correzioni finali
- Upload

**Totale: 5 giorni, 22 ore**

---

*Documento generato da MediaSynth Core per tube-forge-agents-team*
*Versione: 1.0 | Data: 2025-12-15*
