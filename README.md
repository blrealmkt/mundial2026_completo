<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mundial FIFA 2026 — GDL × 123KLAN</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;500;600;700;800;900&family=Barlow:wght@400;500;600&family=Space+Mono:wght@400;700&display=swap" rel="stylesheet">
<style>
:root {
  --bg: #F5F2EB;
  --bg2: #EDE9DF;
  --bg3: #E3DFD4;
  --white: #FFFFFF;
  --ink: #1A1915;
  --ink2: #3D3C36;
  --ink3: #6B6960;
  --fire: #FF4D1C;
  --fire-light: #FFE8E1;
  --fire-dark: #CC3A12;
  --gold: #D4A820;
  --gold-light: #FFF3CC;
  --gold-dark: #9C7A10;
  --lime: #8FCC00;
  --lime-light: #EEF8D0;
  --green: #2D6A0F;
  --green-light: #E0F0D4;
  --yellow: #FFD600;
  --yellow-dark: #B89A00;
  --red-card: #E02020;
  --red-light: #FDEAEA;
  --blue: #1A4FA0;
  --blue-light: #E4ECFF;
  --border: rgba(26,25,21,0.1);
  --border2: rgba(26,25,21,0.18);
  --shadow: 2px 4px 0px rgba(26,25,21,0.12);
  --font-display: 'Barlow Condensed', sans-serif;
  --font-body: 'Barlow', sans-serif;
  --font-mono: 'Space Mono', monospace;
}

*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

body {
  background: var(--bg);
  font-family: var(--font-body);
  color: var(--ink);
  min-height: 100vh;
  overflow-x: hidden;
}

/* ── HEADER ── */
.site-header {
  background: var(--ink);
  padding: 0 20px;
  position: sticky;
  top: 0;
  z-index: 100;
  border-bottom: 3px solid var(--fire);
}
.header-inner {
  max-width: 1100px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 56px;
  gap: 16px;
}
.logo {
  display: flex;
  align-items: center;
  gap: 10px;
  flex-shrink: 0;
}
.logo-badge {
  background: var(--fire);
  color: #fff;
  font-family: var(--font-display);
  font-weight: 900;
  font-style: italic;
  font-size: 10px;
  letter-spacing: .14em;
  text-transform: uppercase;
  padding: 5px 12px 5px 9px;
  border: 2px solid #fff;
  clip-path: polygon(0 0, 100% 0, 88% 100%, 0% 100%);
  transform: rotate(-3deg);
  flex-shrink: 0;
}
.logo-text {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 22px;
  color: #fff;
  letter-spacing: 0;
  line-height: 1;
  text-transform: uppercase;
}
.logo-text span { color: var(--fire); font-size: 1.15em; }
.live-dot {
  display: flex;
  align-items: center;
  gap: 6px;
  font-family: var(--font-mono);
  font-size: 10px;
  color: var(--lime);
  letter-spacing: .08em;
  text-transform: uppercase;
}
.live-dot::before {
  content: '';
  width: 7px;
  height: 7px;
  border-radius: 50%;
  background: var(--lime);
  animation: pulse 1.4s ease-in-out infinite;
}
@keyframes pulse {
  0%,100% { opacity: 1; transform: scale(1); }
  50% { opacity: .5; transform: scale(.8); }
}

/* ── MAIN NAV ── */
.main-nav {
  background: var(--bg2);
  border-bottom: 1.5px solid var(--border2);
  padding: 0 20px;
  overflow-x: auto;
  scrollbar-width: none;
}
.main-nav::-webkit-scrollbar { display: none; }
.nav-inner {
  max-width: 1100px;
  margin: 0 auto;
  display: flex;
  gap: 0;
}
.nav-btn {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 13px;
  letter-spacing: .08em;
  text-transform: uppercase;
  color: var(--ink3);
  padding: 12px 18px;
  border: none;
  background: none;
  cursor: pointer;
  border-bottom: 3px solid transparent;
  transition: color .15s, border-color .15s;
  white-space: nowrap;
  flex-shrink: 0;
}
.nav-btn:hover { color: var(--ink); }
.nav-btn.active {
  color: var(--fire-dark);
  border-bottom-color: var(--fire);
}

/* ── LAYOUT ── */
.page {
  max-width: 1100px;
  margin: 0 auto;
  padding: 24px 20px 60px;
}
.view { display: none; }
.view.active { display: block; }

/* ── SECTION HEADER ── */
.section-head {
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
  margin-bottom: 16px;
  flex-wrap: wrap;
  gap: 10px;
}
.section-title {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 30px;
  letter-spacing: -.01em;
  line-height: 1;
  color: var(--ink);
  text-transform: uppercase;
}
.section-title span { color: var(--fire); }
.section-sub {
  font-family: var(--font-mono);
  font-size: 10px;
  color: var(--ink3);
  letter-spacing: .1em;
  text-transform: uppercase;
}

/* ── PHASE SELECTOR (resultados) ── */
.phase-pills {
  display: flex;
  gap: 6px;
  flex-wrap: wrap;
  margin-bottom: 20px;
}
.phase-pill {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 11px;
  letter-spacing: .08em;
  text-transform: uppercase;
  padding: 6px 14px;
  border: 1.5px solid var(--border2);
  border-radius: 3px;
  background: var(--white);
  color: var(--ink3);
  cursor: pointer;
  transition: all .15s;
}
.phase-pill:hover { border-color: var(--fire); color: var(--fire-dark); }
.phase-pill.active {
  background: var(--ink);
  color: #fff;
  border-color: var(--ink);
}

/* ── GROUP SELECTOR ── */
.group-selector {
  display: flex;
  gap: 6px;
  margin-bottom: 20px;
  flex-wrap: wrap;
}
.grp-btn {
  font-family: var(--font-display);
  font-weight: 800;
  font-size: 13px;
  letter-spacing: .06em;
  text-transform: uppercase;
  width: 38px;
  height: 38px;
  display: flex;
  align-items: center;
  justify-content: center;
  border: 1.5px solid var(--border2);
  border-radius: 4px;
  background: var(--white);
  color: var(--ink3);
  cursor: pointer;
  transition: all .15s;
}
.grp-btn:hover { border-color: var(--fire); color: var(--fire-dark); }
.grp-btn.active {
  background: var(--fire);
  color: #fff;
  border-color: var(--fire);
}

