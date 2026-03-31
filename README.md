# AI Captions App

Nahrál jsem video, řekl Claudovi co chci — a za hodinu vznikla plně funkční aplikace na titulky.

Žádný kurz. Žádné tutoriály. Jen správný prompty.

Nahraj video → AI přepíše → Upravíš editor → Exportuješ s titulky

---

## 🏗️ Jak to funguje

### Architektura

```
Nahraj video
    ↓
/api/upload         → uloží video lokálně
    ↓
/api/transcribe     → FFmpeg extrahuje audio → OpenAI Whisper → word timestamps
    ↓
Editor              → VideoPlayer (9:16) + TranscriptEditor + StylePanel
    ↓
/api/export         → FFmpeg vypálí .ass titulky do videa → MP4
```

---

## Co to umí

- Automaticky přepíše mluvené slovo z videa
- Každé slovo se zvýrazní přesně ve chvíli, kdy je řečeno
- Funguje i na videa s hudbou na pozadí
- 4 vizuální styly titulků
- Náhled v 9:16 — vidíš přesně jak to bude vypadat na Instagramu
- Export MP4 s titulky vypálenými přímo do videa

---

## Jak to vzniklo

Tohle není výsledek měsíců programování.

Je to výsledek toho, že víš **jak správně komunikovat s AI** — jak strukturovat zadání, jak iterovat, jak dostat přesně to co chceš.

Kdybych ti dal zdrojový kód bez kontextu, budeš stuck na prvním problému.

Celý postup — krok za krokem, včetně promptů a rozhodnutí které jsem dělal — je uvnitř komunity.

---

<div align="center">

<img src="headshot.jpg" width="180" />

### Celý postup je v Makers Clubu

Přidej se a postav to taky — krok za krokem, od nuly.

**[→ Makers Club](https://www.skool.com/makers-club-7388/about)**

*@krystof_ai*

</div>
