# Course Media — App Akademie

Video-Hosting für LMS-Kurseinheiten via GitHub Pages.

## URL-Schema

```
https://jpappakademie.github.io/course-media/videos/{kurs}/{dateiname}.mp4
```

### Beispiele

- `https://jpappakademie.github.io/course-media/videos/ux/gestalt_proximity_demo.mp4`
- `https://jpappakademie.github.io/course-media/videos/figma/auto_layout_walkthrough.mp4`

## Ordnerstruktur

```
videos/
├── ux/       ← UX-Kurs Videos
├── ui/       ← UI-Kurs Videos
└── figma/    ← Figma-101 Videos
```

## Videos hochladen

1. Auf GitHub dieses Repo öffnen
2. In den passenden Ordner navigieren (z.B. `videos/ux/`)
3. **Add file → Upload files** → Video reinziehen → Commit
4. URL ist sofort verfügbar (nach ~1 Min.)

## Im LMS verwenden (HTML-Template)

Autoplay-Loop (wie GIF):
```html
<video src="https://jpappakademie.github.io/course-media/videos/ux/DATEINAME.mp4"
  style="width:100%; height:auto; display:block; border-radius:38px;
  box-shadow: 0 9px 28px rgba(0,0,0,0.1); border:1px solid rgba(0,0,0,0.03);
  margin: 24px 0 0 0;"
  autoplay loop muted playsinline></video>
```

Mit Play-Button:
```html
<video src="https://jpappakademie.github.io/course-media/videos/ux/DATEINAME.mp4"
  style="width:100%; height:auto; display:block; border-radius:38px;
  box-shadow: 0 9px 28px rgba(0,0,0,0.1); border:1px solid rgba(0,0,0,0.03);
  margin: 24px 0 0 0;"
  controls playsinline preload="metadata"></video>
```

## Limits

- Max. Dateigröße pro Upload: **100 MB** (GitHub Limit)
- Empfehlung: Videos unter 10 MB halten (kurze Clips, komprimiert)
- GitHub Pages Bandbreite: 100 GB/Monat (mehr als genug)