/* ── MATCH CARD ── */
.matches-list {
  display: flex;
  flex-direction: column;
  gap: 8px;
}
.day-separator {
  display: flex;
  align-items: center;
  gap: 14px;
  margin: 22px 0 8px;
}
/* ── JUEGOS PASADOS ── */
.past-section-toggle {
  display: flex;
  align-items: center;
  gap: 10px;
  margin: 8px 0 6px;
  cursor: pointer;
  user-select: none;
}
.past-section-label {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 13px;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: var(--ink3);
  background: var(--bg3);
  padding: 4px 12px 4px 10px;
  border: 1.5px solid var(--border2);
  clip-path: polygon(0 0, 100% 0, 93% 100%, 0% 100%);
}
.past-section-toggle::after {
  content: '';
  flex: 1;
  height: 1px;
  background: var(--border2);
}
.past-toggle-btn {
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .08em;
  text-transform: uppercase;
  color: var(--ink3);
  background: var(--bg2);
  border: 1px solid var(--border2);
  border-radius: 2px;
  padding: 3px 8px;
  cursor: pointer;
  flex-shrink: 0;
}
.past-match-card {
  opacity: .55;
  filter: grayscale(30%);
  border-color: var(--border) !important;
}
.past-match-card .match-label-bar {
  background: var(--bg3) !important;
}
.past-match-card .score-box {
  background: var(--ink3) !important;
}
.past-match-card .score-sep {
  background: var(--ink3) !important;
}
.day-separator:first-child { margin-top: 4px; }
.day-separator-label {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 15px;
  letter-spacing: .1em;
  text-transform: uppercase;
  background: var(--fire);
  color: #fff;
  padding: 5px 16px 5px 12px;
  position: relative;
  clip-path: polygon(0 0, 100% 0, 92% 100%, 0% 100%);
  border: 2px solid var(--ink);
  transform: rotate(-2deg);
  box-shadow: 3px 3px 0 var(--ink);
}
.day-separator::after {
  content: '';
  flex: 1;
  height: 2px;
  background: repeating-linear-gradient(90deg, var(--border2) 0, var(--border2) 6px, transparent 6px, transparent 12px);
}
.match-card {
  background: var(--white);
  border: 1.5px solid var(--border);
  border-radius: 6px;
  overflow: hidden;
  transition: border-color .15s;
}
.match-card:hover { border-color: var(--border2); }
.match-card.live { border-color: var(--fire); }
.match-card.live .match-inner { background: #fffaf8; }

.match-label-bar {
  background: var(--bg3);
  padding: 4px 14px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.match-label {
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: var(--ink3);
}
.match-status {
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .08em;
  text-transform: uppercase;
  color: var(--ink3);
}
.match-status.live-status {
  color: var(--fire);
  font-weight: 700;
}
.match-status.done { color: var(--green); }

.match-inner {
  padding: 12px 14px;
  display: grid;
  grid-template-columns: 1fr auto 1fr;
  align-items: center;
  gap: 10px;
}
.team-home, .team-away {
  display: flex;
  align-items: center;
  gap: 10px;
}
.team-away {
  flex-direction: row-reverse;
  text-align: right;
}
.team-flag {
  font-size: 26px;
  line-height: 1;
  flex-shrink: 0;
}
.team-name {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 15px;
  letter-spacing: .02em;
  text-transform: uppercase;
  color: var(--ink);
  line-height: 1.1;
}
.team-abbr {
  font-family: var(--font-mono);
  font-size: 9px;
  color: var(--ink3);
  letter-spacing: .06em;
  text-transform: uppercase;
  margin-top: 1px;
}

.score-block {
  display: flex;
  align-items: center;
  gap: 0;
  flex-shrink: 0;
}
.score-box {
  background: var(--ink);
  color: #fff;
  font-family: var(--font-display);
  font-weight: 900;
  font-style: italic;
  font-size: 26px;
  letter-spacing: -.02em;
  width: 46px;
  height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
  line-height: 1;
}
.score-box.home {
  clip-path: polygon(0 0, 100% 0, 100% 100%, 8px 100%);
  padding-left: 4px;
}
.score-box.away {
  clip-path: polygon(0 0, calc(100% - 8px) 0, 100% 100%, 0 100%);
  padding-right: 4px;
}
.score-box.fire { background: var(--fire); }
.score-sep {
  background: var(--fire);
  color: #fff;
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 20px;
  width: 16px;
  height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
  transform: skewX(-12deg) scaleY(1.05);
  margin: 0 -2px;
  position: relative;
  z-index: 1;
}
.score-sep span { display: inline-block; transform: skewX(12deg); }
.score-pending {
  font-family: var(--font-mono);
  font-size: 11px;
  color: var(--ink3);
  letter-spacing: .04em;
  text-align: center;
  padding: 4px 8px;
  background: var(--bg2);
  border-radius: 4px;
  white-space: nowrap;
}

/* ── STANDINGS TABLE ── */
.groups-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 16px;
}
@media (max-width: 640px) {
  .groups-grid { grid-template-columns: 1fr; }
  .match-inner { grid-template-columns: 1fr auto 1fr; }
  .team-name { font-size: 12px; }
  .score-box { width: 36px; height: 36px; font-size: 20px; }
}
.group-card {
  background: var(--white);
  border: 1.5px solid var(--border);
  border-radius: 8px;
  overflow: hidden;
}
.group-card-header {
  background: var(--ink);
  padding: 10px 14px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.group-card-title {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 16px;
  letter-spacing: .08em;
  text-transform: uppercase;
  color: #fff;
}
.group-card-detail {
  font-family: var(--font-mono);
  font-size: 9px;
  color: rgba(255,255,255,.5);
  letter-spacing: .08em;
  text-transform: uppercase;
}
.standings-table {
  width: 100%;
  border-collapse: collapse;
  font-size: 12px;
}
.standings-table thead tr {
  background: var(--bg3);
}
.standings-table th {
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .08em;
  text-transform: uppercase;
  color: var(--ink3);
  padding: 6px 6px;
  text-align: center;
  font-weight: 400;
  border-bottom: 1px solid var(--border);
}
.standings-table th:first-child { text-align: left; padding-left: 12px; }
.standings-table td {
  padding: 8px 6px;
  text-align: center;
  border-bottom: 1px solid var(--border);
  color: var(--ink2);
  font-size: 12px;
}
.standings-table td:first-child { text-align: left; padding-left: 12px; }
.standings-table tr:last-child td { border-bottom: none; }
/* Columnas secundarias (PJ PG PE PP) */
.th-secondary, .td-secondary {
  color: var(--ink3) !important;
  font-size: 11px !important;
}
/* Columnas menores (GF GC DG) — visibles pero discretas */
.th-minor, .td-minor {
  color: var(--border2) !important;
  font-size: 10px !important;
}
@media (max-width: 520px) {
  .th-minor, .td-minor { display: none; }
}

.team-cell {
  display: flex;
  align-items: center;
  gap: 8px;
}
.team-cell-flag { font-size: 18px; line-height: 1; }
.team-cell-name {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 13px;
  text-transform: uppercase;
  letter-spacing: .02em;
  color: var(--ink);
  white-space: nowrap;
}
.pts-cell {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 16px;
  color: var(--ink);
}
.pos-indicator {
  display: inline-block;
  width: 4px;
  height: 28px;
  border-radius: 2px;
  margin-right: 6px;
  vertical-align: middle;
  flex-shrink: 0;
}
.pos-q2 { background: var(--green); }
.pos-q3 { background: var(--gold); }
.pos-out { background: transparent; border: 1px solid var(--border2); }

.pos-row { display: flex; align-items: center; gap: 0; }
.pos-num {
  font-family: var(--font-mono);
  font-size: 10px;
  color: var(--ink3);
  width: 16px;
  flex-shrink: 0;
}

/* ── STATS VIEW ── */
.stats-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
}
@media (max-width: 640px) { .stats-grid { grid-template-columns: 1fr; } }

.stats-card {
  background: var(--white);
  border: 1.5px solid var(--border);
  border-radius: 8px;
  overflow: hidden;
}
.stats-card-header {
  padding: 12px 14px;
  border-bottom: 1.5px solid var(--border);
  display: flex;
  align-items: center;
  gap: 10px;
}
.stats-card-icon {
  width: 32px;
  height: 32px;
  border-radius: 4px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 16px;
  flex-shrink: 0;
}
.icon-fire { background: var(--fire-light); }
.icon-yellow { background: var(--gold-light); }
.icon-red { background: var(--red-light); }
.stats-card-title {
  font-family: var(--font-display);
  font-weight: 800;
  font-size: 14px;
  text-transform: uppercase;
  letter-spacing: .06em;
  color: var(--ink);
}
.stats-card-body { padding: 4px 0; }

.scorer-row {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 9px 14px;
  border-bottom: 1px solid var(--border);
}
.scorer-row:last-child { border-bottom: none; }

/* ── STATS: fade-in al expandir + botón mejorado ── */
@keyframes statsFadeIn {
  from { opacity: 0; transform: translateY(-4px); }
  to   { opacity: 1; transform: translateY(0); }
}
.stats-fade-in {
  animation: statsFadeIn .28s ease-out both;
}
.stats-toggle-btn {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 12px;
  letter-spacing: .06em;
  text-transform: uppercase;
  background: none;
  border: 1.5px solid var(--border2);
  color: var(--ink2);
  padding: 7px 14px;
  border-radius: 3px;
  cursor: pointer;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 6px;
  transition: background .15s, border-color .15s;
}
.stats-toggle-btn:hover {
  background: var(--bg3);
  border-color: var(--fire);
  color: var(--ink);
}
.stats-more-badge {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--fire);
  color: #fff;
  font-family: var(--font-mono);
  font-size: 10px;
  font-weight: 700;
  letter-spacing: 0;
  padding: 1px 6px;
  border-radius: 3px;
  min-width: 20px;
}
.scorer-rank {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 20px;
  color: var(--bg3);
  width: 26px;
  flex-shrink: 0;
  text-align: center;
  line-height: 1;
}
.scorer-rank.top { color: var(--fire); }
.scorer-info { flex: 1; min-width: 0; }
.scorer-name {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 14px;
  text-transform: uppercase;
  color: var(--ink);
  letter-spacing: .02em;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
.scorer-team {
  font-family: var(--font-mono);
  font-size: 9px;
  color: var(--ink3);
  letter-spacing: .06em;
  text-transform: uppercase;
}
.scorer-goals {
  display: flex;
  align-items: center;
  gap: 4px;
  flex-shrink: 0;
}
.goal-pip {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: var(--fire);
}
.goals-num {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 22px;
  color: var(--ink);
  line-height: 1;
}
.goals-label {
  font-family: var(--font-mono);
  font-size: 9px;
  color: var(--ink3);
  text-transform: uppercase;
  letter-spacing: .06em;
  margin-top: 2px;
}

.card-row {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 9px 14px;
  border-bottom: 1px solid var(--border);
}
.card-row:last-child { border-bottom: none; }
.tarjeta {
  width: 18px;
  height: 24px;
  border-radius: 2px;
  flex-shrink: 0;
  display: inline-block;
}
.tarjeta-amarilla { background: var(--yellow); box-shadow: 1px 1px 0 var(--yellow-dark); }
.tarjeta-roja { background: var(--red-card); box-shadow: 1px 1px 0 #a01010; }
.card-info { flex: 1; }
.card-player {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 13px;
  text-transform: uppercase;
  letter-spacing: .02em;
  color: var(--ink);
}
.card-team {
  font-family: var(--font-mono);
  font-size: 9px;
  color: var(--ink3);
  letter-spacing: .06em;
  text-transform: uppercase;
}
.card-min {
  font-family: var(--font-mono);
  font-size: 10px;
  color: var(--ink3);
  flex-shrink: 0;
}

/* ── NOTICIAS 123KLAN STYLE ── */
.noticias-list {
  display: flex;
  flex-direction: column;
  gap: 16px;
}
.noticia-card {
  background: var(--white);
  border: 1.5px solid var(--border);
  border-radius: 8px;
  overflow: hidden;
  cursor: pointer;
  transition: border-color .15s, transform .1s;
}
.noticia-card:hover { border-color: var(--fire); transform: translateY(-1px); }
.noticia-accent {
  height: 6px;
  background: var(--fire);
}
.noticia-accent.gold { background: var(--gold); }
.noticia-accent.lime { background: var(--lime); }
.noticia-accent.blue { background: var(--blue); }

.noticia-body { padding: 16px 18px; }
.noticia-kicker {
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .14em;
  text-transform: uppercase;
  color: var(--fire);
  margin-bottom: 6px;
}
.noticia-kicker.gold { color: var(--gold-dark); }
.noticia-kicker.lime { color: #4A7200; }
.noticia-kicker.blue { color: var(--blue); }

.noticia-title {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 22px;
  line-height: 1.08;
  letter-spacing: -.01em;
  color: var(--ink);
  text-transform: uppercase;
  margin-bottom: 10px;
}
.noticia-text {
  font-family: var(--font-body);
  font-size: 13px;
  line-height: 1.65;
  color: var(--ink2);
  margin-bottom: 14px;
}
.noticia-footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 8px;
}
.noticia-tag {
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .1em;
  text-transform: uppercase;
  padding: 3px 8px;
  border-radius: 2px;
  border: 1px solid var(--border2);
  color: var(--ink3);
}
.noticia-jugador {
  display: flex;
  align-items: center;
  gap: 8px;
}
.jugador-flag { font-size: 16px; }
.jugador-name {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 13px;
  text-transform: uppercase;
  letter-spacing: .04em;
  color: var(--ink);
}
.jugador-label {
  font-family: var(--font-mono);
  font-size: 9px;
  color: var(--ink3);
  text-transform: uppercase;
}

/* ── GDL VIEW ── */
.gdl-hero {
  background: var(--ink);
  border-radius: 10px;
  padding: 28px 24px;
  margin-bottom: 20px;
  position: relative;
  overflow: hidden;
}
.gdl-hero::before {
  content: 'GDL';
  position: absolute;
  right: -20px;
  top: -20px;
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 140px;
  color: rgba(255,255,255,.04);
  letter-spacing: -.04em;
  line-height: 1;
  pointer-events: none;
  user-select: none;
}
.gdl-hero-kicker {
  font-family: var(--font-mono);
  font-size: 10px;
  letter-spacing: .14em;
  text-transform: uppercase;
  color: var(--fire);
  margin-bottom: 8px;
}
.gdl-hero-title {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 36px;
  line-height: 1;
  letter-spacing: -.02em;
  text-transform: uppercase;
  color: #fff;
  margin-bottom: 12px;
}
.gdl-hero-title span { color: var(--fire); }
.gdl-hero-text {
  font-size: 13px;
  line-height: 1.6;
  color: rgba(255,255,255,.65);
  max-width: 580px;
  margin-bottom: 20px;
}
.gdl-stats-row {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
}
.gdl-stat {
  display: flex;
  flex-direction: column;
}
.gdl-stat-num {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 32px;
  color: var(--fire);
  line-height: 1;
}
.gdl-stat-label {
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: rgba(255,255,255,.45);
  margin-top: 2px;
}
.gdl-matches-list { display: flex; flex-direction: column; gap: 8px; }

/* ── FOOTER ── */
.site-footer {
  background: var(--ink);
  padding: 20px;
  margin-top: 40px;
  border-top: 3px solid var(--fire);
}
.footer-inner {
  max-width: 1100px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 12px;
}
.footer-copy {
  font-family: var(--font-mono);
  font-size: 10px;
  color: rgba(255,255,255,.35);
  letter-spacing: .08em;
}
.footer-tagline {
  font-family: var(--font-display);
  font-weight: 700;
  font-size: 12px;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: var(--fire);
}

.match-card.mexico-venue { border-color: #006847; }
.match-card.mexico-venue .match-label-bar { background: #e8f5ee; }
.match-card.mexico-venue .match-label { color: #006847; font-weight: 700; }
.mexico-badge {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .08em;
  text-transform: uppercase;
  background: #006847;
  color: #fff;
  padding: 2px 7px;
  border-radius: 2px;
  margin-left: 6px;
}

.full-width { grid-column: 1 / -1; }

/* ── SEDES GRID ── */
.sedes-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 14px;
  margin-bottom: 4px;
}
@media (max-width: 760px) {
  .sedes-grid { grid-template-columns: 1fr; }
}

/* acento izquierdo por ciudad */
.sede-hero-gdl { border-left: 4px solid var(--fire); }
.sede-hero-cdmx { border-left: 4px solid #006847; }
.sede-hero-mty  { border-left: 4px solid var(--gold); }

.sede-hero-cdmx .gdl-hero-title span { color: #4CAF50; }
.sede-hero-mty  .gdl-hero-title span { color: var(--gold); }

/* ── EVENTO CARDS ── */
.evento-card {
  background: var(--white);
  border: 1.5px solid var(--border);
  border-radius: 8px;
  overflow: hidden;
  display: grid;
  grid-template-columns: 80px 1fr;
}
.evento-lateral {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 16px 8px;
  gap: 6px;
}
.evento-emoji { font-size: 28px; line-height: 1; }
.evento-acceso {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 9px;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: #fff;
  padding: 3px 7px;
  border-radius: 2px;
  white-space: nowrap;
  transform: rotate(-90deg);
}
.evento-body { padding: 14px 16px; border-left: 1.5px solid var(--border); }
.evento-cat {
  font-family: var(--font-mono);
  font-size: 9px;
  letter-spacing: .12em;
  text-transform: uppercase;
  margin-bottom: 4px;
}
.evento-nombre {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 18px;
  text-transform: uppercase;
  letter-spacing: .02em;
  color: var(--ink);
  line-height: 1.1;
  margin-bottom: 8px;
}
.evento-meta {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-bottom: 6px;
}
.evento-meta-item {
  display: flex;
  align-items: center;
  gap: 4px;
  font-family: var(--font-mono);
  font-size: 10px;
  color: var(--ink2);
  letter-spacing: .04em;
}
.evento-nota {
  font-family: var(--font-body);
  font-size: 12px;
  color: var(--ink3);
  line-height: 1.4;
  margin-top: 6px;
  padding-top: 6px;
  border-top: 0.5px solid var(--border);
}

/* ── FOOTER DECO SVG ── */
.footer-deco {
  width: 100%;
  margin-bottom: 8px;
}
.footer-block {
  background: var(--fire);
  padding: 22px 20px;
  text-align: center;
  overflow: hidden;
}
.footer-block-text {
  font-family: var(--font-display);
  font-weight: 900;
  font-style: italic;
  font-size: clamp(32px, 9vw, 88px);
  letter-spacing: .06em;
  color: var(--ink);
  line-height: 1;
  display: inline-block;
  white-space: nowrap;
}

/* ── 123KLAN KNOCKOUT BRACKET STYLES ── */
.bracket-wrapper {
  width: 100%;
  overflow-x: auto;
  padding: 10px 0 30px;
  scrollbar-width: thin;
}
.bracket-wrapper::-webkit-scrollbar {
  height: 6px;
}
.bracket-wrapper::-webkit-scrollbar-thumb {
  background: var(--ink3);
  border-radius: 3px;
}
.bracket-container {
  display: grid;
  grid-template-columns: repeat(5, 250px);
  gap: 24px;
  min-width: 1350px;
  padding: 10px;
}
.bracket-column {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  position: relative;
}
.bracket-column-title {
  font-family: var(--font-display);
  font-weight: 900;
  font-size: 15px;
  letter-spacing: .08em;
  text-transform: uppercase;
  color: var(--ink);
  background: var(--bg2);
  padding: 6px 12px;
  border: 1.5px solid var(--ink);
  margin-bottom: 16px;
  text-align: center;
  box-shadow: 2px 2px 0 var(--ink);
  transform: rotate(-1.5deg);
}
.bracket-match-node {
  background: var(--white);
  border: 2px solid var(--ink);
  border-radius: 4px;
  padding: 8px 10px;
  position: relative;
  box-shadow: 3px 3px 0 var(--ink);
  margin: 14px 0;
  transition: all .2s ease-out;
}
.bracket-match-node:hover {
  transform: scale(1.02) rotate(0.5deg);
  border-color: var(--fire);
  box-shadow: 4px 4px 0 var(--fire);
}
.bracket-node-header {
  display: flex;
  justify-content: space-between;
  border-bottom: 1px dashed var(--border2);
  padding-bottom: 4px;
  margin-bottom: 6px;
}
.bracket-node-id {
  font-family: var(--font-mono);
  font-size: 8px;
  background: var(--ink);
  color: #fff;
  padding: 1px 5px;
  font-weight: 700;
  border-radius: 1px;
}
.bracket-node-meta {
  font-family: var(--font-mono);
  font-size: 8px;
  color: var(--ink3);
  text-transform: uppercase;
}
.bracket-node-team {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-family: var(--font-display);
  font-size: 14px;
  font-weight: 700;
  color: var(--ink2);
  padding: 2px 0;
  text-transform: uppercase;
}
.bracket-node-team.winner {
  color: var(--ink);
  font-weight: 900;
}
.bracket-node-score {
  font-family: var(--font-mono);
  font-weight: 700;
  font-size: 13px;
  background: var(--bg2);
  padding: 1px 6px;
  border-radius: 2px;
  min-width: 22px;
  text-align: center;
}
.bracket-node-team.winner .bracket-node-score {
  background: var(--fire);
  color: #fff;
}
.bracket-match-node.unresolved {
  background: rgba(26,25,21,0.03);
  border-style: dashed;
  box-shadow: none;
}
.bracket-match-node.unresolved .bracket-node-team {
  color: var(--ink3);
  font-weight: 400;
  font-style: italic;
}

/* ── ANIMACIÓN TRANSICIÓN BRACKET (ESTILO FIFAis) ── */
@keyframes bracketFadeSlide {
  from { opacity: 0; transform: translateY(12px); }
  to { opacity: 1; transform: translateY(0); }
}
.bracket-match-node {
  animation: bracketFadeSlide 0.35s cubic-bezier(0.25, 1, 0.5, 1) both;
}
.bracket-column:nth-child(1) .bracket-match-node { animation-delay: 0.05s; }
.bracket-column:nth-child(2) .bracket-match-node { animation-delay: 0.12s; }
.bracket-column:nth-child(3) .bracket-match-node { animation-delay: 0.18s; }
.bracket-column:nth-child(4) .bracket-match-node { animation-delay: 0.22s; }
.bracket-column:nth-child(5) .bracket-match-node { animation-delay: 0.26s; }
/* ── INTERACTIVE CANVAS BRACKET (123KLAN GESTURES) ── */
.canvas-frame-container {
  width: 100%;
  height: 72vh;
  overflow: auto;
  border: 4px solid var(--ink);
  background: var(--bg2);
  box-shadow: 6px 6px 0 var(--ink);
  position: relative;
  cursor: grab;
  border-radius: 4px;
  touch-action: none;
}
.canvas-frame-container:active { cursor: grabbing; }

.viewport-scaler-area {
  padding: 40px;
  transform-origin: top left;
  display: grid;
  grid-template-columns: repeat(6, 265px);
  gap: 35px;
  width: max-content;
  min-height: 100%;
}
.bracket-column {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  position: relative;
}
.bracket-column-title {
  font-weight: 900;
  font-size: 16px;
  text-transform: uppercase;
  color: #fff;
  background: var(--ink);
  padding: 8px;
  border: 2px solid var(--fire);
  text-align: center;
  transform: rotate(-1.5deg);
  box-shadow: 3px 3px 0 var(--fire);
  margin-bottom: 20px;
}
.bracket-match-node {
  background: var(--white);
  border: 2.5px solid var(--ink);
  border-radius: 4px;
  padding: 8px 10px;
  box-shadow: 4px 4px 0 var(--ink);
  margin: 14px 0;
}
.node-info-row {
  display: flex;
  justify-content: space-between;
  font-family: var(--font-mono);
  font-size: 8px;
  font-weight: 700;
  color: var(--ink2);
  border-bottom: 1px dashed var(--bg3);
  padding-bottom: 4px;
  margin-bottom: 6px;
  text-transform: uppercase;
}
.node-match-id { background: var(--ink); color: #fff; padding: 1px 5px; }

.team-selectable-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 15px;
  font-weight: 800;
  padding: 7px 8px;
  margin: 4px 0;
  border: 1.5px solid transparent;
  border-radius: 3px;
  cursor: pointer;
  transition: all 0.1s ease;
  text-transform: uppercase;
}
.team-selectable-row:hover { background: var(--fire-light); border-color: var(--fire); }
.team-selectable-row.selected-winner { background: var(--ink); color: #fff; border-color: var(--ink); }
.score-box-display {
  font-family: var(--font-mono);
  background: var(--bg3);
  padding: 2px 6px;
  font-size: 11px;
  border-radius: 2px;
  color: var(--ink);
  font-weight: 900;
}
.team-selectable-row.selected-winner .score-box-display { background: var(--fire); color: #fff; }
.fav-badge {
  font-family: var(--font-mono);
  font-size: 9px;
  color: var(--fire);
  font-weight: bold;
  background: var(--fire-light);
  padding: 1px 5px;
  border-radius: 2px;
}
.team-selectable-row.selected-winner .fav-badge { color: var(--white); background: rgba(255,255,255,0.2); }
.unresolved-node { opacity: 0.55; border-style: dashed; box-shadow: none; }
.unresolved-node .team-selectable-row { color: var(--ink3); font-weight: 500; }

/* PANEL CONTROLES SLIDER */
.bracket-controls-panel {
  display: grid;
  grid-template-columns: 1fr auto;
  gap: 15px;
  align-items: center;
  background: var(--bg3);
  padding: 12px;
  border: 3px solid var(--ink);
  box-shadow: 4px 4px 0 var(--ink);
  margin-bottom: 15px;
}
.zoom-slider-container { display: flex; align-items: center; gap: 10px; }
.zoom-slider-container label { font-weight: 900; text-transform: uppercase; font-size: 13px; }
.123klan-slider { -webkit-appearance: none; width: 100%; height: 10px; background: var(--white); border: 2px solid var(--ink); outline: none; }
.123klan-slider::-webkit-slider-thumb { -webkit-appearance: none; width: 20px; height: 20px; background: var(--fire); border: 2px solid var(--ink); cursor: pointer; }
.bracket-ctrl-btn { font-family: var(--font-display); font-weight: 900; font-size: 13px; text-transform: uppercase; background: var(--fire-dark); color: #fff; border: 2px solid var(--ink); padding: 8px 16px; cursor: pointer; box-shadow: 2px 2px 0 var(--ink); }
</style>
</head>
<body>

<header class="site-header">
  <div class="header-inner">
    <div class="logo">
      <span class="logo-badge">Zona de Gol</span>
      <span class="logo-text"><span>¿</span>QUIÉN JUEGA HOY<span>?</span></span>
    </div>
    <div class="live-dot">En vivo</div>
  </div>
</header>

<nav class="main-nav">
  <div class="nav-inner">
    <button class="nav-btn active" onclick="showView('resultados', event)">Resultados</button>
    <button class="nav-btn" onclick="showView('posiciones', event)">Posiciones</button>
    <button class="nav-btn" onclick="showView('bracket', event)">Quiniela</button> <button class="nav-btn" onclick="showView('estadisticas', event)">Stats</button>
    <button class="nav-btn" onclick="showView('estadisticas', event)">Stats</button>
    <button class="nav-btn" onclick="showView('noticias', event)">Noticias</button>
    <button class="nav-btn" onclick="showView('gdl', event)">Guadalajara</button>
  </div>
</nav>

<main class="page">

<div id="view-resultados" class="view active">
  <div class="section-head">
    <div>
      <div class="section-title">Resultados y <span>Próximos Juegos</span></div>
      <div class="section-sub" id="results-subtitle">72 partidos fase de grupos · 48 selecciones · 3 países sede</div>
    </div>
  </div>

  <div class="phase-pills" id="phase-pills"></div>
  <div id="group-selector-wrap">
    <div class="group-selector" id="group-selector"></div>
  </div>
  <div class="matches-list" id="matches-container"></div>
</div>

<div id="view-posiciones" class="view">
  <div class="section-head">
    <div>
      <div class="section-title">Fase de <span>Grupos</span></div>
      <div class="section-sub">Tabla de posiciones · Actualizado en vivo</div>
    </div>
  </div>
  <div class="groups-grid" id="standings-container"></div>

  <div style="margin-top: 20px; display: flex; gap: 16px; flex-wrap: wrap;">
    <div style="display:flex;align-items:center;gap:6px;">
      <span style="display:inline-block;width:12px;height:12px;border-radius:2px;background:var(--green);"></span>
      <span style="font-family:var(--font-mono);font-size:10px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Clasifica (Octavos)</span>
    </div>
    <div style="display:flex;align-items:center;gap:6px;">
      <span style="display:inline-block;width:12px;height:12px;border-radius:2px;background:var(--gold);"></span>
      <span style="font-family:var(--font-mono);font-size:10px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Mejor 3ro (posible clasificación)</span>
    </div>
    <div style="display:flex;align-items:center;gap:6px;">
      <span style="display:inline-block;width:12px;height:12px;border-radius:2px;border:1px solid var(--border2);background:transparent;"></span>
      <span style="font-family:var(--font-mono);font-size:10px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Eliminado</span>
    </div>
  </div>
</div>

<div id="view-bracket" class="view">
  <div class="section-head">
    <div>
      <div class="section-title">¡Arma tu <span>quiniela!</span></div>
      <div class="section-sub">El mundial es ahora · Desplaza y controla el zoom con el deslizador</div>
    </div>
  </div>

  <div class="bracket-controls-panel">
    <div class="zoom-slider-container">
      <label>Zoom:</label>
      <input type="range" class="123klan-slider" id="scale-slider" min="0.35" max="1.1" step="0.05" value="0.65" oninput="manualZoomAdjust(this.value)">
    </div>
    <button class="bracket-ctrl-btn" onclick="resetUserQuiniela()">Reiniciar 🔄</button>
  </div>

  <div class="canvas-frame-container" id="canvas-container-scroll">
    <div class="viewport-scaler-area" id="bracket-render-container">
      </div>
  </div>
</div>

<div id="view-estadisticas" class="view">
  <div class="section-head">
    <div>
      <div class="section-title">Estadística <span>Mundialista</span></div>
      <div class="section-sub">Goleadores · Tarjetas · Números que importan</div>
    </div>
  </div>

  <div class="stats-grid">
    <div class="stats-card">
      <div class="stats-card-header">
        <div class="stats-card-icon icon-fire">⚽</div>
        <div>
          <div class="stats-card-title">Top Goleadores</div>
          <div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Fase de grupos</div>
        </div>
      </div>
      <div class="stats-card-body" id="scorers-list"></div>
    </div>

    <div class="stats-card">
      <div class="stats-card-header">
        <div class="stats-card-icon icon-yellow">
          <span class="tarjeta tarjeta-amarilla"></span>
        </div>
        <div>
          <div class="stats-card-title">Tarjetas Amarillas</div>
          <div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Por selección</div>
        </div>
      </div>
      <div class="stats-card-body" id="yellow-list"></div>
    </div>

    <div class="stats-card">
      <div class="stats-card-header">
        <div class="stats-card-icon icon-red">
          <span class="tarjeta tarjeta-roja"></span>
        </div>
        <div>
          <div class="stats-card-title">Tarjetas Rojas</div>
          <div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Expulsados del torneo</div>
        </div>
      </div>
      <div class="stats-card-body" id="red-list"></div>
    </div>

    <div class="stats-card">
      <div class="stats-card-header">
        <div class="stats-card-icon" style="background:var(--blue-light);font-size:16px;">📊</div>
        <div>
          <div class="stats-card-title">Números Locos</div>
          <div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Datos que no esperabas</div>
        </div>
      </div>
      <div class="stats-card-body" id="crazy-numbers"></div>
    </div>
  </div>
</div>

<div id="view-noticias" class="view">
  <div class="section-head">
    <div>
      <div class="section-title">La <span>Crónica</span></div>
      <div class="section-sub">Periodismo deportivo · Al estilo de la calle</div>
    </div>
  </div>
  <div class="noticias-list" id="noticias-container"></div>
</div>

<div id="view-gdl" class="view">

  <div class="section-head">
    <div>
      <div class="section-title">México <span>2026</span></div>
      <div class="section-sub">3 ciudades sede · 3 estadios · El Mundial en casa</div>
    </div>
  </div>

  <div class="sedes-grid">

    <div class="gdl-hero sede-hero-gdl">
      <div class="gdl-hero-kicker">Estadio Guadalajara · 3 veces mundialista</div>
      <div class="gdl-hero-title">Guadalajara <span>2026</span></div>
      <div class="gdl-hero-text">La ciudad del mariachi, el tequila y el fútbol tapatío. 1970, 1986 y ahora 2026: el Estadio Guadalajara escribe el tercer capítulo de la historia.</div>
      <div class="gdl-stats-row">
        <div class="gdl-stat"><span class="gdl-stat-num">4</span><span class="gdl-stat-label">Partidos</span></div>
        <div class="gdl-stat"><span class="gdl-stat-num">3×</span><span class="gdl-stat-label">Mundialista</span></div>
        <div class="gdl-stat"><span class="gdl-stat-num">49k</span><span class="gdl-stat-label">Capacidad</span></div>
      </div>
    </div>

    <div class="gdl-hero sede-hero-cdmx">
      <div class="gdl-hero-kicker">Estadio Ciudad de México · Leyenda viva</div>
      <div class="gdl-hero-title">Ciudad de <span>México</span></div>
      <div class="gdl-hero-text">El Estadio Azteca. La casa del Gol del Siglo. El recinto más icónico del fútbol mundial vuelve a ser el escenario más grande del torneo.</div>
      <div class="gdl-stats-row">
        <div class="gdl-stat"><span class="gdl-stat-num">5</span><span class="gdl-stat-label">Partidos</span></div>
        <div class="gdl-stat"><span class="gdl-stat-num">3×</span><span class="gdl-stat-label">Mundialista</span></div>
        <div class="gdl-stat"><span class="gdl-stat-num">87k</span><span class="gdl-stat-label">Capacidad</span></div>
      </div>
    </div>

    <div class="gdl-hero sede-hero-mty">
      <div class="gdl-hero-kicker">Estadio Monterrey · La sultana del norte</div>
      <div class="gdl-hero-title">Monterrey <span>2026</span></div>
      <div class="gdl-hero-text">La ciudad más industrial y cosmopolita del norte de México entra al mapa mundial con el Estadio BBVA como escenario de lujo para el torneo.</div>
      <div class="gdl-stats-row">
        <div class="gdl-stat"><span class="gdl-stat-num">4</span><span class="gdl-stat-label">Partidos</span></div>
        <div class="gdl-stat"><span class="gdl-stat-num">1×</span><span class="gdl-stat-label">Mundialista</span></div>
        <div class="gdl-stat"><span class="gdl-stat-num">53k</span><span class="gdl-stat-label">Capacidad</span></div>
      </div>
    </div>

  </div>

  <div class="section-head mt-20">
    <div class="section-title">Partidos en <span>México</span></div>
  </div>
  <div class="gdl-matches-list" id="gdl-matches"></div>

  <div class="section-head mt-20">
    <div class="section-title">Eventos en <span>Guadalajara</span></div>
    <div class="section-sub">Conciertos · Activaciones · Entretenimiento · Todos gratuitos</div>
  </div>
  <div id="eventos-container" style="display:flex;flex-direction:column;gap:12px;"></div>

  <div class="section-head mt-20">
    <div class="section-title">Datos <span>Curiosos</span></div>
    <div class="section-sub">Lo que no sabías de GDL y el Mundial</div>
  </div>
  <div id="curiosidades-container" style="display:flex;flex-direction:column;gap:12px;"></div>
</div>

</main>

<footer class="site-footer">
  <div class="footer-deco" aria-hidden="true">
    <div class="footer-block">
      <span class="footer-block-text">PASIÓN MUNDIAL</span>
    </div>
  </div>
  <div class="footer-inner" style="flex-direction:column; align-items:center; text-align:center; gap:6px;">
    <span class="footer-tagline">El corazón del juego</span>
    <span class="footer-copy">© 2026 · Datos: worldcup2026 API · NFOKU MKT</span>
  </div>
</footer>

<script>
// ══════════════════════════════════════════════════════════
// DATA LAYER — edita aquí para actualizar resultados
// ══════════════════════════════════════════════════════════
const MEXICO_VENUES = ['Estadio Guadalajara', 'Estadio Ciudad de México', 'Estadio Monterrey'];

const MONTH_MAP = { Jun:6, Jul:7 };
const DAY_NAMES = ['DOM','LUN','MAR','MIÉ','JUE','VIE','SÁB'];
function getDayName(dateStr) {
  const parts = dateStr.split(' ');
  const day = parseInt(parts[0], 10);
  const month = (MONTH_MAP[parts[1]] || 6) - 1;
  const year = 2026;
  const d = new Date(year, month, day);
  return DAY_NAMES[d.getDay()];
}
function matchSortKey(m) {
  const parts = m.date.split(' ');
  const day = parseInt(parts[0], 10) || 0;
  const month = MONTH_MAP[parts[1]] || 6;
  const timeStr = (m.time || '00:00').replace(' hrs','').split(':');
  const hh = parseInt(timeStr[0], 10) || 0;
  const mm = parseInt(timeStr[1], 10) || 0;
  return month * 100000 + day * 1000 + hh * 10 + (mm >= 30 ? 5 : 0);
}
function dateOnlyKey(dateStr) {
  const parts = dateStr.split(' ');
  const day = parseInt(parts[0], 10) || 0;
  const month = MONTH_MAP[parts[1]] || 6;
  return month * 100 + day;
}

const DATA = {
  currentWeek: { startDate: '29 Jun', endDate: '5 Jul', label: 'Semana del 29 de Jun al 5 de jul' },

  phases: [
    { id: 'semana',        label: 'Esta Semana' },
    { id: 'grupos',        label: 'Fase de Grupos' },
    { id: 'dieciseisavos', label: 'Dieciseisavos' },
    { id: 'octavos',       label: 'Octavos de Final' },
    { id: 'cuartos',       label: 'Cuartos de Final' },
    { id: 'semis',         label: 'Semifinales' },
    { id: 'final',         label: 'Final' },
  ],

  groups: ['A','B','C','D','E','F','G','H','I','J','K','L'],

  matches: [
    // ── GRUPO A: México · Sudáfrica · Rep. de Corea · Rep. Checa
    { id:1,  phase:'grupos', group:'A', home:'México',        homeFlag:'🇲🇽', away:'Sudáfrica',     awayFlag:'🇿🇦', homeScore:2, awayScore:0, date:'11 Jun', time:'13:00', venue:'Estadio Ciudad de México', status:'done' },
    { id:2,  phase:'grupos', group:'A', home:'Rep. de Corea', homeFlag:'🇰🇷', away:'Rep. Checa',    awayFlag:'🇨🇿', homeScore:2, awayScore:1, date:'11 Jun', time:'20:00', venue:'Estadio Guadalajara',      status:'done' },
    { id:3,  phase:'grupos', group:'A', home:'Rep. Checa',    homeFlag:'🇨🇿', away:'Sudáfrica',     awayFlag:'🇿🇦', homeScore:1, awayScore:1, date:'18 Jun', time:'10:00', venue:'Estadio Atlanta',          status:'done' },
    { id:4,  phase:'grupos', group:'A', home:'México',        homeFlag:'🇲🇽', away:'Rep. de Corea', awayFlag:'🇰🇷', homeScore:1, awayScore:0, date:'18 Jun', time:'19:00', venue:'Estadio Guadalajara',      status:'done' },
    { id:5,  phase:'grupos', group:'A', home:'Rep. Checa',    homeFlag:'🇨🇿', away:'México',        awayFlag:'🇲🇽', homeScore:0, awayScore:3, date:'24 Jun', time:'19:00', venue:'Estadio Ciudad de México', status:'done' },
    { id:6,  phase:'grupos', group:'A', home:'Sudáfrica',     homeFlag:'🇿🇦', away:'Rep. de Corea', awayFlag:'🇰🇷', homeScore:1, awayScore:0, date:'24 Jun', time:'19:00', venue:'Estadio Monterrey',        status:'done' },
    // ── GRUPO B: Canadá · Bosnia y Herzegovina · Catar · Suiza
    { id:7,  phase:'grupos', group:'B', home:'Canadá',               homeFlag:'🇨🇦', away:'Bosnia y Herzegovina', awayFlag:'🇧🇦', homeScore:1, awayScore:1, date:'12 Jun', time:'13:00', venue:'Estadio Toronto',               status:'done' },
    { id:8,  phase:'grupos', group:'B', home:'Catar',                homeFlag:'🇶🇦', away:'Suiza',                awayFlag:'🇨🇭', homeScore:1, awayScore:1, date:'13 Jun', time:'13:00', venue:'Estadio Bahía de San Francisco', status:'done' },
    { id:9,  phase:'grupos', group:'B', home:'Suiza',                homeFlag:'🇨🇭', away:'Bosnia y Herzegovina', awayFlag:'🇧🇦', homeScore:4, awayScore:1, date:'18 Jun', time:'13:00', venue:'Estadio Los Ángeles',            status:'done' },
    { id:10, phase:'grupos', group:'B', home:'Canadá',               homeFlag:'🇨🇦', away:'Catar',                awayFlag:'🇶🇦', homeScore:6, awayScore:0, date:'18 Jun', time:'16:00', venue:'Estadio BC Place Vancouver',    status:'done' },
    { id:11, phase:'grupos', group:'B', home:'Suiza',                homeFlag:'🇨🇭', away:'Canadá',               awayFlag:'🇨🇦', homeScore:2, awayScore:0, date:'24 Jun', time:'13:00', venue:'Estadio BC Place Vancouver',    status:'done' },
    { id:12, phase:'grupos', group:'B', home:'Bosnia y Herzegovina', homeFlag:'🇧🇦', away:'Catar',                awayFlag:'🇶🇦', homeScore:2, awayScore:1, date:'24 Jun', time:'13:00', venue:'Estadio Seattle',               status:'done' },
    // ── GRUPO C: Brasil · Marruecos · Haití · Escocia
    { id:13, phase:'grupos', group:'C', home:'Brasil',    homeFlag:'🇧🇷', away:'Marruecos', awayFlag:'🇲🇦', homeScore:1, awayScore:1, date:'13 Jun', time:'16:00', venue:'Estadio Nueva York',            status:'done' },
    { id:14, phase:'grupos', group:'C', home:'Haití',     homeFlag:'🇭🇹', away:'Escocia',   awayFlag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', homeScore:0, awayScore:1, date:'13 Jun', time:'19:00', venue:'Estadio Boston',                status:'done' },
    { id:15, phase:'grupos', group:'C', home:'Escocia',   homeFlag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', away:'Marruecos', awayFlag:'🇲🇦', homeScore:0, awayScore:1, date:'19 Jun', time:'16:00', venue:'Estadio Boston',                status:'done' },
    { id:16, phase:'grupos', group:'C', home:'Brasil',    homeFlag:'🇧🇷', away:'Haití',     awayFlag:'🇭🇹', homeScore:3, awayScore:0, date:'19 Jun', time:'18:30', venue:'Estadio Filadelfia',            status:'done' },
    { id:17, phase:'grupos', group:'C', home:'Marruecos', homeFlag:'🇲🇦', away:'Haití',     awayFlag:'🇭🇹', homeScore:4, awayScore:2, date:'24 Jun', time:'16:00', venue:'Estadio Atlanta',               status:'done' },
    { id:18, phase:'grupos', group:'C', home:'Escocia',   homeFlag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', away:'Brasil',    awayFlag:'🇧🇷', homeScore:0, awayScore:3, date:'24 Jun', time:'16:00', venue:'Estadio Miami',                 status:'done' },
    // ── GRUPO D: Estados Unidos · Paraguay · Australia · Turquía
    { id:19, phase:'grupos', group:'D', home:'Estados Unidos', homeFlag:'🇺🇸', away:'Paraguay',       awayFlag:'🇵🇾', homeScore:4, awayScore:1, date:'12 Jun', time:'19:00', venue:'Estadio Los Ángeles',            status:'done' },
    { id:20, phase:'grupos', group:'D', home:'Australia',      homeFlag:'🇦🇺', away:'Turquía',        awayFlag:'🇹🇷', homeScore:2, awayScore:0, date:'13 Jun', time:'22:00', venue:'Estadio BC Place Vancouver',    status:'done' },
    { id:21, phase:'grupos', group:'D', home:'Estados Unidos', homeFlag:'🇺🇸', away:'Australia',      awayFlag:'🇦🇺', homeScore:2, awayScore:0, date:'19 Jun', time:'13:00', venue:'Estadio Seattle',               status:'done' },
    { id:22, phase:'grupos', group:'D', home:'Turquía',        homeFlag:'🇹🇷', away:'Paraguay',       awayFlag:'🇵🇾', homeScore:0, awayScore:1, date:'19 Jun', time:'22:00', venue:'Estadio Bahía de San Francisco', status:'done' },
    { id:23, phase:'grupos', group:'D', home:'Turquía',        homeFlag:'🇹🇷', away:'Estados Unidos', awayFlag:'🇺🇸', homeScore:3, awayScore:2, date:'25 Jun', time:'20:00', venue:'Estadio Los Ángeles',            status:'done' },
    { id:24, phase:'grupos', group:'D', home:'Paraguay',       homeFlag:'🇵🇾', away:'Australia',      awayFlag:'🇦🇺', homeScore:0, awayScore:0, date:'25 Jun', time:'20:00', venue:'Estadio Bahía de San Francisco', status:'done' },
    // ── GRUPO E: Alemania · Curazao · Costa de Marfil · Ecuador
    { id:25, phase:'grupos', group:'E', home:'Alemania',        homeFlag:'🇩🇪', away:'Curazao',        awayFlag:'🇨🇼', homeScore:7, awayScore:1, date:'14 Jun', time:'11:00', venue:'Estadio Houston',    status:'done' },
    { id:26, phase:'grupos', group:'E', home:'Costa de Marfil', homeFlag:'🇨🇮', away:'Ecuador',        awayFlag:'🇪🇨', homeScore:1, awayScore:0, date:'14 Jun', time:'17:00', venue:'Estadio Filadelfia', status:'done' },
    { id:27, phase:'grupos', group:'E', home:'Alemania',        homeFlag:'🇩🇪', away:'Costa de Marfil',awayFlag:'🇨🇮', homeScore:2, awayScore:1, date:'20 Jun', time:'14:00', venue:'Estadio Toronto',    status:'done' },
    { id:28, phase:'grupos', group:'E', home:'Ecuador',         homeFlag:'🇪🇨', away:'Curazao',        awayFlag:'🇨🇼', homeScore:0, awayScore:0, date:'20 Jun', time:'17:00', venue:'Estadio Kansas City', status:'done' },
    { id:29, phase:'grupos', group:'E', home:'Curazao',         homeFlag:'🇨🇼', away:'Costa de Marfil',awayFlag:'🇨🇮', homeScore:0, awayScore:2, date:'25 Jun', time:'14:00', venue:'Estadio Filadelfia', status:'done' },
    { id:30, phase:'grupos', group:'E', home:'Ecuador',         homeFlag:'🇪🇨', away:'Alemania',       awayFlag:'🇩🇪', homeScore:2, awayScore:1, date:'25 Jun', time:'14:00', venue:'Estadio Nueva York', status:'done' },
    // ── GRUPO F: Países Bajos · Japón · Suecia · Túnez
    { id:31, phase:'grupos', group:'F', home:'Países Bajos', homeFlag:'🇳🇱', away:'Japón',  awayFlag:'🇯🇵', homeScore:2, awayScore:2, date:'14 Jun', time:'14:00', venue:'Estadio Dallas',    status:'done' },
    { id:32, phase:'grupos', group:'F', home:'Suecia',       homeFlag:'🇸🇪', away:'Túnez',  awayFlag:'🇹🇳', homeScore:5, awayScore:1, date:'14 Jun', time:'20:00', venue:'Estadio Monterrey',  status:'done' },
    { id:33, phase:'grupos', group:'F', home:'Países Bajos', homeFlag:'🇳🇱', away:'Suecia', awayFlag:'🇸🇪', homeScore:5, awayScore:1, date:'20 Jun', time:'11:00', venue:'Estadio Houston',    status:'done' },
    { id:34, phase:'grupos', group:'F', home:'Túnez',        homeFlag:'🇹🇳', away:'Japón',  awayFlag:'🇯🇵', homeScore:0, awayScore:4, date:'20 Jun', time:'20:00', venue:'Estadio Monterrey',  status:'done' },
    { id:35, phase:'grupos', group:'F', home:'Túnez',        homeFlag:'🇹🇳', away:'Países Bajos', awayFlag:'🇳🇱', homeScore:1, awayScore:3, date:'25 Jun', time:'17:00', venue:'Estadio Kansas City', status:'done' },
    { id:36, phase:'grupos', group:'F', home:'Japón',        homeFlag:'🇯🇵', away:'Suecia', awayFlag:'🇸🇪', homeScore:1, awayScore:1, date:'25 Jun', time:'17:00', venue:'Estadio Dallas',    status:'done' },
    // ── GRUPO G: Bélgica · Egipto · RI de Irán · Nueva Zelanda
    { id:37, phase:'grupos', group:'G', home:'Bélgica',      homeFlag:'🇧🇪', away:'Egipto',       awayFlag:'🇪🇬', homeScore:1, awayScore:1, date:'15 Jun', time:'13:00', venue:'Estadio Seattle',            status:'done' },
    { id:38, phase:'grupos', group:'G', home:'RI de Irán',   homeFlag:'🇮🇷', away:'Nueva Zelanda', awayFlag:'🇳🇿', homeScore:2, awayScore:2, date:'15 Jun', time:'19:00', venue:'Estadio Los Ángeles',        status:'done' },
    { id:39, phase:'grupos', group:'G', home:'Bélgica',      homeFlag:'🇧🇪', away:'RI de Irán',   awayFlag:'🇮🇷', homeScore:0, awayScore:0, date:'21 Jun', time:'13:00', venue:'Estadio Los Ángeles',        status:'done' },
    { id:40, phase:'grupos', group:'G', home:'Nueva Zelanda',homeFlag:'🇳🇿', away:'Egipto',       awayFlag:'🇪🇬', homeScore:1, awayScore:3, date:'21 Jun', time:'19:00', venue:'Estadio BC Place Vancouver',  status:'done' },
    { id:41, phase:'grupos', group:'G', home:'Egipto',       homeFlag:'🇪🇬', away:'RI de Irán',   awayFlag:'🇮🇷', homeScore:1, awayScore:1, date:'26 Jun', time:'21:00', venue:'Estadio Seattle',            status:'scheduled' },
    { id:42, phase:'grupos', group:'G', home:'Nueva Zelanda',homeFlag:'🇳🇿', away:'Bélgica',      awayFlag:'🇧🇪', homeScore:1, awayScore:5, date:'26 Jun', time:'21:00', venue:'Estadio Los Ángeles',        status:'scheduled' },
    // ── GRUPO H: España · Cabo Verde · Arabia Saudita · Uruguay
    { id:43, phase:'grupos', group:'H', home:'España',        homeFlag:'🇪🇸', away:'Cabo Verde',     awayFlag:'🇨🇻', homeScore:0, awayScore:0, date:'15 Jun', time:'10:00', venue:'Estadio Atlanta',  status:'done' },
    { id:44, phase:'grupos', group:'H', home:'Arabia Saudita',homeFlag:'🇸🇦', away:'Uruguay',        awayFlag:'🇺🇾', homeScore:1, awayScore:1, date:'15 Jun', time:'16:00', venue:'Estadio Miami',    status:'done' },
    { id:45, phase:'grupos', group:'H', home:'España',        homeFlag:'🇪🇸', away:'Arabia Saudita', awayFlag:'🇸🇦', homeScore:4, awayScore:0, date:'21 Jun', time:'10:00', venue:'Estadio Atlanta',  status:'done' },
    { id:46, phase:'grupos', group:'H', home:'Uruguay',       homeFlag:'🇺🇾', away:'Cabo Verde',     awayFlag:'🇨🇻', homeScore:2, awayScore:2, date:'21 Jun', time:'16:00', venue:'Estadio Miami',    status:'done' },
    { id:47, phase:'grupos', group:'H', home:'Uruguay',       homeFlag:'🇺🇾', away:'España',         awayFlag:'🇪🇸', homeScore:0, awayScore:1, date:'26 Jun', time:'18:00', venue:'Estadio Guadalajara', status:'done' },
    { id:48, phase:'grupos', group:'H', home:'Cabo Verde',    homeFlag:'🇨🇻', away:'Arabia Saudita', awayFlag:'🇸🇦', homeScore:0, awayScore:0, date:'26 Jun', time:'18:00', venue:'Estadio Houston',  status:'done' },
    // ── GRUPO I: Francia · Senegal · Irak · Noruega
    { id:49, phase:'grupos', group:'I', home:'Francia',  homeFlag:'🇫🇷', away:'Senegal', awayFlag:'🇸🇳', homeScore:3, awayScore:1, date:'16 Jun', time:'13:00', venue:'Estadio Nueva York',            status:'done' },
    { id:50, phase:'grupos', group:'I', home:'Noruega',  homeFlag:'🇳🇴', away:'Irak',     awayFlag:'🇮🇶', homeScore:4, awayScore:1, date:'16 Jun', time:'16:00', venue:'Estadio Boston',                status:'done' },
    { id:51, phase:'grupos', group:'I', home:'Francia',  homeFlag:'🇫🇷', away:'Irak',    awayFlag:'🇮🇶', homeScore:3, awayScore:0, date:'22 Jun', time:'15:00', venue:'Estadio Filadelfia',            status:'done' },
    { id:52, phase:'grupos', group:'I', home:'Noruega',  homeFlag:'🇳🇴', away:'Senegal', awayFlag:'🇸🇳', homeScore:3, awayScore:2, date:'22 Jun', time:'18:00', venue:'Estadio Nueva York',            status:'done' },
    { id:53, phase:'grupos', group:'I', home:'Noruega',  homeFlag:'🇳🇴', away:'Francia', awayFlag:'🇫🇷', homeScore:1, awayScore:4, date:'26 Jun', time:'13:00', venue:'Estadio Boston',                status:'done' },
    { id:54, phase:'grupos', group:'I', home:'Senegal',  homeFlag:'🇸🇳', away:'Irak',    awayFlag:'🇮🇶', homeScore:5, awayScore:0, date:'26 Jun', time:'13:00', venue:'Estadio Toronto',               status:'done' },
    // ── GRUPO J: Argentina · Argelia · Austria · Jordania
    { id:55, phase:'grupos', group:'J', home:'Argentina', homeFlag:'🇦🇷', away:'Argelia',  awayFlag:'🇩🇿', homeScore:3, awayScore:0, date:'16 Jun', time:'19:00', venue:'Estadio Kansas City',           status:'done' },
    { id:56, phase:'grupos', group:'J', home:'Austria',   homeFlag:'🇦🇹', away:'Jordania', awayFlag:'🇯🇴', homeScore:3, awayScore:1, date:'16 Jun', time:'22:00', venue:'Estadio Bahía de San Francisco', status:'done' },
    { id:57, phase:'grupos', group:'J', home:'Argentina', homeFlag:'🇦🇷', away:'Austria',  awayFlag:'🇦🇹', homeScore:2, awayScore:0, date:'22 Jun', time:'11:00', venue:'Estadio Dallas',                status:'done' },
    { id:58, phase:'grupos', group:'J', home:'Jordania',  homeFlag:'🇯🇴', away:'Argelia',  awayFlag:'🇩🇿', homeScore:1, awayScore:0, date:'22 Jun', time:'21:00', venue:'Estadio Bahía de San Francisco', status:'done' },
    { id:59, phase:'grupos', group:'J', home:'Jordania',  homeFlag:'🇯🇴', away:'Argentina',awayFlag:'🇦🇷', homeScore:1, awayScore:3, date:'27 Jun', time:'20:00', venue:'Estadio Kansas City',           status:'done' },
    { id:60, phase:'grupos', group:'J', home:'Argelia',   homeFlag:'🇩🇿', away:'Austria',  awayFlag:'🇦🇹', homeScore:3, awayScore:3, date:'27 Jun', time:'20:00', venue:'Estadio Dallas',                status:'done' },
    // ── GRUPO K: Portugal · RD Congo · Uzbekistán · Colombia
    { id:61, phase:'grupos', group:'K', home:'Portugal',   homeFlag:'🇵🇹', away:'RD Congo',   awayFlag:'🇨🇩', homeScore:1, awayScore:1, date:'17 Jun', time:'11:00', venue:'Estadio Houston',         status:'done' },
    { id:62, phase:'grupos', group:'K', home:'Colombia',   homeFlag:'🇨🇴', away:'Uzbekistán', awayFlag:'🇺🇿', homeScore:3, awayScore:1, date:'17 Jun', time:'20:00', venue:'Estadio Ciudad de México', status:'done' },
    { id:63, phase:'grupos', group:'K', home:'Portugal',   homeFlag:'🇵🇹', away:'Uzbekistán', awayFlag:'🇺🇿', homeScore:5, awayScore:0, date:'23 Jun', time:'11:00', venue:'Estadio Houston',         status:'done' },
    { id:64, phase:'grupos', group:'K', home:'Colombia',   homeFlag:'🇨🇴', away:'RD Congo',   awayFlag:'🇨🇩', homeScore:1, awayScore:0, date:'23 Jun', time:'20:00', venue:'Estadio Guadalajara',      status:'done' },
    { id:65, phase:'grupos', group:'K', home:'RD Congo',   homeFlag:'🇨🇩', away:'Uzbekistán', awayFlag:'🇺🇿', homeScore:3, awayScore:1, date:'27 Jun', time:'17:30', venue:'Estadio Atlanta',         status:'done' },
    { id:66, phase:'grupos', group:'K', home:'Colombia',   homeFlag:'🇨🇴', away:'Portugal',   awayFlag:'🇵🇹', homeScore:0, awayScore:0, date:'27 Jun', time:'17:30', venue:'Estadio Miami',            status:'done' },
    // ── GRUPO L: Inglaterra · Croacia · Ghana · Panamá
    { id:67, phase:'grupos', group:'L', home:'Inglaterra', homeFlag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', away:'Croacia', awayFlag:'🇭🇷', homeScore:4, awayScore:2, date:'17 Jun', time:'14:00', venue:'Estadio Dallas',     status:'done' },
    { id:68, phase:'grupos', group:'L', home:'Ghana',      homeFlag:'🇬🇭', away:'Panamá',  awayFlag:'🇵🇦', homeScore:1, awayScore:0, date:'17 Jun', time:'17:00', venue:'Estadio Toronto',    status:'done' },
    { id:69, phase:'grupos', group:'L', home:'Inglaterra', homeFlag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', away:'Ghana',  awayFlag:'🇬🇭', homeScore:0, awayScore:0, date:'23 Jun', time:'14:00', venue:'Estadio Boston',     status:'done' },
    { id:70, phase:'grupos', group:'L', home:'Panamá',     homeFlag:'🇵🇦', away:'Croacia', awayFlag:'🇭🇷', homeScore:0, awayScore:1, date:'23 Jun', time:'17:00', venue:'Estadio Toronto',    status:'done' },
    { id:71, phase:'grupos', group:'L', home:'Croacia',    homeFlag:'🇭🇷', away:'Ghana',   awayFlag:'🇬🇭', homeScore:2, awayScore:1, date:'27 Jun', time:'15:00', venue:'Estadio Filadelfia',  status:'done' },
    { id:72, phase:'grupos', group:'L', home:'Panamá',     homeFlag:'🇵🇦', away:'Inglaterra',awayFlag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', homeScore:0, awayScore:2, date:'27 Jun', time:'15:00', venue:'Estadio Nueva York', status:'done' },
// ── DIECISEISAVOS DE FINAL (Mapeados con Favoritos)
    { id:73, phase:'dieciseisavos', nextId:89, slot:'home', home:'Sudáfrica', homeFlag:'🇿🇦', away:'Canadá', awayFlag:'🇨🇦', homeScore:0, awayScore:1, status:'done', date:'28 Jun' },
    { id:74, phase:'dieciseisavos', nextId:89, slot:'away', home:'Alemania', homeFlag:'🇩🇪', fav:'75%', away:'Paraguay', awayFlag:'🇵🇾', homeScore:null, awayScore:null, status:'scheduled', date:'29 Jun' },
    { id:75, phase:'dieciseisavos', nextId:90, slot:'home', home:'Países Bajos', homeFlag:'🇳🇱', fav:'50%', away:'Marruecos', awayFlag:'🇲🇦', homeScore:null, awayScore:null, status:'scheduled', date:'29 Jun' },
    { id:76, phase:'dieciseisavos', nextId:90, slot:'away', home:'Brasil', homeFlag:'🇧🇷', fav:'65%', away:'Japón', awayFlag:'🇯🇵', homeScore:2, awayScore:1, status:'done', date:'29 Jun' },
    { id:77, phase:'dieciseisavos', nextId:91, slot:'home', home:'Francia', homeFlag:'🇫🇷', fav:'80%', away:'Suecia', awayFlag:'🇸🇪', homeScore:null, awayScore:null, status:'scheduled', date:'30 Jun' },
    { id:78, phase:'dieciseisavos', nextId:91, slot:'away', home:'Costa de Marfil', homeFlag:'🇨🇮', away:'Noruega', awayFlag:'🇳🇴', favAway:'56%', homeScore:null, awayScore:null, status:'scheduled', date:'30 Jun' },
    { id:79, phase:'dieciseisavos', nextId:92, slot:'home', home:'México', homeFlag:'🇲🇽', fav:'51%', away:'Ecuador', awayFlag:'🇪🇨', homeScore:null, awayScore:null, status:'scheduled', date:'30 Jun' },
    { id:80, phase:'dieciseisavos', nextId:92, slot:'away', home:'Inglaterra', homeFlag:'🏴\u200d󠁢󠁥󠁮󠁧󠁿', fav:'80%', away:'RD Congo', awayFlag:'🇨🇩', homeScore:null, awayScore:null, status:'scheduled', date:'01 Jul' },
    { id:81, phase:'dieciseisavos', nextId:93, slot:'home', home:'Estados Unidos', homeFlag:'🇺🇸', fav:'70%', away:'Bosnia', awayFlag:'🇧🇦', homeScore:null, awayScore:null, status:'scheduled', date:'01 Jul' },
    { id:82, phase:'dieciseisavos', nextId:93, slot:'away', home:'Bélgica', homeFlag:'🇧🇪', fav:'45%', away:'Senegal', awayFlag:'🇸🇳', homeScore:null, awayScore:null, status:'scheduled', date:'01 Jul' },
    { id:83, phase:'dieciseisavos', nextId:94, slot:'home', home:'Portugal', homeFlag:'🇵🇹', fav:'60%', away:'Croacia', awayFlag:'🇭🇷', homeScore:null, awayScore:null, status:'scheduled', date:'02 Jul' },
    { id:84, phase:'dieciseisavos', nextId:94, slot:'away', home:'España', homeFlag:'🇪🇸', fav:'80%', away:'Austria', awayFlag:'🇦🇹', homeScore:null, awayScore:null, status:'scheduled', date:'02 Jul' },
    { id:85, phase:'dieciseisavos', nextId:95, slot:'home', home:'Suiza', homeFlag:'🇨🇭', fav:'55%', away:'Argelia', awayFlag:'🇩🇿', homeScore:null, awayScore:null, status:'scheduled', date:'02 Jul' },
    { id:86, phase:'dieciseisavos', nextId:95, slot:'away', home:'Argentina', homeFlag:'🇦🇷', fav:'90%', away:'Cabo Verde', awayFlag:'🇨🇻', homeScore:null, awayScore:null, status:'scheduled', date:'03 Jul' },
    { id:87, phase:'dieciseisavos', nextId:96, slot:'home', home:'Colombia', homeFlag:'🇨🇴', fav:'70%', away:'Ghana', awayFlag:'🇬🇭', homeScore:null, awayScore:null, status:'scheduled', date:'03 Jul' },
    { id:88, phase:'dieciseisavos', nextId:96, slot:'away', home:'Australia', homeFlag:'🇦🇺', away:'Egipto', awayFlag:'🇪🇬', favAway:'45%', homeScore:null, awayScore:null, status:'scheduled', date:'03 Jul' },
    
    // ── OCTAVOS DE FINAL
    { id:89, phase:'octavos', nextId:97, slot:'home', home:'Canadá', homeFlag:'🇨🇦', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'04 Jul' },
    { id:90, phase:'octavos', nextId:97, slot:'away', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'04 Jul' },
    { id:91, phase:'octavos', nextId:98, slot:'home', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'05 Jul' },
    { id:92, phase:'octavos', nextId:98, slot:'away', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'05 Jul' },
    { id:93, phase:'octavos', nextId:99, slot:'home', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'06 Jul' },
    { id:94, phase:'octavos', nextId:99, slot:'away', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'06 Jul' },
    { id:95, phase:'octavos', nextId:100, slot:'home', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'07 Jul' },
    { id:96, phase:'octavos', nextId:100, slot:'away', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'07 Jul' },
    
    // ── CUARTOS DE FINAL
    { id:97, phase:'cuartos', nextId:101, slot:'home', home:'Ganador M89', homeFlag:'⚽', away:'Ganador M90', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'09 Jul' },
    { id:98, phase:'cuartos', nextId:101, slot:'away', home:'Ganador M91', homeFlag:'⚽', away:'Ganador M92', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'10 Jul' },
    { id:99, phase:'cuartos', nextId:102, slot:'home', home:'Ganador M93', homeFlag:'⚽', away:'Ganador M94', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'11 Jul' },
    { id:100, phase:'cuartos', nextId:102, slot:'away', home:'Ganador M95', homeFlag:'⚽', away:'Ganador M96', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'11 Jul' },
    
    // ── SEMIFINALES
    { id:101, phase:'semis', nextId:104, slot:'home', home:'Ganador Semis 1', homeFlag:'⚽', away:'Ganador Semis 2', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'14 Jul' },
    { id:102, phase:'semis', nextId:104, slot:'away', home:'Ganador Semis 3', homeFlag:'⚽', away:'Ganador Semis 4', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'15 Jul' },
    
    // ── TERCER LUGAR Y GRAN FINAL
    { id:103, phase:'tercer-lugar', nextId:null, slot:null, home:'Perdedor Semi 1', homeFlag:'🥉', away:'Perdedor Semi 2', awayFlag:'🥉', homeScore:null, awayScore:null, status:'scheduled', date:'18 Jul' },
    { id:104, phase:'final', nextId:null, slot:null, home:'Finalista 1', homeFlag:'🌍', away:'Finalista 2', awayFlag:'🌍', homeScore:null, awayScore:null, status:'scheduled', date:'19 Jul' }
  ],

  standings: {
    A: [
      { team:'México',        flag:'🇲🇽', pj:3, pg:3, pe:0, pp:0, gf:6, gc:0, pts:9 },
      { team:'Sudáfrica',     flag:'🇿🇦', pj:3, pg:1, pe:1, pp:1, gf:2, gc:3, pts:4 },
      { team:'Rep. de Corea', flag:'🇰🇷', pj:3, pg:1, pe:0, pp:2, gf:2, gc:3, pts:3 },
      { team:'Rep. Checa',    flag:'🇨🇿', pj:3, pg:0, pe:1, pp:2, gf:2, gc:6, pts:1 },
    ],
    B: [
      { team:'Suiza',                flag:'🇨🇭', pj:3, pg:2, pe:1, pp:0, gf:7, gc:2, pts:7 },
      { team:'Canadá',               flag:'🇨🇦', pj:3, pg:1, pe:1, pp:1, gf:7, gc:3, pts:4 },
      { team:'Bosnia y Herzegovina', flag:'🇧🇦', pj:3, pg:1, pe:1, pp:1, gf:4, gc:6, pts:4 },
      { team:'Catar',                flag:'🇶🇦', pj:3, pg:0, pe:1, pp:2, gf:2, gc:9, pts:1 },
    ],
    C: [
      { team:'Marruecos', flag:'🇲🇦', pj:3, pg:2, pe:1, pp:0, gf:6, gc:3, pts:7 },
      { team:'Brasil',    flag:'🇧🇷', pj:3, pg:2, pe:1, pp:0, gf:7, gc:1, pts:7 },
      { team:'Escocia',   flag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', pj:3, pg:1, pe:0, pp:2, gf:1, gc:4, pts:3 },
      { team:'Haití',     flag:'🇭🇹', pj:3, pg:0, pe:0, pp:3, gf:2, gc:8, pts:0 },
    ],
    D: [
      { team:'Estados Unidos', flag:'🇺🇸', pj:3, pg:2, pe:0, pp:1, gf:8, gc:4, pts:6 },
      { team:'Australia',      flag:'🇦🇺', pj:3, pg:1, pe:1, pp:1, gf:2, gc:2, pts:4 },
      { team:'Paraguay',       flag:'🇵🇾', pj:3, pg:1, pe:1, pp:1, gf:2, gc:4, pts:4 },
      { team:'Turquía',        flag:'🇹🇷', pj:3, pg:1, pe:0, pp:2, gf:3, gc:5, pts:3 },
    ],
    E: [
      { team:'Alemania',        flag:'🇩🇪', pj:3, pg:2, pe:0, pp:1, gf:10, gc:4, pts:6 },
      { team:'Costa de Marfil', flag:'🇨🇮', pj:3, pg:2, pe:0, pp:1, gf:4,  gc:2, pts:6 },
      { team:'Ecuador',         flag:'🇪🇨', pj:3, pg:1, pe:1, pp:1, gf:2,  gc:2, pts:4 },
      { team:'Curazao',         flag:'🇨🇼', pj:3, pg:0, pe:1, pp:2, gf:1,  gc:9, pts:1 },
    ],
    F: [
      { team:'Países Bajos', flag:'🇳🇱', pj:3, pg:2, pe:1, pp:0, gf:10, gc:4, pts:7 },
      { team:'Japón',        flag:'🇯🇵', pj:3, pg:1, pe:2, pp:0, gf:7,  gc:3, pts:5 },
      { team:'Suecia',       flag:'🇸🇪', pj:3, pg:1, pe:1, pp:1, gf:7,  gc:7, pts:4 },
      { team:'Túnez',        flag:'🇹🇳', pj:3, pg:0, pe:0, pp:3, gf:2,  gc:12, pts:0 },
    ],
    G: [
      { team:'Bélgica',       flag:'🇧🇪', pj:3, pg:1, pe:2, pp:0, gf:6, gc:2, pts:5 },
      { team:'Egipto',        flag:'🇪🇬', pj:3, pg:1, pe:2, pp:0, gf:5, gc:3, pts:5 },
      { team:'RI de Irán',    flag:'🇮🇷', pj:3, pg:0, pe:3, pp:0, gf:3, gc:3, pts:3 },
      { team:'Nueva Zelanda', flag:'🇳🇿', pj:3, pg:0, pe:1, pp:2, gf:4, gc:10, pts:1 },
    ],
    H: [
      { team:'España',        flag:'🇪🇸', pj:3, pg:2, pe:1, pp:0, gf:5, gc:0, pts:7 },
      { team:'Cabo Verde',    flag:'🇨🇻', pj:3, pg:0, pe:3, pp:0, gf:2, gc:2, pts:3 },
      { team:'Uruguay',       flag:'🇺🇾', pj:3, pg:0, pe:2, pp:1, gf:3, gc:4, pts:2 },
      { team:'Arabia Saudita', flag:'🇸🇦', pj:3, pg:0, pe:2, pp:1, gf:1, gc:5, pts:2 },
    ],
    I: [
      { team:'Francia',  flag:'🇫🇷', pj:3, pg:3, pe:0, pp:0, gf:10, gc:2, pts:9 },
      { team:'Noruega',  flag:'🇳🇴', pj:3, pg:2, pe:0, pp:1, gf:8,  gc:7, pts:6 },
      { team:'Senegal',  flag:'🇸🇳', pj:3, pg:1, pe:0, pp:2, gf:8,  gc:6, pts:3 },
      { team:'Irak',     flag:'🇮🇶', pj:3, pg:0, pe:0, pp:3, gf:1,  gc:12, pts:0 },
    ],
    J: [
      { team:'Argentina', flag:'🇦🇷', pj:3, pg:3, pe:0, pp:0, gf:8, gc:1, pts:9 },
      { team:'Austria',   flag:'🇦🇹', pj:3, pg:1, pe:1, pp:1, gf:6, gc:6, pts:4 },
      { team:'Argelia',   flag:'🇩🇿', pj:3, pg:1, pe:1, pp:1, gf:5, gc:7, pts:4 },
      { team:'Jordania',  flag:'🇯🇴', pj:3, pg:0, pe:0, pp:3, gf:3, gc:8, pts:0 },
    ],
    K: [
      { team:'Colombia',   flag:'🇨🇴', pj:3, pg:2, pe:1, pp:0, gf:4, gc:1, pts:7 },
      { team:'Portugal',   flag:'🇵🇹', pj:3, pg:1, pe:2, pp:0, gf:6, gc:1, pts:5 },
      { team:'RD Congo',   flag:'🇨🇩', pj:3, pg:1, pe:1, pp:1, gf:4, gc:3, pts:4 },
      { team:'Uzbekistán', flag:'🇺🇿', pj:3, pg:0, pe:0, pp:3, gf:2, gc:11, pts:0 },
    ],
    L: [
      { team:'Inglaterra', flag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', pj:3, pg:2, pe:1, pp:0, gf:6, gc:2, pts:7 },
      { team:'Croacia',    flag:'🇭🇷', pj:3, pg:2, pe:0, pp:1, gf:5, gc:5, pts:6 },
      { team:'Ghana',      flag:'🇬🇭', pj:3, pg:1, pe:1, pp:1, gf:2, gc:2, pts:4 },
      { team:'Panamá',     flag:'🇵🇦', pj:3, pg:0, pe:0, pp:3, gf:4, gc:4, pts:0 },
    ],
  },

  scorers: [
    { name:'Lionel Messi', team:'Argentina · Min. 17\', 60\' y 76\' (J1) · Min. 38\' y 90+5\' (J2)', flag:'🇦🇷', goals:6, highlight:true },
    { name:'Kylian Mbappé', team:'Francia · Min. 66\' y 90+6\' (J1) · Min. 14\' y 53\' (J2)', flag:'🇫🇷', goals:4, highlight:true },
    { name:'Erling Haaland', team:'Noruega · Min. 29\' y 42\' (J1) · Min. 48\' y 58\' (J2)', flag:'🇳🇴', goals:4, highlight:true },
    { name:'Vinícius Júnior', team:'Brasil · Min. 31\' y 45+3\' (J1) · Min. 7\' y 45+3\' (J2)', flag:'🇧🇷', goals:4, highlight:true },
    { name:'Ousmane Dembélé', team:'Francia · Min. 66\'', flag:'🇫🇷', goals:4, highlight:true },
    { name:'Jonathan David', team:'Canadá · Min. 29\', 45+3\' y 90+2\' (Hat-trick)', flag:'🇨🇦', goals:3, highlight:true },
    { name:'Deniz Undav', team:'Alemania · Min. 78\' (J1), 68\' y 90+4\' (J2)', flag:'🇩🇪', goals:3, highlight:true },
    { name:'Matheus Cunha', team:'Brasil · Min. 23\' y 36\' (J1) · Min. 60\' (J2)', flag:'🇧🇷', goals:3, highlight:true },
    { name:'Johan Manzambi', team:'Suiza · Min. 74\' y 90\' (J1) · Min. 57\' (J2)', flag:'🇨🇭', goals:3, highlight:true },
    { name:'Harry Kane', team:'Inglaterra · Min. 12\' y 42\' (10 goles en Copas del Mundo)', flag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', goals:3, highlight:true },
    { name:'Ismael Saibari', team:'Marruecos ·', flag:'🇲🇦', goals:3, highlight:true },
    { name:'Ismaïla Sarr', team:'Senegal · Min. 84\' y 90+3\'', flag:'🇸🇳', goals:3, highlight:true },
    { name:'Brian Brobbey', team:'Países Bajos · Min. 5\' y 17\'', flag:'🇳🇱', goals:3, highlight:true },
    { name:'Elijah Just', team:'Nueva Zelanda · Min. 7\' y 55\'', flag:'🇳🇿', goals:3, highlight:true },
    { name:'Cristiano Ronaldo', team:'Portugal · Min. 6\' y 39\' (1er jugador en marcar en 6 Mundiales)', flag:'🇵🇹', goals:2 },
    { name:'Julián Quiñones', team:'México · Min. 11\' (Primer gol del Mundial) · Min. 61\' (J3)', flag:'🇲🇽', goals:2 },
    { name:'Kai Havertz', team:'Alemania · Min. 45+5\' (Pen.) y 88\'', flag:'🇩🇪', goals:2 },
    { name:'Yasin Ayari', team:'Suecia · Min. 7\' y 90+3\'', flag:'🇸🇪', goals:2 },
    { name:'Pape Gueye', team:'Senegal · Min. 59\' y 71\' vs Irak', flag:'🇸🇳', goals:2 },
    { name:'Jude Bellingham', team:'Inglaterra · Min. 47\'', flag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', goals:2 },
    { name:'Nicolas Pépé', team:'Costa de Marfil · Min. 7\' y 64\' vs Curazao', flag:'🇨🇮', goals:2 },
    { name:'Folarin Balogun', team:'Estados Unidos · Min. 30\' y 45+4\'', flag:'🇺🇸', goals:2 },
    { name:'Cyle Larin', team:'Canadá · Min. 55\' (J1) y 16\' (J2)', flag:'🇨🇦', goals:2 },
    { name:'Cody Gakpo', team:'Países Bajos · Min. 47\' y 54\'', flag:'🇳🇱', goals:2 },
    { name:'Daichi Kamada', team:'Japón · Min. 89\' (J1) y 4\' (J2) ⚡ EN VIVO', flag:'🇯🇵', goals:2 },
    { name:'Leandro Trossard', team:'Bélgica · Min. 28\' y 50\' vs Nueva Zelanda', flag:'🇧🇪', goals:2 },
    { name:'Crysencio Summerville', team:'Países Bajos · Min. 73\' (J1) y 89\' (J2)', flag:'🇳🇱', goals:2 },
    { name:'Maximiliano Araújo', team:'Uruguay · Min. 80\' (J1) y 45\' (J2)', flag:'🇺🇾', goals:2 },
    { name:'Mikel Oyarzabal', team:'España · Min. 21\' y 24\'', flag:'🇪🇸', goals:2 },
    { name:'Raúl Jiménez', team:'México · Min. 67\'', flag:'🇲🇽', goals:1 },
    { name:'Hwang In-beom', team:'Corea del Sur', flag:'🇰🇷', goals:1 },
    { name:'Ladislav Krejčí', team:'Chequia · Min. 32\'', flag:'🇨🇿', goals:1 },
    { name:'Breel Embolo', team:'Suiza · Pen. Min. 16\'', flag:'🇨🇭', goals:1 },
    { name:'Nestory Irankunda', team:'Australia · Min. 26\'', flag:'🇦🇺', goals:1 },
    { name:'Connor Metcalfe', team:'Australia · Min. 74\'', flag:'🇦🇺', goals:1 },
    { name:'John McGinn', team:'Escocia · Min. 27\'', flag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', goals:1 },
    { name:'Felix Nmecha', team:'Alemania · Min. 6\'', flag:'🇩🇪', goals:1 },
    { name:'Nico Schlotterbeck', team:'Alemania · Min. 38\'', flag:'🇩🇪', goals:1 },
    { name:'Jamal Musiala', team:'Alemania · Min. 47\'', flag:'🇩🇪', goals:1 },
    { name:'Nathaniel Brown', team:'Alemania · Min. 68\'', flag:'🇩🇪', goals:1 },
    { name:'Amad Diallo', team:'Costa de Marfil · Min. 90\'', flag:'🇨🇮', goals:1 },
    { name:'Virgil van Dijk', team:'Países Bajos · Min. 52\'', flag:'🇳🇱', goals:1 },
    { name:'Keito Nakamura', team:'Japón · Min. 58\'', flag:'🇯🇵', goals:1 },
    { name:'Alexander Isak', team:'Suecia · Min. 30\'', flag:'🇸🇪', goals:1 },
    { name:'Viktor Gyökeres', team:'Suecia · Min. 59\'', flag:'🇸🇪', goals:1 },
    { name:'Mattias Svanberg', team:'Suecia · Min. 84\'', flag:'🇸🇪', goals:1 },
    { name:'Christian Pulisic', team:'Estados Unidos · Min. 78\'', flag:'🇺🇸', goals:1 },
    { name:'Livano Comenencia', team:'Curazao · Min. 21\'', flag:'🇨🇼', goals:1 },
    { name:'Omar Rekik', team:'Túnez · Min. 42\'', flag:'🇹🇳', goals:1 },
    { name:'Romano Schmid', team:'Austria · Min. 21\'', flag:'🇦🇹', goals:1 },
    { name:'Ali Iyad Olwan', team:'Jordania · Min. 50\'', flag:'🇯🇴', goals:1 },
    { name:'Marko Arnautović', team:'Austria · Pen. Min. 90+12\'', flag:'🇦🇹', goals:1 },
    { name:'Bradley Barcola', team:'Francia · Min. 82\'', flag:'🇫🇷', goals:1 },
    { name:'Ibrahim Mbaye', team:'Senegal · Min. 90+5\'', flag:'🇸🇳', goals:1 },
    { name:'Aymen Hussein', team:'Irak · Min. 38\'', flag:'🇮🇶', goals:1 },
    { name:'Leo Østigård', team:'Noruega · Min. 75\'', flag:'🇳🇴', goals:1 },
    { name:'Ramin Rezaeian', team:'RI de Irán · Min. 32\'', flag:'🇮🇷', goals:1 },
    { name:'Mohammad Mohebi', team:'RI de Irán · Min. 64\'', flag:'🇮🇷', goals:1 },
    { name:'Abdulelah Al Amri', team:'Arabia Saudita · Min. 41\'', flag:'🇸🇦', goals:1 },
    { name:'Lamine Yamal', team:'España · Min. 10\'', flag:'🇪🇸', goals:1 },
    { name:'Kevin Pina', team:'Cabo Verde · Min. 21\'', flag:'🇨🇻', goals:1 },
    { name:'Agustín Canobbio', team:'Uruguay · Min. 45+4\'', flag:'🇺🇾', goals:1 },
    { name:'Hélio Varela', team:'Cabo Verde · Min. 61\'', flag:'🇨🇻', goals:1 },
    { name:'Finn Surman', team:'Nueva Zelanda · Min. 14\'', flag:'🇳🇿', goals:1 },
    { name:'Mostafa Zico', team:'Egipto · Min. 58\'', flag:'🇪🇬', goals:1 },
    { name:'Mohamed Salah', team:'Egipto · Min. 67\'', flag:'🇪🇬', goals:1 },
    { name:'Mahmoud Hassan "Trezeguet"', team:'Egipto · Min. 82\'', flag:'🇪🇬', goals:1 },
    { name:'Emam Ashour', team:'Egipto · Min. 20\'', flag:'🇪🇬', goals:1 },
    { name:'Daniel Muñoz', team:'Colombia · Min. 40\' (J1) · Min. 76\' (J2)', flag:'🇨🇴', goals:2 },
    { name:'Luis Díaz', team:'Colombia · Min. 65\'', flag:'🇨🇴', goals:1 },
    { name:'Jáminton Campaz', team:'Colombia', flag:'🇨🇴', goals:1 },
    { name:'Abbosbek Fayzullaev', team:'Uzbekistán · Min. 60\'', flag:'🇺🇿', goals:1 },
    { name:'Marcus Rashford', team:'Inglaterra · Min. 85\'', flag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', goals:1 },
    { name:'Martin Baturina', team:'Croacia · Min. 36\'', flag:'🇭🇷', goals:1 },
    { name:'Petar Musa', team:'Croacia · Min. 55+5\'', flag:'🇭🇷', goals:1 },
    { name:'Yirenkyi', team:'Ghana · Min. 90+5\'', flag:'🇬🇭', goals:1 },
    { name:'João Neves', team:'Portugal · Min. 6\'', flag:'🇵🇹', goals:1 },
    { name:'Yoane Wissa', team:'RD Congo · Min. 45+5\'', flag:'🇨🇩', goals:1 },
    { name:'Michal Sadílek', team:'Rep. Checa · Min. 6\'', flag:'🇨🇿', goals:1 },
    { name:'Teboho Mokoena', team:'Sudáfrica · Pen. Min. 83\'', flag:'🇿🇦', goals:1 },
    { name:'Ruben Vargas', team:'Suiza · Min. 84\' (J1) · Min. 46\' (J2)', flag:'🇨🇭', goals:2 },
    { name:'Granit Xhaka', team:'Suiza · Pen. Min. 90+7\'', flag:'🇨🇭', goals:1 },
    { name:'Ermin Mahmic', team:'Bosnia y Herzegovina · Min. 90+3\'', flag:'🇧🇦', goals:1 },
    { name:'Nathan Saliba', team:'Canadá · Min. 64\'', flag:'🇨🇦', goals:1 },
    { name:'Luis Romo', team:'México · Min. 58\' (Primer clasificado del torneo)', flag:'🇲🇽', goals:1 },
    { name:'Alex Freeman', team:'Estados Unidos · Min. 43\'', flag:'🇺🇸', goals:1 },
    { name:'Matías Galarza', team:'Paraguay · Min. 2\'', flag:'🇵🇾', goals:1 },
    { name:'Anthony Elanga', team:'Suecia · Min. 59\'', flag:'🇸🇪', goals:1 },
    { name:'Franck Kessié', team:'Costa de Marfil · Min. 39\'', flag:'🇨🇮', goals:1 },
    { name:'A. Ueda', team:'Japón · Min. 31\' ⚡ EN VIVO', flag:'🇯🇵', goals:1 },
    { name:'Marcus Pedersen', team:'Noruega · Min. 43\'', flag:'🇳🇴', goals:1 },
    { name:'Nizar Al-Rashdan', team:'Jordania · Min. 36\'', flag:'🇯🇴', goals:1 },
    { name:'Nuno Mendes', team:'Portugal · Min. 17\'', flag:'🇵🇹', goals:1 },
    { name:'Rafael Leão', team:'Portugal · Min. 87\'', flag:'🇵🇹', goals:1 },
    { name:'Ante Budimir',        team:'Croacia · Min. 54\'',            flag:'🇭🇷', goals:1 },
    { name:'Kerim Alajbegović',   team:'Bosnia y Herzegovina · Min. 29\'',flag:'🇧🇦', goals:1 },
    { name:'Hassan Al-Haydos',    team:'Catar · Min. 42\'',              flag:'🇶🇦', goals:1 },
    { name:'Mateo Chávez',       team:'México · Min. 54\'',             flag:'🇲🇽', goals:1 },
    { name:'Álvaro Fidalgo',     team:'México · Min. 90+4\'',           flag:'🇲🇽', goals:1 },
    { name:'Achraf Hakimi',      team:'Marruecos · Min. 39\'',          flag:'🇲🇦', goals:1 },
    { name:'Soufiane Rahimi',    team:'Marruecos · Min. 78\'',          flag:'🇲🇦', goals:1 },
    { name:'Gessime Yassine',    team:'Marruecos · Min. 89\'',          flag:'🇲🇦', goals:1 },
    { name:'Wilson Isidor',      team:'Haití · Min. 43\'',              flag:'🇭🇹', goals:1 },
    { name:'Thapelo Maseko',     team:'Sudáfrica · Min. 63\'',          flag:'🇿🇦', goals:1 },
    // ── Autogoles
    { name:'Sultan Al-Brake',   team:'Catar · AG Min. 34\' (a favor de Bosnia y Herzegovina)', flag:'🇶🇦', goals:1, isOwnGoal:true },
    { name:'Khusanov', team:'Uzbekistán · AG Min. 60\' (a favor de Portugal)', flag:'🇺🇿', goals:1, isOwnGoal:true },
    { name:'Hassan Altambakti', team:'Arabia Saudita · AG Min. 55\' (a favor de España)', flag:'🇸🇦', goals:1, isOwnGoal:true },
    { name:'Aymen Hussein', team:'Irak · AG Min. 90+3\' (a favor de Noruega)', flag:'🇮🇶', goals:1, isOwnGoal:true },
    { name:'Yazan Al-Arab', team:'Jordania · AG Min. 76\' (a favor de Austria)', flag:'🇯🇴', goals:1, isOwnGoal:true },
    { name:'Mohamed Hany', team:'Egipto · AG Min. 66\' (a favor de Bélgica)', flag:'🇪🇬', goals:1, isOwnGoal:true },
    { name:'Mohamed Al Mannai', team:'Catar · AG Min. 75\' (a favor de Canadá)', flag:'🇶🇦', goals:1, isOwnGoal:true },
    { name:'Miro Muheim', team:'Suiza · AG Min. 90+3\' (a favor de Catar)', flag:'🇨🇭', goals:1, isOwnGoal:true },
    { name:'Cameron Burgess', team:'Australia · AG Min. 11\' (a favor de Estados Unidos)', flag:'🇦🇺', goals:1, isOwnGoal:true },
  ],
  yellowCards: [
    { player:'Yoel Bárcenas',          team:'Panamá',           flag:'🇵🇦', qty:1, min:'Min. 61\'' },
    { player:'Petar Sučić',            team:'Croacia',          flag:'🇭🇷', qty:1, min:'Min. 90+2\'' },
    { player:'Jhon Lucumí',            team:'Colombia',         flag:'🇨🇴', qty:1, min:'Min. 56\'' },
    { player:'Jefferson Lerma',        team:'Colombia',         flag:'🇨🇴', qty:1, min:'Min. 90+4\'' },
    { player:'Charles Pickel',         team:'RD Congo',         flag:'🇨🇩', qty:1, min:'Min. 90+4\'' },
    { player:'Granit Xhaka',           team:'Suiza',            flag:'🇨🇭', qty:1, min:'Min. 32\'' },
    { player:'Cyle Larin',             team:'Canadá',           flag:'🇨🇦', qty:1, min:'Min. 32\'' },
    { player:'Odiljon Hamrobekov',     team:'Uzbekistán',       flag:'🇺🇿', qty:1, min:'Min. 14\'' },
    { player:'Renato Veiga',           team:'Portugal',         flag:'🇵🇹', qty:1, min:'Min. 68\'' },
    { player:'Declan Rice',            team:'Inglaterra',       flag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', qty:1, min:'Min. 41\'' },
    { player:'Iñaki Williams',         team:'Ghana',            flag:'🇬🇭', qty:1, min:'Min. 60\'' },
    { player:'Stefan Posch',           team:'Austria',          flag:'🇦🇹', qty:1, min:'Min. 40\'' },
    { player:'Konrad Laimer',          team:'Austria',          flag:'🇦🇹', qty:1, min:'Min. 76\'' },
    { player:'Facundo Medina',         team:'Argentina',        flag:'🇦🇷', qty:1, min:'Min. 76\'' },
    { player:'Leandro Paredes',        team:'Argentina',        flag:'🇦🇷', qty:1, min:'Min. 90+2\'' },
    { player:'Amir Al-Ammari',         team:'Irak',             flag:'🇮🇶', qty:1, min:'Min. 6\'' },
    { player:'Ramiz Zerrouki',         team:'Argelia',          flag:'🇩🇿', qty:1, min:'Min. 44\'' },
    { player:'S. Aldawsari',           team:'Arabia Saudita',   flag:'🇸🇦', qty:1, min:'Min. 30\'' },
    { player:'Mohamed Kanno',          team:'Arabia Saudita',   flag:'🇸🇦', qty:1, min:'Min. 60\'' },
    { player:'R. Lukaku',              team:'Bélgica',          flag:'🇧🇪', qty:1, min:'Min. 3\'' },
    { player:'Saeid Ezatolahi',        team:'RI de Irán',       flag:'🇮🇷', qty:1, min:'Min. 33\'' },
    { player:'R. Bentancur',           team:'Uruguay',          flag:'🇺🇾', qty:1, min:'Min. 20\'' },
    { player:'Sidny Lopes Cabral',     team:'Cabo Verde',       flag:'🇨🇻', qty:1, min:'Min. 5\'' },
    { player:'Mathias Olivera',        team:'Uruguay',          flag:'🇺🇾', qty:1, min:'Min. 58\'' },
    { player:'Diney Borges',           team:'Cabo Verde',       flag:'🇨🇻', qty:1, min:'Min. 90+2\'' },
    { player:'Mohanad Lasheen',        team:'Egipto',           flag:'🇪🇬', qty:1, min:'Min. 17\'' },
    { player:'Sarpreet Singh',         team:'Nueva Zelanda',    flag:'🇳🇿', qty:1, min:'Min. 20\'' },
    { player:'Callum McCowatt',        team:'Nueva Zelanda',    flag:'🇳🇿', qty:1, min:'Min. 33\'' },
    { player:'Gabriel Gudmundsson',    team:'Suecia',           flag:'🇸🇪', qty:1, min:'Min. 53\'' },
    { player:'Yasin Ayari',            team:'Suecia',           flag:'🇸🇪', qty:1, min:'Min. 75\'' },
    { player:'Lucas Bergvall',         team:'Suecia',           flag:'🇸🇪', qty:1, min:'Min. 80\'' },
    { player:'Jordy Alcivar',          team:'Ecuador',          flag:'🇪🇨', qty:1, min:'Min. 38\'' },
    { player:'L. Bacuna',              team:'Curazao',          flag:'🇨🇼', qty:1, min:'Min. 39\'' },
    { player:'Juninho Bacuna',         team:'Curazao',          flag:'🇨🇼', qty:1, min:'Min. 53\'' },
    { player:'Livano Comenencia',      team:'Curazao',          flag:'🇨🇼', qty:1, min:'Min. 56\'' },
    { player:'Jurien Gaari',           team:'Curazao',          flag:'🇨🇼', qty:1, min:'Min. 75\'' },
    { player:'Gervane Kastaneer',      team:'Curazao',          flag:'🇨🇼', qty:1, min:'Min. 90\'' },
    { player:'Jordan Bos',             team:'Australia',        flag:'🇦🇺', qty:1, min:'Min. 16\'' },
    { player:'Alessandro Circati',     team:'Australia',        flag:'🇦🇺', qty:1, min:'Min. 32\'' },
    { player:'Antonee Robinson',       team:'Estados Unidos',   flag:'🇺🇸', qty:1, min:'Min. 56\'' },
    { player:'J. Italiano',            team:'Australia',        flag:'🇦🇺', qty:1, min:'Min. 89\'' },
    { player:'Harry Souttar',          team:'Australia',        flag:'🇦🇺', qty:1, min:'Min. 89\'' },
    { player:'Folarin Balogun',        team:'Estados Unidos',   flag:'🇺🇸', qty:1, min:'Min. 89\'' },
    { player:'Chris Richards',         team:'Estados Unidos',   flag:'🇺🇸', qty:1, min:'Min. 90+2\'' },
    { player:'Matías Galarza',         team:'Paraguay',         flag:'🇵🇾', qty:1, min:'Min. 4\'' },
    { player:'Eren Elmali',            team:'Turquía',          flag:'🇹🇷', qty:1, min:'Min. 71\'' },
    { player:'Arcus Carlens',          team:'Haití',            flag:'🇭🇹', qty:1, min:'Min. 4\'' },
    { player:'Frantzdy Pierrot',       team:'Haití',            flag:'🇭🇹', qty:1, min:'Min. 45+3\'' },
    { player:'D. Santos',              team:'Brasil',           flag:'🇧🇷', qty:1, min:'Min. 65\'' },
    { player:'Danley Jean Jacques',    team:'Haití',            flag:'🇭🇹', qty:1, min:'Min. 72\'' },
    { player:'Issa Diop',              team:'Marruecos',        flag:'🇲🇦', qty:1, min:'Min. 23\'' },
    { player:'Andrew Robertson',       team:'Escocia',          flag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', qty:1, min:'Min. 65\'' },
    { player:'Teboho Mokoena',         team:'Sudáfrica',        flag:'🇿🇦', qty:1, min:'—' },
    { player:'Nkosinathi Sibisi',      team:'Sudáfrica',        flag:'🇿🇦', qty:1, min:'—' },
    { player:'Ermedin Demirović',      team:'Bosnia y Herzegovina', flag:'🇧🇦', qty:1, min:'—' },
    { player:'Alistair Johnston',      team:'Canadá',           flag:'🇨🇦', qty:1, min:'—' },
    { player:'Gustavo Gómez',          team:'Paraguay',         flag:'🇵🇾', qty:1, min:'Falta táctica / Juego brusco' },
    { player:'Andrés Cubas',           team:'Paraguay',         flag:'🇵🇾', qty:1, min:'Reiteración de faltas' },
    { player:'Weston McKennie',        team:'Estados Unidos',   flag:'🇺🇸', qty:1, min:'Protestas al árbitro' },
    { player:'Homam Ahmed',            team:'Catar',            flag:'🇶🇦', qty:1, min:'Min. 15\'' },
    { player:'Jassem Gaber',           team:'Catar',            flag:'🇶🇦', qty:1, min:'Min. 22\'' },
    { player:'Granit Xhaka',           team:'Suiza',            flag:'🇨🇭', qty:1, min:'Min. 41\'' },
    { player:'Bruno Guimarães',        team:'Brasil',           flag:'🇧🇷', qty:1, min:'Min. 36\'' },
    { player:'Lucas Paquetá',          team:'Brasil',           flag:'🇧🇷', qty:1, min:'Min. 42\'' },
    { player:'Carlens Arcus',          team:'Haití',            flag:'🇭🇹', qty:1, min:'Min. 38\'' },
    { player:'Billy Gilmour',          team:'Escocia',          flag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', qty:1, min:'Min. 45\'' },
    { player:'Scott McTominay',        team:'Escocia',          flag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', qty:1, min:'Min. 90\'' },
    { player:'John McGinn',            team:'Escocia',          flag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', qty:1, min:'Min. 90+4\'' },
    { player:'Yunus Akgün',            team:'Turquía',          flag:'🇹🇷',    qty:1, min:'Min. 85\'' },
    { player:'Crysencio Summerville',  team:'Países Bajos',     flag:'🇳🇱',    qty:1, min:'Min. 61\'' },
    { player:'Memphis Depay',          team:'Países Bajos',     flag:'🇳🇱',    qty:1, min:'Min. 83\'' },
    { player:'Micky van de Ven',       team:'Países Bajos',     flag:'🇳🇱',    qty:1, min:'Min. 90+1\'' },
    { player:'Seko Fofana',            team:'Costa de Marfil',  flag:'🇨🇮',    qty:1, min:'Min. 28\'' },
    { player:'Franck Kessié',          team:'Costa de Marfil',  flag:'🇨🇮',    qty:1, min:'Min. 38\'' },
    { player:'Georges Doué',           team:'Costa de Marfil',  flag:'🇨🇮',    qty:1, min:'Min. 40\'' },
    { player:'Jackson Porozo',         team:'Ecuador',          flag:'🇪🇨',    qty:1, min:'Min. 73\'' },
    { player:'Ladislav Krejčí',        team:'Rep. Checa',       flag:'🇨🇿',    qty:1, min:'Min. 75\'' },
    { player:'Thalente Mbatha',        team:'Sudáfrica',        flag:'🇿🇦',    qty:1, min:'Min. 40\'' },
    { player:'Teboho Mokoena',         team:'Sudáfrica · ⚠️ 2ª', flag:'🇿🇦',    qty:1, min:'Min. 33\'' },
    { player:'Amar Dedić',             team:'Bosnia y Herzegovina', flag:'🇧🇦', qty:1, min:'Min. 59\'' },
    { player:'Edin Džeko',             team:'Bosnia y Herzegovina', flag:'🇧🇦', qty:1, min:'Min. 61\'' },
    { player:'Nico Elvedi',            team:'Suiza',            flag:'🇨🇭',    qty:1, min:'Min. 65\'' },
    { player:'Derek Cornelius',        team:'Canadá',           flag:'🇨🇦',    qty:1, min:'Min. 9\'' },
    { player:'Ahmed Fathi',            team:'Catar',            flag:'🇶🇦',    qty:1, min:'Min. 62\'' },
    { player:'K. Lee',                 team:'Rep. de Corea',    flag:'🇰🇷',    qty:1, min:'Min. 4\'' },
    { player:'Paik Seung-Ho',          team:'Rep. de Corea',    flag:'🇰🇷',    qty:1, min:'Min. 58\'' },
    { player:'Johan Mojica',           team:'Colombia',         flag:'🇨🇴',    qty:1, min:'Min. 7\'' },
    { player:'Abdukodir Khusanov',     team:'Uzbekistán',       flag:'🇺🇿',    qty:1, min:'Min. 34\'' },
    { player:'Yirenkyi',               team:'Ghana',            flag:'🇬🇭',    qty:1, min:'Min. 16\'' },
    { player:'César Blackman',         team:'Panamá',           flag:'🇵🇦',    qty:1, min:'Min. 72\'' },
    { player:'Carlos Harvey',          team:'Panamá',           flag:'🇵🇦',    qty:1, min:'Min. 90+8\'' },
    { player:'Bernardo Silva',         team:'Portugal',         flag:'🇵🇹',    qty:1, min:'Min. 13\'' },
    { player:'Chancel Mbemba',         team:'RD Congo',         flag:'🇨🇩',    qty:1, min:'Min. 32\'' },
    { player:'Nelson Semedo',          team:'Portugal',         flag:'🇵🇹',    qty:1, min:'Min. 88\'' },
    { player:'Tomás Araújo',           team:'Portugal',         flag:'🇵🇹',    qty:1, min:'Min. 90+1\'' },
    { player:'Marcel Sabitzer',        team:'Austria',          flag:'🇦🇹',    qty:1, min:'Min. 77\'' },
    { player:'Zaid Tahseen',           team:'Irak',             flag:'🇮🇶',    qty:1, min:'Min. 86\'' },
    { player:'Ehsan Hajsafi',          team:'RI de Irán',       flag:'🇮🇷',    qty:1, min:'Min. 89\'' },
    { player:'Abdulelah Al Amri',      team:'Arabia Saudita',   flag:'🇸🇦',    qty:1, min:'Min. 44\'' },
    { player:'Sidny Lopes Cabral',     team:'Cabo Verde',       flag:'🇨🇻',    qty:1, min:'Min. 16\'' },
    { player:'Pedri',                  team:'España',           flag:'🇪🇸',    qty:1, min:'Min. 90+2\'' },
    { player:'Marwan Attia',           team:'Egipto',           flag:'🇪🇬',    qty:1, min:'Min. 13\'' },
    { player:'Timothy Castagne',       team:'Bélgica',          flag:'🇧🇪',    qty:1, min:'Min. 14\'' },
    { player:'Ahmed Abou El Fotouh',   team:'Egipto',           flag:'🇪🇬',    qty:1, min:'Min. 34\'' },
    { player:'Maxim De Cuyper',        team:'Bélgica',          flag:'🇧🇪',    qty:1, min:'Min. 75\'' },
  ],

  redCards: [
    { player:'Nathan Ngoy',          team:'Bélgica',              flag:'🇧🇪', min:'Min. 67\'',       desc:'Roja directa que deja a Bélgica con 10 hombres en un partido sin goles ante Irán.' },
    { player:'Miguel Almirón',       team:'Paraguay',              flag:'🇵🇾', min:'Min. 45+3\'',     desc:'Roja directa que deja a Paraguay con 10 hombres antes del descanso ante Turquía.' },
    { player:'Yaya Sithole',         team:'Sudáfrica',            flag:'🇿🇦', min:'Doble amarilla', desc:'Expulsado por doble amonestación tras faltas consecutivas.' },
    { player:'Themba Zwane',         team:'Sudáfrica',            flag:'🇿🇦', min:'Roja directa',   desc:'Tarjeta roja tras un altercado y manotazo a un rival.' },
    { player:'César Montes',         team:'México',                flag:'🇲🇽', min:'Roja directa',   desc:'Expulsado sobre la hora por una fuerte entrada tardía.' },
    { player:'Tarik Muharemović',    team:'Bosnia y Herzegovina', flag:'🇧🇦', min:'Min. 80\'',       desc:'Roja directa que condena a Bosnia a jugar con 10 los últimos minutos ante Suiza.' },
    { player:'Homam Ahmed',          team:'Catar',                flag:'🇶🇦', min:'Min. 33\'',       desc:'Roja directa que reduce a Catar a 10 hombres ante Canadá desde el primer tiempo.' },
    { player:'Assim Madibo',         team:'Catar',                flag:'🇶🇦', min:'Min. 53\'',       desc:'Segunda roja para Catar: el equipo acaba el partido con 9 hombres.' },
  ],

  crazyNumbers: [
    { num:'137', label:'Goles en los primeros 46 partidos del torneo', sub:'3.0 por partido — Ronaldo ya marcó en 6 Mundiales distintos' },
    { num:'40%', label:'De los partidos han tenido gol antes del minuto 15', sub:'El torneo arranca caliente — casi 1 de cada 2 juegos tiene gol tempranero' },
    { num:'1°', label:'Gol de Julián Quiñones para México', sub:'El primer gol oficial del Mundial 2026 · Min. 11\'' },
    { num:'28', label:'Tarjetas amarillas acumuladas en lo que va del torneo', sub:'Costa de Marfil acumula 3 en un solo partido' },
  ],

  noticias: [
    {
      accentColor: 'gold',
      kicker: '🏆 Camino a Dieciseisavos · Análisis',
      kickerClass: 'gold',
      title: 'El mapa de dieciseisavos empieza a tomar forma: los cruces que todos quieren evitar',
      text: 'La fase de grupos empieza a definir el camino rumbo a la eliminación directa. Las grandes selecciones buscan asegurar posiciones altas para evitar cruces complicados en los primeros partidos de eliminación. Los líderes actuales comienzan a marcar territorio: Argentina, Brasil, España, Alemania, Francia y Portugal. Mientras las tablas todavía pueden cambiar, algunos duelos ya aparecen como posibles enfrentamientos de alto impacto: Argentina vs Alemania, Brasil vs Países Bajos, España vs Francia, México vs una potencia europea. La diferencia entre terminar primero o segundo puede cambiar completamente el camino hacia la final — en un torneo de 48 equipos, la selección de rivales en el cuadro es más importante que nunca.',
      jugadorFlag: '🏆',
      jugadorName: 'Fase Eliminatoria',
      jugadorLabel: 'Los cruces de alto riesgo ya están en el horizonte',
      tags: ['#Dieciseisavos2026', '#CrucesDelMundial', '#RouteToFinal'],
      momento: 'Terminar 1° o 2° en el grupo puede significar la diferencia entre enfrentar a un gigante o un equipo sorpresa.',
      impacto: 'Los equipos que controlan su grupo controlan su destino. Los que empatan puntos, dependen del gol diferencia.',
    },
    {
      accentColor: 'gold',
      kicker: '🇲🇽 Impacto Cultural · Fan Festivals',
      kickerClass: 'gold',
      title: 'El alma del Mundial es latina: los datos demuestran que México opacó a EE. UU. y Canadá en el arranque del Mundial',
      text: 'Hay torneos que se ganan en la cancha y otros que se ganan en la calle. Las principales consultoras de turismo y los reportes de ocupación de las Fan Zones de la FIFA revelan datos contundentes: México está liderando por completo la experiencia e impacto cultural del Mundial 2026, superando drásticamente a Estados Unidos y Canadá en las métricas de hospitalidad y asistencia. Mientras las sedes de Los Ángeles y Toronto registraron una asistencia promedio del 65% de su capacidad en las primeras jornadas —golpeadas por los altos costos de transporte y accesos—, el FIFA Fan Festival del Centro Histórico de Guadalajara y el de la Ciudad de México reportaron un lleno absoluto del 100% desde el día uno, promediando más de 45,000 personas diarias. No es solo una cifra de turismo: es la confirmación de algo que cualquier aficionado latinoamericano ya sabía. El fútbol en México no se consume, se vive.',
      jugadorFlag: '🇲🇽',
      jugadorName: 'Fan Festival GDL y CDMX',
      jugadorLabel: '100% de ocupación · +45,000 personas diarias',
      tags: ['#MéxicoEsFiesta', '#FanFest2026', '#LatinPower'],
      momento: 'Mientras LA y Toronto rondan el 65% de ocupación, las Fan Zones mexicanas no han tenido un solo boleto disponible.',
      impacto: 'México se consolida como el verdadero corazón cultural del torneo, más allá de los resultados deportivos.',
    },
    {
      accentColor: '',
      kicker: '🇲🇽 Jornada 1 · Grupo A · México 2-0 Sudáfrica',
      kickerClass: '',
      title: 'El tercer Mundial llegó y México no falló: Quiñones, Jiménez y la ilusión de una nueva generación',
      text: 'Hay países que cargan el fútbol como una religión. México es uno de ellos, y el 11 de junio de 2026 lo volvió a demostrar. Para el Tri, este no es cualquier Mundial: es el tercero en el que México figura entre los países sede, después de 1970 y 1986, y el primero en casa en cuatro décadas. La deuda histórica del quinto partido —ese maldito techo que siempre se aparece en los dieciseisavos— pesaba en el ambiente, pero dentro del estadio Ciudad de México nadie quieras escuchar de maldiciones. Quiñones abrió el marcador al minuto 11 con un disparo que entró por el ángulo bajo y encendió una mezcla de alivio y euforia que nadie en las tribunas sabía cómo procesar. Era el primer gol de este Mundial. Su gol. El de México. Raúl Jiménez cerró la cuenta al 67\'. Pero el momento que nadie va a olvidar llegó cuando ingresó la Hormiga González y, con él, Gilberto Mora — 17 años recién cumplidos.',
      jugadorFlag: '🇲🇽',
      jugadorName: 'Julián Quiñones',
      jugadorLabel: 'Primer gol del Mundial 2026 · Min. 11\'',
      tags: ['#VamosTricolor', '#GDL2026', '#HormigaGonzalez'],
      momento: 'Min. 11\' — Quiñones dispara cruzado y convierte el primer gol oficial del Mundial 2026.',
      impacto: 'México lidera el Grupo A con 3 pts. La ilusión del quinto partido está viva.',
    },
    {
      accentColor: 'lime',
      kicker: '🚑 Parte Médico · Las Bajas del Torneo',
      kickerClass: 'lime',
      title: 'El Mundial de las lesiones: las estrellas que se quedaron fuera antes de empezar',
      text: 'Si algo nos enseñó esta previa es que el cuerpo humano tiene límites, aunque la agenda FIFA no quiera saberlo. El parte médico previo al arranque ha sido durísimo y supera con creces el índice de lesionados de torneos anteriores, todo por la carga brutal de la temporada europea de clubes. Brasil es, sin duda, el más golpeado: perdió a Rodrygo Goes, a Éder Militão y a la joven promesa Estevão justo antes de viajar, mientras su lateral Noussair Mazraoui quedó descartado para el arranque de grupos por una luxación de hombro. Japón sufrió un golpe devastador con la baja de su capitán Wataru Endo, quien además anunció su retiro de la selección. Países Bajos perdió por completo su columna vertebral creativa tras las roturas de ligamentos de Xavi Simons y Jerdy Schouten. México tampoco se salvó: su portero titular, Luis Malagón, quedó fuera de la convocatoria por una lesión de último momento. La lista sigue creciendo.',
      jugadorFlag: '🇧🇷',
      jugadorName: 'Rodrygo, Militão, Estevão',
      jugadorLabel: 'Bajas confirmadas · Brasil',
      tags: ['#PartesMedicos', '#Mundial2026', '#FuerzaCampeones'],
      momento: 'Brasil llega al torneo sin tres piezas clave de su ofensiva y su defensa.',
      impacto: 'Cada selección golpeada deberá reconfigurar su plan de juego. El nivel competitivo del grupo puede cambiar drásticamente.',
    },
  ],

  gdlMatches: [
    { id:1,  sede:'cdmx', grupo:'Grupo A', home:'México',        homeFlag:'🇲🇽', away:'Sudáfrica',    awayFlag:'🇿🇦', homeScore:2,    awayScore:0,    date:'11 Jun', time:'13:00', status:'done' },
    { id:62, sede:'cdmx', grupo:'Grupo K', home:'Colombia',      homeFlag:'🇨🇴', away:'Uzbekistán',   awayFlag:'🇺🇿', homeScore:3, awayScore:1, date:'17 Jun', time:'20:00', status:'done' },
    { id:5,  sede:'cdmx', grupo:'Grupo A', home:'Rep. Checa',   homeFlag:'🇨🇿', away:'México',       awayFlag:'🇲🇽', homeScore:0, awayScore:3, date:'24 Jun', time:'19:00', status:'done' },
    { id:79, sede:'cdmx', grupo:'Dieciseisavos', home:'México', homeFlag:'🇲🇽', away:'3° C/E/F/H/I', awayFlag:'⭐', homeScore:null, awayScore:null, date:'30 Jun', time:'19:00', status:'scheduled' },
    { id:92, sede:'cdmx', grupo:'Cuartos de Final', home:'Por definir', homeFlag:'⚽', away:'Por definir', awayFlag:'⚽', homeScore:null, awayScore:null, date:'05 Jul', time:'18:00', status:'scheduled' },
    { id:2,  sede:'gdl',  grupo:'Grupo A', home:'Rep. de Corea', homeFlag:'🇰🇷', away:'Rep. Checa',  awayFlag:'🇨🇿', homeScore:2,    awayScore:1,    date:'11 Jun', time:'20:00', status:'done' },
    { id:4,  sede:'gdl',  grupo:'Grupo A', home:'México',        homeFlag:'🇲🇽', away:'Rep. de Corea',awayFlag:'🇰🇷', homeScore:1, awayScore:0, date:'18 Jun', time:'19:00', status:'done' },
    { id:64, sede:'gdl',  grupo:'Grupo K', home:'Colombia',      homeFlag:'🇨🇴', away:'RD Congo',    awayFlag:'🇨🇩', homeScore:1, awayScore:0, date:'23 Jun', time:'20:00', status:'done' },
    { id:47, sede:'gdl',  grupo:'Grupo H', home:'Uruguay',       homeFlag:'🇺🇾', away:'España',      awayFlag:'🇪🇸', homeScore:0, awayScore:1, date:'26 Jun', time:'18:00', status:'scheduled' },
    { id:32, sede:'mty',  grupo:'Grupo F', home:'Suecia',        homeFlag:'🇸🇪', away:'Túnez',       awayFlag:'🇹🇳', homeScore:5, awayScore:1, date:'14 Jun', time:'20:00', status:'done' },
    { id:34, sede:'mty',  grupo:'Grupo F', home:'Túnez',         homeFlag:'🇹🇳', away:'Japón',        awayFlag:'🇯🇵', homeScore:0, awayScore:4, date:'20 Jun', time:'20:00', status:'done' },
    { id:6,  sede:'mty',  grupo:'Grupo A', home:'Sudáfrica',     homeFlag:'🇿🇦', away:'Rep. de Corea',awayFlag:'🇰🇷', homeScore:1, awayScore:0, date:'24 Jun', time:'19:00', status:'done' },
    { id:75, sede:'mty',  grupo:'Dieciseisavos', home:'Países Bajos', homeFlag:'🇳🇱', away:'Marruecos',  awayFlag:'🇲🇦', homeScore:null, awayScore:null, date:'29 Jun', time:'19:00', status:'scheduled' },
  ],

  eventos: [
    {
      nombre: 'Maná — "Una Noche Histórica"',
      categoria: 'Concierto',
      categoriaColor: '#FF4D1C',
      emoji: '🎸',
      fecha: 'Miércoles 17 de junio',
      hora: 'Accesos desde las 18:00 hrs',
      lugar: 'La Minerva · Av. Ignacio L. Vallarta',
      acceso: 'GRATIS',
      nota: 'Un día antes del partido México vs. Rep. de Corea en el Estadio Guadalajara.',
    },
    {
      nombre: 'Alejandro Fernández',
      categoria: 'Concierto',
      categoriaColor: '#D4A820',
      emoji: '🎤',
      fecha: 'Jueves 25 de junio',
      hora: 'A partir de las 20:00 hrs',
      lugar: 'La Minerva · Av. Ignacio L. Vallarta',
      acceso: 'GRATIS',
      nota: 'Noche de festejo en la ciudad anfitriona del Mundial.',
    },
  ],

  curiosidades: [
    { emoji:'🌵', titulo:'La Hormiga González y la generación que ilusiona', texto:'Cuando Gilberto Mora entró al campo ante Sudáfrica con 17 años, el estadio Ciudad de México quedó en silencio por un segundo —y luego estalló. La Hormiga González ya es símbolo de la nueva cara del Tri: rápido, desequilibrante y sin miedo. Esta selección no carga solo con la experiencia de Jiménez o Quiñones; lleva también la energía cruda de una generación que no sabe lo que es el quinto partido y por eso quizás lo llegue a romper.' },
    { emoji:'🏟️', titulo:'El Estadio Guadalajara tiene historia propia', texto:'El recinto de Chivas —renombrado como Estadio Guadalajara para este torneo— ha sido sede de Mundiales solo en la mente de sus aficionados... hasta 2026. Antes de él, el Jalisco fue escenario del "Gol del Siglo" de Maradona en 1986. GDL lleva la historia en el ADN.' },
    { emoji:'🌆', titulo:'GDL no es ciudad anfitriona. Es ciudad protagonista.', texto:'Desde la Plaza de los Mariachis hasta la Catedral, desde Chapultepec hasta la explanada de la Minerva, Guadalajara vive el Mundial como ninguna otra ciudad en Norte América. No hay turno de descanso. Los 5.3 millones del área metropolitana convirtieron cada partido —incluso los que no son en Guadalajara— en un evento colectivo.' },
    { emoji:'⚽', titulo:'1970, 1986, 2026: trinidad mundialista', texto:'Solo una docena de ciudades en el mundo han sido sede del Mundial tres veces. GDL se une al club con Ciudad de México, Roma y París. Para una ciudad que también produjo a Cardenal, Rulfo y al mariachi, el fútbol es el menor de sus logros.' },
  ],
};

// ══════════════════════════════════════════════════════════
// STATE
// ══════════════════════════════════════════════════════════
let currentPhase = 'semana';
let currentGroup = 'A';

// ══════════════════════════════════════════════════════════
// NAVIGATION
// ══════════════════════════════════════════════════════════
function showView(id, e) {
  document.querySelectorAll('.view').forEach(v => v.classList.remove('active'));
  document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
  document.getElementById('view-' + id).classList.add('active');
  
  if (e && e.target) {
    e.target.classList.add('active');
  } else if (window.event && window.event.target) {
    window.event.target.classList.add('active');
  }
}

// ══════════════════════════════════════════════════════════
// RENDER: PHASE PILLS
// ══════════════════════════════════════════════════════════
function renderPhasePills() {
  const wrap = document.getElementById('phase-pills');
  wrap.innerHTML = DATA.phases.map(p => `
    <button class="phase-pill ${p.id === currentPhase ? 'active' : ''}" onclick="selectPhase('${p.id}')">
      ${p.label}
    </button>
  `).join('');
}

function selectPhase(id) {
  currentPhase = id;
  renderPhasePills();
  const isGroups = id === 'grupos';
  document.getElementById('group-selector-wrap').style.display = isGroups ? 'block' : 'none';
  updateResultsSubtitle();
  renderMatches();
}

function updateResultsSubtitle() {
  const el = document.getElementById('results-subtitle');
  if (currentPhase === 'semana') {
    el.textContent = `${DATA.currentWeek.label} · Hora CDMX · Resaltado: partidos en México`;
  } else {
    el.textContent = '72 partidos fase de grupos · 48 selecciones · 3 países sede';
  }
}

// ══════════════════════════════════════════════════════════
// RENDER: GROUP SELECTOR
// ══════════════════════════════════════════════════════════
function renderGroupSelector() {
  const wrap = document.getElementById('group-selector');
  wrap.innerHTML = DATA.groups.map(g => `
    <button class="grp-btn ${g === currentGroup ? 'active' : ''}" onclick="selectGroup('${g}')">
      ${g}
    </button>
  `).join('');
}

function selectGroup(g) {
  currentGroup = g;
  renderGroupSelector();
  renderMatches();
}

// ══════════════════════════════════════════════════════════
// RENDER: MATCHES
// ══════════════════════════════════════════════════════════
let pastVisible = false;
function togglePast() { pastVisible = !pastVisible; renderMatches(); }

function buildMatchCard(m, extraClass) {
  extraClass = extraClass || '';
  const isDone = m.status === 'done';
  const isLive = m.status === 'live';
  const hasScore = m.homeScore !== null && m.awayScore !== null;
  const isMexico = MEXICO_VENUES.some(v => m.venue && m.venue.includes(v));
  const scoreHTML = hasScore
    ? `<div class="score-block"><div class="score-box home ${isLive?'fire':''}">${m.homeScore}</div><div class="score-sep"><span>-</span></div><div class="score-box away ${isLive?'fire':''}">${m.awayScore}</div></div>`
    : `<div class="score-pending">${m.time} hrs</div>`;
  const statusLabel = isLive
    ? `<span class="match-status live-status">● En vivo</span>`
    : isDone ? `<span class="match-status done">✓ Finalizado</span>`
    : `<span class="match-status">${m.date}</span>`;
  const mexicoBadge = isMexico ? `<span class="mexico-badge">🇲🇽 México</span>` : '';
  return `<div class="match-card ${isLive?'live':''} ${isMexico?'mexico-venue':''} ${extraClass}">
    <div class="match-label-bar"><span class="match-label">${m.venue||''}${mexicoBadge}</span>${statusLabel}</div>
    <div class="match-inner">
      <div class="team-home"><span class="team-flag">${m.homeFlag}</span><div><div class="team-name">${m.home}</div><div class="team-abbr">${m.home.substring(0,3).toUpperCase()}</div></div></div>
      ${scoreHTML}
      <div class="team-away"><span class="team-flag">${m.awayFlag}</span><div><div class="team-name">${m.away}</div><div class="team-abbr">${m.away.substring(0,3).toUpperCase()}</div></div></div>
    </div></div>`;
}

function renderMatches() {
  const container = document.getElementById('matches-container');

  if (currentPhase === 'semana') {
    const weekStart = dateOnlyKey(DATA.currentWeek.startDate);
    const weekEnd   = dateOnlyKey(DATA.currentWeek.endDate);

    const pastMatches = DATA.matches
      .filter(m => m.status === 'done' && dateOnlyKey(m.date) < weekStart)
      .sort((a,b) => matchSortKey(a) - matchSortKey(b));

    const weekMatches = DATA.matches
      .filter(m => { const k = dateOnlyKey(m.date); return k >= weekStart && k <= weekEnd; })
      .sort((a,b) => matchSortKey(a) - matchSortKey(b));

    let html = '';

    if (pastMatches.length) {
      const btnLabel = pastVisible ? 'Ocultar ↑' : `Ver ${pastMatches.length} partidos anteriores ↓`;
      html += `<div class="past-section-toggle" onclick="togglePast()"><span class="past-section-label">Juegos Pasados</span><button class="past-toggle-btn">${btnLabel}</button></div>`;
      if (pastVisible) {
        let lastDate = null;
        pastMatches.forEach(m => {
          if (m.date !== lastDate) { html += `<div class="day-separator"><span class="day-separator-label" style="background:var(--ink3);">${m.date} <strong style="font-weight:900;letter-spacing:.14em;">${getDayName(m.date)}</strong></span></div>`; lastDate = m.date; }
          html += buildMatchCard(m, 'past-match-card');
        });
        html += `<div style="height:8px;"></div>`;
      }
    }

    if (!weekMatches.length) {
      html += `<div style="padding:30px;text-align:center;font-family:var(--font-mono);font-size:11px;color:var(--ink3);letter-spacing:.1em;text-transform:uppercase;">Sin partidos esta semana</div>`;
    } else {
      let lastDate = null;
      weekMatches.forEach(m => {
        if (m.date !== lastDate) { html += `<div class="day-separator"><span class="day-separator-label">${m.date} <strong style="font-weight:900;letter-spacing:.14em;">${getDayName(m.date)}</strong></span></div>`; lastDate = m.date; }
        html += buildMatchCard(m);
      });
    }
    container.innerHTML = html;
    return;
  }

  let filtered = DATA.matches.filter(m => m.phase === currentPhase);
  if (currentPhase === 'grupos') filtered = filtered.filter(m => m.group === currentGroup);
  filtered = [...filtered].sort((a,b) => matchSortKey(a) - matchSortKey(b));
  if (!filtered.length) {
    container.innerHTML = `<div style="padding:40px;text-align:center;font-family:var(--font-mono);font-size:11px;color:var(--ink3);letter-spacing:.1em;text-transform:uppercase;">Partidos por confirmar</div>`;
    return;
  }
  container.innerHTML = filtered.map(m => buildMatchCard(m)).join('');
}

// ══════════════════════════════════════════════════════════
// RENDER: STANDINGS
// ══════════════════════════════════════════════════════════
function renderStandings() {
  const container = document.getElementById('standings-container');
  const groupKeys = Object.keys(DATA.standings);

  container.innerHTML = groupKeys.map(g => {
    const teams = [...DATA.standings[g]].sort((a,b) => b.pts - a.pts || (b.gf - b.gc) - (a.gf - a.gc));
    const rows = teams.map((t, i) => {
      const dg = t.gf - t.gc;
      const dgStr = (dg > 0 ? '+' : '') + dg;
      let posClass = i < 2 ? 'pos-q2' : i === 2 ? 'pos-q3' : 'pos-out';
      return `
        <tr>
          <td>
            <div class="pos-row">
              <span class="pos-num">${i+1}</span>
              <span class="pos-indicator ${posClass}"></span>
              <div class="team-cell">
                <span class="team-cell-flag">${t.flag}</span>
                <span class="team-cell-name">${t.team}</span>
              </div>
            </div>
          </td>
          <td class="td-secondary">${t.pj}</td>
          <td class="td-secondary">${t.pg}</td>
          <td class="td-secondary">${t.pe}</td>
          <td class="td-secondary">${t.pp}</td>
          <td class="td-minor">${t.gf}</td>
          <td class="td-minor">${t.gc}</td>
          <td class="td-minor">${dgStr}</td>
          <td><span class="pts-cell">${t.pts}</span></td>
        </tr>
      `;
    }).join('');

    return `
      <div class="group-card">
        <div class="group-card-header">
          <span class="group-card-title">Grupo ${g}</span>
          <span class="group-card-detail">${teams[0].pj} / 3 jornadas</span>
        </div>
        <table class="standings-table">
          <thead><tr>
            <th style="width:42%">Selección</th>
            <th class="th-secondary">PJ</th>
            <th class="th-secondary">PG</th>
            <th class="th-secondary">PE</th>
            <th class="th-secondary">PP</th>
            <th class="th-minor">GF</th>
            <th class="th-minor">GC</th>
            <th class="th-minor">DG</th>
            <th style="color:var(--ink);font-weight:700;">PTS</th>
          </tr></thead>
          <tbody>${rows}</tbody>
        </table>
      </div>
    `;
  }).join('');
}

// ══════════════════════════════════════════════════════════
// RENDER: DYNAMIC KNOCKOUT BRACKET (123KLAN ESTILO)
// ══════════════════════════════════════════════════════════
function renderBracket() {
  const targetContainer = document.getElementById('bracket-render-container');
  const bracketPhases = [
    { id: 'dieciseisavos', label: 'Dieciseisavos' },
    { id: 'octavos',       label: 'Octavos' },
    { id: 'cuartos',       label: 'Cuartos' },
    { id: 'semis',         label: 'Semifinales' },
    { id: 'final',         label: 'Gran Final' }
  ];

  let bracketHTML = '';

  bracketPhases.forEach(phase => {
    let phaseMatches = DATA.matches.filter(m => m.phase === phase.id);
    
    bracketHTML += `<div class="bracket-column">`;
    bracketHTML += `<div class="bracket-column-title">${phase.label}</div>`;

    phaseMatches.forEach(m => {
      const isDone = m.status === 'done';
      const hasHomeWinner = isDone && (m.homeScore > m.awayScore);
      const hasAwayWinner = isDone && (m.awayScore > m.homeScore);
      const isScheduled = m.status === 'scheduled';

      bracketHTML += `
        <div class="bracket-match-node ${isScheduled ? 'unresolved' : ''}">
          <div class="bracket-node-header">
            <span class="bracket-node-id">M${m.id}</span>
            <span class="bracket-node-meta">${m.date} · ${m.time}</span>
          </div>
          <div class="bracket-node-team ${hasHomeWinner ? 'winner' : ''}">
            <span>${m.homeFlag || '⭐'} ${m.home}</span>
            <span class="bracket-node-score">${m.homeScore !== null ? m.homeScore : '—'}</span>
          </div>
          <div class="bracket-node-team ${hasAwayWinner ? 'winner' : ''}">
            <span>${m.awayFlag || '⭐'} ${m.away}</span>
            <span class="bracket-node-score">${m.awayScore !== null ? m.awayScore : '—'}</span>
          </div>
        </div>
      `;
    });

    bracketHTML += `</div>`;
  });

  targetContainer.innerHTML = bracketHTML;
}

// ══════════════════════════════════════════════════════════
// RENDER: STATS
// ══════════════════════════════════════════════════════════
const STATS_LIMIT = 10;
const statsExpanded = { scorers: false, yellow: false, red: false };

function renderStatsSection(listId, items, renderFn, expanded) {
  const limit = expanded ? items.length : Math.min(STATS_LIMIT, items.length);
  const visible = items.slice(0, limit);
  const hiddenCount = items.length - STATS_LIMIT;
  const hasMore = items.length > STATS_LIMIT;

  const rows = visible.map((item, i) => {
    const isExtra = i >= STATS_LIMIT;
    return isExtra
      ? `<div class="stats-fade-in" style="animation-delay:${(i - STATS_LIMIT) * 35}ms;">${renderFn(item, i)}</div>`
      : renderFn(item, i);
  }).join('');

  const btnContent = expanded
    ? `Mostrar menos <span style="display:inline-block;transform:translateY(-1px);">↑</span>`
    : `Mostrar más <span class="stats-more-badge">+${hiddenCount}</span>`;

  return rows +
    (hasMore ? `<div style="padding:10px 14px;border-top:1px solid var(--border);">
      <button onclick="toggleStats('${listId}')" class="stats-toggle-btn">${btnContent}</button>
    </div>` : '');
}

function toggleStats(listId) {
  const key = listId === 'scorers-list' ? 'scorers' : listId === 'yellow-list' ? 'yellow' : 'red';
  statsExpanded[key] = !statsExpanded[key];
  renderStats();
}

function renderStats() {
  const scorerFn = (s, i) => {
    const agTag = s.isOwnGoal
      ? `<span style="font-family:var(--font-mono);font-size:9px;background:var(--bg3);color:var(--ink3);padding:1px 5px;border-radius:2px;margin-left:4px;letter-spacing:.06em;">AG</span>`
      : '';
    return `<div class="scorer-row" style="${s.highlight ? 'background:var(--fire-light);' : s.isOwnGoal ? 'opacity:.75;' : ''}">
      <span class="scorer-rank ${(i < 3 || s.highlight) && !s.isOwnGoal ? 'top' : ''}">${i+1}</span>
      <div class="scorer-info">
        <div class="scorer-name">${s.flag} ${s.name}${agTag}</div>
        <div class="scorer-team">${s.team}</div>
      </div>
      <div style="text-align:right;">
        <div class="goals-num" style="${s.isOwnGoal ? 'color:var(--ink3);font-size:16px;' : ''}">${s.goals}</div>
        <div class="goals-label">${s.isOwnGoal ? 'autogol' : 'gol' + (s.goals !== 1 ? 'es' : '')}</div>
      </div>
    </div>`;
  };
  document.getElementById('scorers-list').innerHTML =
    renderStatsSection('scorers-list', DATA.scorers, scorerFn, statsExpanded.scorers);

  const yellowFn = c => `
    <div class="card-row" style="align-items:flex-start;">
      <span class="tarjeta tarjeta-amarilla" style="margin-top:2px;"></span>
      <div class="card-info">
        <div class="card-player">${c.flag} ${c.player}</div>
        <div class="card-team">${c.team}</div>
        ${c.min && c.min !== '—' ? `<div style="font-family:var(--font-body);font-size:11px;color:var(--ink2);margin-top:2px;">${c.min}</div>` : ''}
      </div>
    </div>`;
  document.getElementById('yellow-list').innerHTML =
    renderStatsSection('yellow-list', DATA.yellowCards, yellowFn, statsExpanded.yellow);

  if (!DATA.redCards.length) {
    document.getElementById('red-list').innerHTML =
      `<div style="padding:20px;text-align:center;font-family:var(--font-mono);font-size:10px;color:var(--ink3);letter-spacing:.08em;text-transform:uppercase;">Sin expulsados aún</div>`;
  } else {
    const redFn = c => `
      <div class="card-row" style="align-items:flex-start;">
        <span class="tarjeta tarjeta-roja" style="margin-top:2px;"></span>
        <div class="card-info">
          <div class="card-player">${c.flag} ${c.player}</div>
          <div class="card-team">${c.team}</div>
          <div style="font-family:var(--font-body);font-size:11px;color:var(--ink2);margin-top:3px;line-height:1.4;">${c.desc || ''}</div>
        </div>
        <span class="card-min" style="flex-shrink:0;">${c.min}</span>
      </div>`;
    document.getElementById('red-list').innerHTML =
      renderStatsSection('red-list', DATA.redCards, redFn, statsExpanded.red);
  }

  document.getElementById('crazy-numbers').innerHTML = DATA.crazyNumbers.map(n => `
    <div style="padding:10px 14px;border-bottom:1px solid var(--border);display:flex;align-items:center;gap:12px;">
      <div style="font-family:var(--font-display);font-weight:900;font-size:28px;color:var(--fire);line-height:1;flex-shrink:0;min-width:48px;text-align:center;">${n.num}</div>
      <div>
        <div style="font-family:var(--font-display);font-weight:700;font-size:13px;text-transform:uppercase;letter-spacing:.02em;color:var(--ink);">${n.label}</div>
        <div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;margin-top:2px;">${n.sub}</div>
      </div>
    </div>
  `).join('');
}

// ══════════════════════════════════════════════════════════
// RENDER: NOTICIAS
// ══════════════════════════════════════════════════════════
function renderNoticias() {
  document.getElementById('noticias-container').innerHTML = DATA.noticias.map(n => `
    <div class="noticia-card">
      <div class="noticia-accent ${n.accentColor}"></div>
      <div class="noticia-body">
        <div class="noticia-kicker ${n.kickerClass}">${n.kicker}</div>
        <div class="noticia-title">${n.title}</div>
        <div class="noticia-text">${n.text}</div>
        <div style="background:var(--bg2);border-radius:4px;padding:10px 12px;margin-bottom:14px;">
          <div style="font-family:var(--font-mono);font-size:9px;letter-spacing:.1em;text-transform:uppercase;color:var(--ink3);margin-bottom:4px;">⚡ Momento clave</div>
          <div style="font-family:var(--font-body);font-size:12px;color:var(--ink2);">${n.momento}</div>
          <div style="font-family:var(--font-mono);font-size:9px;letter-spacing:.1em;text-transform:uppercase;color:var(--ink3);margin:8px 0 4px;">📈 Impacto en clasificación</div>
          <div style="font-family:var(--font-body);font-size:12px;color:var(--ink2);">${n.impacto}</div>
        </div>
        <div class="noticia-footer">
          <div class="noticia-jugador">
            <span class="jugador-flag">${n.jugadorFlag}</span>
            <div>
              <div class="jugador-name">${n.jugadorName}</div>
              <div class="jugador-label">${n.jugadorLabel}</div>
            </div>
          </div>
          <div style="display:flex;gap:5px;flex-wrap:wrap;">
            ${n.tags.map(t => `<span class="noticia-tag">${t}</span>`).join('')}
          </div>
        </div>
      </div>
    </div>
  `).join('');
}

// ══════════════════════════════════════════════════════════
// RENDER: GDL VIEW
// ══════════════════════════════════════════════════════════
function renderGDL() {
  const sedes = [
    { key:'cdmx', label:'Partidos en Ciudad de México', estadio:'Estadio Ciudad de México', emoji:'🏟️', color:'#006847' },
    { key:'gdl',  label:'Partidos en Guadalajara',      estadio:'Estadio Guadalajara',      emoji:'⚽', color:'#FF4D1C' },
    { key:'mty',  label:'Partidos en Monterrey',        estadio:'Estadio Monterrey',         emoji:'🦁', color:'#D4A820' },
  ];

  function matchCard(m, estadio) {
    const hasScore = m.homeScore !== null && m.awayScore !== null;
    const isDone = m.status === 'done';
    const scoreHTML = hasScore
      ? `<div class="score-block">
           <div class="score-box home">${m.homeScore}</div>
           <div class="score-sep"><span>-</span></div>
           <div class="score-box away">${m.awayScore}</div>
         </div>`
      : `<div class="score-pending">${m.time} hrs</div>`;
    return `
      <div class="match-card mexico-venue">
        <div class="match-label-bar">
          <span class="match-label">${m.grupo} · ${estadio} <span class="mexico-badge">🇲🇽 México</span></span>
          <span class="match-status ${isDone ? 'done' : ''}">${isDone ? '✓ Finalizado' : m.date + ' · ' + m.time}</span>
        </div>
        <div class="match-inner">
          <div class="team-home">
            <span class="team-flag">${m.homeFlag}</span>
            <div>
              <div class="team-name">${m.home}</div>
              <div class="team-abbr">${m.home.substring(0,3).toUpperCase()}</div>
            </div>
          </div>
          ${scoreHTML}
          <div class="team-away">
            <span class="team-flag">${m.awayFlag}</span>
            <div>
              <div class="team-name">${m.away}</div>
              <div class="team-abbr">${m.away.substring(0,3).toUpperCase()}</div>
            </div>
          </div>
        </div>
      </div>`;
  }

  let html = '';
  sedes.forEach(s => {
    const ms = DATA.gdlMatches.filter(m => m.sede === s.key);
    if (!ms.length) return;
    html += `
      <div style="margin-bottom:24px;">
        <div style="display:flex;align-items:center;gap:10px;margin-bottom:10px;">
          <div style="width:4px;height:28px;background:${s.color};border-radius:2px;flex-shrink:0;"></div>
          <div>
            <div style="font-family:var(--font-display);font-weight:900;font-size:16px;text-transform:uppercase;letter-spacing:.06em;color:var(--ink);">${s.label}</div>
            <div style="font-family:var(--font-mono);font-size:10px;color:var(--ink3);letter-spacing:.08em;text-transform:uppercase;">${s.estadio} · ${ms.length} partido${ms.length !== 1 ? 's' : ''}</div>
          </div>
        </div>
        <div style="display:flex;flex-direction:column;gap:8px;">
          ${ms.map(m => matchCard(m, s.estadio)).join('')}
        </div>
      </div>`;
  });

  document.getElementById('gdl-matches').innerHTML = html;

  document.getElementById('eventos-container').innerHTML = DATA.eventos.map(e => `
    <div class="evento-card">
      <div class="evento-lateral" style="background:${e.categoriaColor}12;">
        <span class="evento-emoji">${e.emoji}</span>
        <span class="evento-acceso" style="background:${e.categoriaColor};">${e.acceso}</span>
      </div>
      <div class="evento-body">
        <div class="evento-cat" style="color:${e.categoriaColor};">${e.categoria}</div>
        <div class="evento-nombre">${e.nombre}</div>
        <div class="evento-meta">
          <span class="evento-meta-item">📅 ${e.fecha}</span>
          <span class="evento-meta-item">🕐 ${e.hora}</span>
          <span class="evento-meta-item">📍 ${e.lugar}</span>
        </div>
        ${e.nota ? `<div class="evento-nota">${e.nota}</div>` : ''}
      </div>
    </div>
  `).join('');

  document.getElementById('curiosidades-container').innerHTML = DATA.curiosidades.map(c => `
    <div style="background:var(--white);border:1.5px solid var(--border);border-radius:8px;padding:18px 20px;display:flex;gap:16px;align-items:flex-start;">
      <span style="font-size:28px;line-height:1;flex-shrink:0;">${c.emoji}</span>
      <div>
        <div style="font-family:var(--font-display);font-weight:800;font-size:16px;text-transform:uppercase;letter-spacing:.03em;color:var(--ink);margin-bottom:6px;">${c.titulo}</div>
        <div style="font-family:var(--font-body);font-size:13px;line-height:1.65;color:var(--ink2);">${c.texto}</div>
      </div>
    </div>
  `).join('');
}

// ══════════════════════════════════════════════════════════
// AQUÍ PEGAS TODO EL BLOQUE DEL PASO 5
// ═════════════════════════════════════════════════════════
function renderBracket() {
  const container = document.getElementById('bracket-render-container');
  // ... (resto del código de renderBracket)
}

function advanceTeam(matchId, side) {
  // ... (código de advanceTeam)
}

function manualZoomAdjust(val) {
  // ... (código de manualZoomAdjust)
}

function resetUserQuiniela() {
  // ... (código de resetUserQuiniela)
}

// Vincula el listener táctil de paneo
setTimeout(() => {
  const frameContainer = document.getElementById('canvas-container-scroll');
  // ... (resto del código del setTimeout táctil)
}, 400);
// ══════════════════════════════════════════════════════════
// INIT
// ══════════════════════════════════════════════════════════
function init() {
  renderPhasePills();
  renderGroupSelector();
  document.getElementById('group-selector-wrap').style.display = currentPhase === 'grupos' ? 'block' : 'none';
  updateResultsSubtitle();
  renderMatches();
  renderStandings();
  renderBracket(); //  renderStats();
  renderNoticias();
  renderGDL();
}

init();
</script>
</body>
</html>
