# Vimo welkomstscherm

Welkomstscherm voor de tv in de showroom van Vanerum. Vimo, de mascotte van Vanerum, heet bezoekers welkom en doet tussendoor bewegingen met de Motion Cube. Links staan wisselende weetjes.

- Eén bestand: `index.html`. Lettertype, logo en Vimo zitten erin, dus de pagina haalt niets van internet op.
- Licht: platte 2D-Vimo (SVG), geen 3D. Geschikt voor een Android-box of smart-tv.
- Vast 16:9 (1920 × 1080), schaalt naar elk scherm. Muispijl verborgen; elke tien minuten schuift het beeld een paar pixels tegen inbranden.

## Teksten aanpassen

Bovenin `index.html` staat het blok **Teksten**: de welkomsttekst, de ondertitel, de weetjes en wat Vimo zegt en doet. Pas ze daar aan en push naar `main`.

## Publiceren op Cloudflare Pages

1. Cloudflare-dashboard → **Workers & Pages** → **Create** → tab **Pages** → **Connect to Git**.
2. Kies deze repository.
3. Framework preset: **None**. Build command: leeg laten. Build output directory: `/`.
4. **Save and Deploy**. Elke push naar `main` zet daarna automatisch een nieuwe versie online.

`_headers` zorgt dat het scherm altijd de nieuwste versie ophaalt.

## In AbleSign

**Websites → Add website**, plak het adres van de Cloudflare-site (bijv. `https://vimo-demo.paul-westerhout.workers.dev`), geef hem een naam en sla op. Sleep hem daarna bij **Screens** in de playlist van het scherm en zet de duur zo lang mogelijk.
