<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0, user-scalable=yes">
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
    <button class="nav-btn" onclick="showView('bracket', event)">Quiniela</button>
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
      <div class="section-title">¡Arma tu quiniela!</div>
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
    <div class="viewport-scaler-area" id="bracket-render-container"></div>
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
    <div class="stats-card"><div class="stats-card-header"><div class="stats-card-icon icon-fire">⚽</div><div><div class="stats-card-title">Top Goleadores</div><div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Fase de grupos</div></div></div><div class="stats-card-body" id="scorers-list"></div></div>
    <div class="stats-card"><div class="stats-card-header"><div class="stats-card-icon icon-yellow"><span class="tarjeta tarjeta-amarilla"></span></div><div><div class="stats-card-title">Tarjetas Amarillas</div><div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Por selección</div></div></div><div class="stats-card-body" id="yellow-list"></div></div>
    <div class="stats-card"><div class="stats-card-header"><div class="stats-card-icon icon-red"><span class="tarjeta tarjeta-roja"></span></div><div><div class="stats-card-title">Tarjetas Rojas</div><div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Expulsados del torneo</div></div></div><div class="stats-card-body" id="red-list"></div></div>
    <div class="stats-card"><div class="stats-card-header"><div class="stats-card-icon" style="background:var(--blue-light);font-size:16px;">📊</div><div><div class="stats-card-title">Números Locos</div><div style="font-family:var(--font-mono);font-size:9px;color:var(--ink3);letter-spacing:.06em;text-transform:uppercase;">Datos que no esperabas</div></div></div><div class="stats-card-body" id="crazy-numbers"></div></div>
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
  <div class="section-head"><div><div class="section-title">México <span>2026</span></div><div class="section-sub">3 ciudades sede · 3 estadios · El Mundial en casa</div></div></div>
  <div class="sedes-grid">
    <div class="gdl-hero sede-hero-gdl"><div class="gdl-hero-kicker">Estadio Guadalajara · 3 veces mundialista</div><div class="gdl-hero-title">Guadalajara <span>2026</span></div><div class="gdl-hero-text">La ciudad del mariachi, el tequila y el fútbol tapatío. 1970, 1986 y ahora 2026: el Estadio Guadalajara escribe el tercer capítulo de la historia.</div><div class="gdl-stats-row"><div class="gdl-stat"><span class="gdl-stat-num">4</span><span class="gdl-stat-label">Partidos</span></div><div class="gdl-stat"><span class="gdl-stat-num">3×</span><span class="gdl-stat-label">Mundialista</span></div><div class="gdl-stat"><span class="gdl-stat-num">49k</span><span class="gdl-stat-label">Capacidad</span></div></div></div>
    <div class="gdl-hero sede-hero-cdmx"><div class="gdl-hero-kicker">Estadio Ciudad de México · Leyenda viva</div><div class="gdl-hero-title">Ciudad de <span>México</span></div><div class="gdl-hero-text">El Estadio Azteca. La casa del Gol del Siglo. El recinto más icónico del fútbol mundial vuelve a ser el escenario más grande del torneo.</div><div class="gdl-stats-row"><div class="gdl-stat"><span class="gdl-stat-num">5</span><span class="gdl-stat-label">Partidos</span></div><div class="gdl-stat"><span class="gdl-stat-num">3×</span><span class="gdl-stat-label">Mundialista</span></div><div class="gdl-stat"><span class="gdl-stat-num">87k</span><span class="gdl-stat-label">Capacidad</span></div></div></div>
    <div class="gdl-hero sede-hero-mty"><div class="gdl-hero-kicker">Estadio Monterrey · La sultana del norte</div><div class="gdl-hero-title">Monterrey <span>2026</span></div><div class="gdl-hero-text">La ciudad más industrial y cosmopolita del norte de México entra al mapa mundial con el Estadio BBVA como escenario de lujo para el torneo.</div><div class="gdl-stats-row"><div class="gdl-stat"><span class="gdl-stat-num">4</span><span class="gdl-stat-label">Partidos</span></div><div class="gdl-stat"><span class="gdl-stat-num">1×</span><span class="gdl-stat-label">Mundialista</span></div><div class="gdl-stat"><span class="gdl-stat-num">53k</span><span class="gdl-stat-label">Capacidad</span></div></div></div>
  </div>
  <div class="section-head mt-20"><div class="section-title">Partidos en <span>México</span></div></div>
  <div class="gdl-matches-list" id="gdl-matches"></div>
  <div class="section-head mt-20"><div class="section-title">Eventos en <span>Guadalajara</span></div><div class="section-sub">Conciertos · Activaciones · Entretenimiento · Todos gratuitos</div></div>
  <div id="eventos-container" style="display:flex;flex-direction:column;gap:12px;"></div>
  <div class="section-head mt-20"><div class="section-title">Datos <span>Curiosos</span></div><div class="section-sub">Lo que no sabías de GDL y el Mundial</div></div>
  <div id="curiosidades-container" style="display:flex;flex-direction:column;gap:12px;"></div>
</div>

</main>

<footer class="site-footer">
  <div class="footer-inner" style="flex-direction:column; align-items:center; text-align:center; gap:6px;">
    <span class="footer-tagline">El corazón del juego</span>
    <span class="footer-copy">© 2026 · Datos: worldcup2026 API · NFOKU MKT</span>
  </div>
</footer>

<script>
const MEXICO_VENUES = ['Estadio Guadalajara', 'Estadio Ciudad de México', 'Estadio Monterrey'];
const MONTH_MAP = { Jun:6, Jul:7 };
const DAY_NAMES = ['DOM','LUN','MAR','MIÉ','JUE','VIE','SÁB'];

function getDayName(dateStr) {
  const parts = dateStr.split(' ');
  const day = parseInt(parts[0], 10);
  const month = (MONTH_MAP[parts[1]] || 6) - 1;
  return DAY_NAMES[new Date(2026, month, day).getDay()];
}

function matchSortKey(m) {
  const parts = m.date.split(' ');
  const day = parseInt(parts[0], 10) || 0;
  const month = MONTH_MAP[parts[1]] || 6;
  const timeStr = (m.time || '00:00').replace(' hrs','').split(':');
  return month * 100000 + day * 1000 + (parseInt(timeStr[0], 10) || 0) * 10;
}

function dateOnlyKey(dateStr) {
  const parts = dateStr.split(' ');
  return (MONTH_MAP[parts[1]] || 6) * 100 + (parseInt(parts[0], 10) || 0);
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
    { id:1,  phase:'grupos', group:'A', home:'México',        homeFlag:'🇲🇽', away:'Sudáfrica',     awayFlag:'🇿🇦', homeScore:2, awayScore:0, date:'11 Jun', time:'13:00', venue:'Estadio Ciudad de México', status:'done' },
    { id:2,  phase:'grupos', group:'A', home:'Rep. de Corea', homeFlag:'🇰🇷', away:'Rep. Checa',    awayFlag:'🇨🇿', homeScore:2, awayScore:1, date:'11 Jun', time:'20:00', venue:'Estadio Guadalajara',      status:'done' },
    { id:3,  phase:'grupos', group:'A', home:'Rep. Checa',    homeFlag:'🇨🇿', away:'Sudáfrica',     awayFlag:'🇿🇦', homeScore:1, awayScore:1, date:'18 Jun', time:'10:00', venue:'Estadio Atlanta',          status:'done' },
    { id:4,  phase:'grupos', group:'A', home:'México',        homeFlag:'🇲🇽', away:'Rep. de Corea', awayFlag:'🇰🇷', homeScore:1, awayScore:0, date:'18 Jun', time:'19:00', venue:'Estadio Guadalajara',      status:'done' },
    { id:5,  phase:'grupos', group:'A', home:'Rep. Checa',    homeFlag:'🇨🇿', away:'México',        awayFlag:'🇲🇽', homeScore:0, awayScore:3, date:'24 Jun', time:'19:00', venue:'Estadio Ciudad de México', status:'done' },
    { id:6,  phase:'grupos', group:'A', home:'Sudáfrica',     homeFlag:'🇿🇦', away:'Rep. de Corea', awayFlag:'🇰🇷', homeScore:1, awayScore:0, date:'24 Jun', time:'19:00', venue:'Estadio Monterrey',        status:'done' },
    { id:19, phase:'grupos', group:'D', home:'Estados Unidos', homeFlag:'🇺🇸', away:'Paraguay',       awayFlag:'🇵🇾', homeScore:4, awayScore:1, date:'12 Jun', time:'19:00', venue:'Estadio Los Ángeles',            status:'done' },
    { id:20, phase:'grupos', group:'D', home:'Australia',      homeFlag:'🇦🇺', away:'Turquía',        awayFlag:'🇹🇷', homeScore:2, awayScore:0, date:'13 Jun', time:'22:00', venue:'Estadio BC Place Vancouver',    status:'done' },
    { id:21, phase:'grupos', group:'D', home:'Estados Unidos', homeFlag:'🇺🇸', away:'Australia',      awayFlag:'🇦🇺', homeScore:2, awayScore:0, date:'19 Jun', time:'13:00', venue:'Estadio Seattle',               status:'done' },
    { id:22, phase:'grupos', group:'D', home:'Turquía',        homeFlag:'🇹🇷', away:'Paraguay',       awayFlag:'🇵🇾', homeScore:0, awayScore:1, date:'19 Jun', time:'22:00', venue:'Estadio Bahía de San Francisco', status:'done' },
    { id:23, phase:'grupos', group:'D', home:'Turquía',        homeFlag:'🇹🇷', away:'Estados Unidos', awayFlag:'🇺🇸', homeScore:3, awayScore:2, date:'25 Jun', time:'20:00', venue:'Estadio Los Ángeles',            status:'done' },
    { id:24, phase:'grupos', group:'D', home:'Paraguay',       homeFlag:'🇵🇾', away:'Australia',      awayFlag:'🇦🇺', homeScore:0, awayScore:0, date:'25 Jun', time:'20:00', venue:'Estadio Bahía de San Francisco', status:'done' },
    { id:25, phase:'grupos', group:'E', home:'Alemania',        homeFlag:'🇩🇪', away:'Curazao',        awayFlag:'🇨🇼', homeScore:7, awayScore:1, date:'14 Jun', time:'11:00', venue:'Estadio Houston',    status:'done' },
    { id:26, phase:'grupos', group:'E', home:'Costa de Marfil', homeFlag:'🇨🇮', away:'Ecuador',        awayFlag:'🇪🇨', homeScore:1, awayScore:0, date:'14 Jun', time:'17:00', venue:'Estadio Filadelfia', status:'done' },
    { id:27, phase:'grupos', group:'E', home:'Alemania',        homeFlag:'🇩🇪', away:'Costa de Marfil',awayFlag:'🇨🇮', homeScore:2, awayScore:1, date:'20 Jun', time:'14:00', venue:'Estadio Toronto',    status:'done' },
    { id:28, phase:'grupos', group:'E', home:'Ecuador',         homeFlag:'🇪🇨', away:'Curazao',        awayFlag:'🇨🇼', homeScore:0, awayScore:0, date:'20 Jun', time:'17:00', venue:'Estadio Kansas City', status:'done' },
    { id:29, phase:'grupos', group:'E', home:'Curazao',         homeFlag:'🇨🇼', away:'Costa de Marfil',awayFlag:'🇨🇮', homeScore:0, awayScore:2, date:'25 Jun', time:'14:00', venue:'Estadio Filadelfia', status:'done' },
    { id:30, phase:'grupos', group:'E', home:'Ecuador',         homeFlag:'🇪🇨', away:'Alemania',       awayFlag:'🇩🇪', homeScore:2, awayScore:1, date:'25 Jun', time:'14:00', venue:'Estadio Nueva York', status:'done' },
    { id:31, phase:'grupos', group:'F', home:'Países Bajos', homeFlag:'🇳🇱', away:'Japón',  awayFlag:'🇯🇵', homeScore:2, awayScore:2, date:'14 Jun', time:'14:00', venue:'Estadio Dallas',    status:'done' },
    { id:32, phase:'grupos', group:'F', home:'Suecia',       homeFlag:'🇸🇪', away:'Túnez',  awayFlag:'🇹🇳', homeScore:5, awayScore:1, date:'14 Jun', time:'20:00', venue:'Estadio Monterrey',  status:'done' },
    { id:33, phase:'grupos', group:'F', home:'Países Bajos', homeFlag:'🇳🇱', away:'Suecia', awayFlag:'🇸🇪', homeScore:5, awayScore:1, date:'20 Jun', time:'11:00', venue:'Estadio Houston',    status:'done' },
    { id:34, phase:'grupos', group:'F', home:'Túnez',        homeFlag:'🇹🇳', away:'Japón',  awayFlag:'🇯🇵', homeScore:0, awayScore:4, date:'20 Jun', time:'20:00', venue:'Estadio Monterrey',  status:'done' },
    { id:35, phase:'grupos', group:'F', home:'Túnez',        homeFlag:'🇹🇳', away:'Países Bajos', awayFlag:'🇳🇱', homeScore:1, awayScore:3, date:'25 Jun', time:'17:00', venue:'Estadio Kansas City', status:'done' },
    { id:36, phase:'grupos', group:'F', home:'Japón',        homeFlag:'🇯🇵', away:'Suecia', awayFlag:'🇸🇪', homeScore:1, awayScore:1, date:'25 Jun', time:'17:00', venue:'Estadio Dallas',    status:'done' },
    { id:41, phase:'grupos', group:'G', home:'Egipto',       homeFlag:'🇪🇬', away:'RI de Irán',   awayFlag:'🇮🇷', homeScore:1, awayScore:1, date:'26 Jun', time:'21:00', venue:'Estadio Seattle',            status:'done' },
    { id:42, phase:'grupos', group:'G', home:'Nueva Zelanda',homeFlag:'🇳🇿', away:'Bélgica',      awayFlag:'🇧🇪', homeScore:1, awayScore:5, date:'26 Jun', time:'21:00', venue:'Estadio Los Ángeles',        status:'done' },
    { id:47, phase:'grupos', group:'H', home:'Uruguay',       homeFlag:'🇺🇾', away:'España',         awayFlag:'🇪🇸', homeScore:0, awayScore:1, date:'26 Jun', time:'18:00', venue:'Estadio Guadalajara', status:'done' },
    { id:48, phase:'grupos', group:'H', home:'Cabo Verde',    homeFlag:'🇨🇻', away:'Arabia Saudita', awayFlag:'🇸🇦', homeScore:0, awayScore:0, date:'26 Jun', time:'18:00', venue:'Estadio Houston',  status:'done' },
    { id:53, phase:'grupos', group:'I', home:'Noruega',  homeFlag:'🇳🇴', away:'Francia', awayFlag:'🇫🇷', homeScore:1, awayScore:4, date:'26 Jun', time:'13:00', venue:'Estadio Boston',                status:'done' },
    { id:54, phase:'grupos', group:'I', home:'Senegal',  homeFlag:'🇸🇳', away:'Irak',    awayFlag:'🇮🇶', homeScore:5, awayScore:0, date:'26 Jun', time:'13:00', venue:'Estadio Toronto',               status:'done' },
    { id:59, phase:'grupos', group:'J', home:'Jordania',  homeFlag:'🇯🇴', away:'Argentina',awayFlag:'🇦🇷', homeScore:1, awayScore:3, date:'27 Jun', time:'20:00', venue:'Estadio Kansas City',           status:'done' },
    { id:60, phase:'grupos', group:'J', home:'Argelia',   homeFlag:'🇩🇿', away:'Austria',  awayFlag:'🇦🇹', homeScore:3, awayScore:3, date:'27 Jun', time:'20:00', venue:'Estadio Dallas',                status:'done' },
    { id:65, phase:'grupos', group:'K', home:'RD Congo',   homeFlag:'🇨🇩', away:'Uzbekistán', awayFlag:'🇺🇿', homeScore:3, awayScore:1, date:'27 Jun', time:'17:30', venue:'Estadio Atlanta',         status:'done' },
    { id:66, phase:'grupos', group:'K', home:'Colombia',   homeFlag:'🇨🇴', away:'Portugal',   awayFlag:'🇵🇹', homeScore:0, awayScore:0, date:'27 Jun', time:'17:30', venue:'Estadio Miami',            status:'done' },
    { id:71, phase:'grupos', group:'L', home:'Croacia',    homeFlag:'🇭🇷', away:'Ghana',   awayFlag:'🇬🇭', homeScore:2, awayScore:1, date:'27 Jun', time:'15:00', venue:'Estadio Filadelfia',  status:'done' },
    { id:72, phase:'grupos', group:'L', home:'Panamá',     homeFlag:'🇵🇦', away:'Inglaterra',awayFlag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', homeScore:0, awayScore:2, date:'27 Jun', time:'15:00', venue:'Estadio Nueva York', status:'done' },
    
    // ── DIECISEISAVOS DE FINAL
    { id:73, phase:'dieciseisavos', nextId:89, slot:'home', home:'Sudáfrica', homeFlag:'🇿🇦', away:'Canadá', awayFlag:'🇨🇦', homeScore:0, awayScore:1, status:'done', date:'28 Jun', time:'13:00', venue:'Estadio Los Ángeles' },
    { id:74, phase:'dieciseisavos', nextId:89, slot:'away', home:'Alemania', homeFlag:'🇩🇪', fav:'75%', away:'Paraguay', awayFlag:'🇵🇾', homeScore:null, awayScore:null, status:'scheduled', date:'29 Jun', time:'14:30', venue:'Estadio Boston' },
    { id:75, phase:'dieciseisavos', nextId:90, slot:'home', home:'Países Bajos', homeFlag:'🇳🇱', fav:'50%', away:'Marruecos', awayFlag:'🇲🇦', homeScore:null, awayScore:null, status:'scheduled', date:'29 Jun', time:'19:00', venue:'Estadio Monterrey' },
    { id:76, phase:'dieciseisavos', nextId:90, slot:'away', home:'Brasil', homeFlag:'🇧🇷', fav:'65%', away:'Japón', awayFlag:'🇯🇵', homeScore:null, awayScore:null, status:'scheduled', date:'29 Jun', time:'11:00', venue:'Estadio Houston' },
    { id:77, phase:'dieciseisavos', nextId:91, slot:'home', home:'Francia', homeFlag:'🇫🇷', fav:'80%', away:'Suecia', awayFlag:'🇸🇪', homeScore:null, awayScore:null, status:'scheduled', date:'30 Jun', time:'15:00', venue:'Estadio Nueva York' },
    { id:78, phase:'dieciseisavos', nextId:91, slot:'away', home:'Costa de Marfil', homeFlag:'🇨🇮', away:'Noruega', awayFlag:'🇳🇴', favAway:'56%', homeScore:null, awayScore:null, status:'scheduled', date:'30 Jun', time:'11:00', venue:'Estadio Dallas' },
    { id:79, phase:'dieciseisavos', nextId:92, slot:'home', home:'México', homeFlag:'🇲🇽', fav:'51%', away:'Ecuador', awayFlag:'🇪🇨', homeScore:null, awayScore:null, status:'scheduled', date:'30 Jun', time:'19:00', venue:'Estadio Ciudad de México' },
    { id:80, phase:'dieciseisavos', nextId:92, slot:'away', home:'Inglaterra', homeFlag:'🏴\u200d󠁢󠁥󠁮󠁧󠁿', fav:'80%', away:'RD Congo', awayFlag:'🇨🇩', homeScore:null, awayScore:null, status:'scheduled', date:'01 Jul', time:'10:00', venue:'Estadio Atlanta' },
    { id:81, phase:'dieciseisavos', nextId:93, slot:'home', home:'Estados Unidos', homeFlag:'🇺🇸', fav:'70%', away:'Bosnia', awayFlag:'🇧🇦', homeScore:null, awayScore:null, status:'scheduled', date:'01 Jul', time:'18:00', venue:'Estadio Bahía de San Francisco' },
    { id:82, phase:'dieciseisavos', nextId:93, slot:'away', home:'Bélgica', homeFlag:'🇧🇪', fav:'45%', away:'Senegal', awayFlag:'🇸🇳', homeScore:null, awayScore:null, status:'scheduled', date:'01 Jul', time:'14:00', venue:'Estadio Seattle' },
    { id:83, phase:'dieciseisavos', nextId:94, slot:'home', home:'Portugal', homeFlag:'🇵🇹', fav:'60%', away:'Croacia', awayFlag:'🇭🇷', homeScore:null, awayScore:null, status:'scheduled', date:'02 Jul', time:'17:00', venue:'Estadio Toronto' },
    { id:84, phase:'dieciseisavos', nextId:94, slot:'away', home:'España', homeFlag:'🇪🇸', fav:'80%', away:'Austria', awayFlag:'🇦🇹', homeScore:null, awayScore:null, status:'scheduled', date:'02 Jul', time:'13:00', venue:'Estadio Los Ángeles' },
    { id:85, phase:'dieciseisavos', nextId:95, slot:'home', home:'Suiza', homeFlag:'🇨🇭', fav:'55%', away:'Argelia', awayFlag:'🇩🇿', homeScore:null, awayScore:null, status:'scheduled', date:'02 Jul', time:'21:00', venue:'Estadio BC Place Vancouver' },
    { id:86, phase:'dieciseisavos', nextId:95, slot:'away', home:'Argentina', homeFlag:'🇦🇷', fav:'90%', away:'Cabo Verde', awayFlag:'🇨🇻', homeScore:null, awayScore:null, status:'scheduled', date:'03 Jul', time:'16:00', venue:'Estadio Miami' },
    { id:87, phase:'dieciseisavos', nextId:96, slot:'home', home:'Colombia', homeFlag:'🇨🇴', fav:'70%', away:'Ghana', awayFlag:'🇬🇭', homeScore:null, awayScore:null, status:'scheduled', date:'03 Jul', time:'19:30', venue:'Estadio Kansas City' },
    { id:88, phase:'dieciseisavos', nextId:96, slot:'away', home:'Australia', homeFlag:'🇦🇺', away:'Egipto', awayFlag:'🇪🇬', favAway:'45%', homeScore:null, awayScore:null, status:'scheduled', date:'03 Jul', time:'12:00', venue:'Estadio Dallas' },
    
    // ── OCTAVOS DE FINAL
    { id:89, phase:'octavos', nextId:97, slot:'home', home:'Canadá', homeFlag:'🇨🇦', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'04 Jul', time:'14:00', venue:'Estadio Filadelfia' },
    { id:90, phase:'octavos', nextId:97, slot:'away', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'04 Jul', time:'19:00', venue:'Estadio Houston' },
    { id:91, phase:'octavos', nextId:98, slot:'home', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'05 Jul', time:'14:00', venue:'Estadio Nueva York' },
    { id:92, phase:'octavos', nextId:98, slot:'away', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'05 Jul', time:'18:00', venue:'Estadio Ciudad de México' },
    { id:93, phase:'octavos', nextId:99, slot:'home', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'06 Jul', time:'18:00', venue:'Estadio Dallas' },
    { id:94, phase:'octavos', nextId:99, slot:'away', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'06 Jul', time:'15:00', venue:'Estadio Seattle' },
    { id:95, phase:'octavos', nextId:100, slot:'home', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'07 Jul', time:'10:00', venue:'Estadio Atlanta' },
    { id:96, phase:'octavos', nextId:100, slot:'away', home:'Por definir', homeFlag:'⭐', away:'Por definir', awayFlag:'⭐', homeScore:null, awayScore:null, status:'scheduled', date:'07 Jul', time:'14:00', venue:'Estadio BC Place Vancouver' },
    
    // ── CUARTOS DE FINAL
    { id:97, phase:'cuartos', nextId:101, slot:'home', home:'Ganador M89', homeFlag:'⚽', away:'Ganador M90', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'09 Jul', time:'13:00', venue:'Gillette Stadium, Boston' },
    { id:98, phase:'cuartos', nextId:101, slot:'away', home:'Ganador M91', homeFlag:'⚽', away:'Ganador M92', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'10 Jul', time:'14:00', venue:'SoFi Stadium, Los Ángeles' },
    { id:99, phase:'cuartos', nextId:102, slot:'home', home:'Ganador M93', homeFlag:'⚽', away:'Ganador M94', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'11 Jul', time:'14:00', venue:'Hard Rock Stadium, Miami' },
    { id:100, phase:'cuartos', nextId:102, slot:'away', home:'Ganador M95', homeFlag:'⚽', away:'Ganador M96', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'11 Jul', time:'18:00', venue:'Arrowhead Stadium, Kansas City' },
    
    // ── SEMIFINALES
    { id:101, phase:'semis', nextId:104, slot:'home', home:'Ganador Semis 1', homeFlag:'⚽', away:'Ganador Semis 2', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'14 Jul', time:'18:00', venue:'Estadio Dallas' },
    { id:102, phase:'semis', nextId:104, slot:'away', home:'Ganador Semis 3', homeFlag:'⚽', away:'Ganador Semis 4', awayFlag:'⚽', homeScore:null, awayScore:null, status:'scheduled', date:'15 Jul', time:'13:00', venue:'Estadio Atlanta' },
    
    // ── TERCER LUGAR Y GRAN FINAL
    { id:103, phase:'tercer-lugar', nextId:null, slot:null, home:'Perdedor Semi 1', homeFlag:'🥉', away:'Perdedor Semi 2', awayFlag:'🥉', homeScore:null, awayScore:null, status:'scheduled', date:'18 Jul', time:'13:00', venue:'Hard Rock Stadium, Miami' },
    { id:104, phase:'final', nextId:null, slot:null, home:'Finalista 1', homeFlag:'🌍', away:'Finalista 2', awayFlag:'🌍', homeScore:null, awayScore:null, status:'scheduled', date:'19 Jul', time:'13:00', venue:'Estadio Nueva York' }
  ],
  standings: {
    A: [{ team:'México', flag:'🇲🇽', pj:3, pg:3, pe:0, pp:0, gf:6, gc:0, pts:9 }, { team:'Sudáfrica', flag:'🇿🇦', pj:3, pg:1, pe:1, pp:1, gf:2, gc:3, pts:4 }, { team:'Rep. de Corea', flag:'🇰🇷', pj:3, pg:1, pe:0, pp:2, gf:2, gc:3, pts:3 }, { team:'Rep. Checa', flag:'🇨🇿', pj:3, pg:0, pe:1, pp:2, gf:2, gc:6, pts:1 }],
    B: [{ team:'Suiza', flag:'🇨🇭', pj:3, pg:2, pe:1, pp:0, gf:7, gc:2, pts:7 }, { team:'Canadá', flag:'🇨🇦', pj:3, pg:1, pe:1, pp:1, gf:7, gc:3, pts:4 }, { team:'Bosnia y Herzegovina', flag:'🇧🇦', pj:3, pg:1, pe:1, pp:1, gf:4, gc:6, pts:4 }, { team:'Catar', flag:'🇶🇦', pj:3, pg:0, pe:1, pp:2, gf:2, gc:9, pts:1 }],
    C: [{ team:'Marruecos', flag:'🇲🇦', pj:3, pg:2, pe:1, pp:0, gf:6, gc:3, pts:7 }, { team:'Brasil', flag:'🇧🇷', pj:3, pg:2, pe:1, pp:0, gf:7, gc:1, pts:7 }, { team:'Escocia', flag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', pj:3, pg:1, pe:0, pp:2, gf:1, gc:4, pts:3 }, { team:'Haití', flag:'🇭🇹', pj:3, pg:0, pe:0, pp:3, gf:2, gc:8, pts:0 }],
    D: [{ team:'Estados Unidos', flag:'🇺🇸', pj:3, pg:2, pe:0, pp:1, gf:8, gc:4, pts:6 }, { team:'Australia', flag:'🇦🇺', pj:3, pg:1, pe:1, pp:1, gf:2, gc:2, pts:4 }, { team:'Paraguay', flag:'🇵🇾', pj:3, pg:1, pe:1, pp:1, gf:2, gc:4, pts:4 }, { team:'Turquía', flag:'🇹🇷', pj:3, pg:1, pe:0, pp:2, gf:3, gc:5, pts:3 }],
    E: [{ team:'Alemania', flag:'🇩🇪', pj:3, pg:2, pe:0, pp:1, gf:10, gc:4, pts:6 }, { team:'Costa de Marfil', flag:'🇨🇮', pj:3, pg:2, pe:0, pp:1, gf:4, gc:2, pts:6 }, { team:'Ecuador', flag:'🇪🇨', pj:3, pg:1, pe:1, pp:1, gf:2, gc:2, pts:4 }, { team:'Curazao', flag:'🇨🇼', pj:3, pg:0, pe:1, pp:2, gf:1, gc:9, pts:1 }],
    F: [{ team:'Países Bajos', flag:'🇳🇱', pj:3, pg:2, pe:1, pp:0, gf:10, gc:4, pts:7 }, { team:'Japón', flag:'🇯🇵', pj:3, pg:1, pe:2, pp:0, gf:7, gc:3, pts:5 }, { team:'Suecia', flag:'🇸🇪', pj:3, pg:1, pe:1, pp:1, gf:7, gc:7, pts:4 }, { team:'Túnez', flag:'🇹🇳', pj:3, pg:0, pe:0, pp:3, gf:2, gc:12, pts:0 }],
    G: [{ team:'Bélgica', flag:'🇧🇪', pj:3, pg:1, pe:2, pp:0, gf:6, gc:2, pts:5 }, { team:'Egipto', flag:'🇪🇬', pj:3, pg:1, pe:2, pp:0, gf:5, gc:3, pts:5 }, { team:'RI de Irán', flag:'🇮🇷', pj:3, pg:0, pe:3, pp:0, gf:3, gc:3, pts:3 }, { team:'Nueva Zelanda', flag:'🇳🇿', pj:3, pg:0, pe:1, pp:2, gf:4, gc:10, pts:1 }],
    H: [{ team:'España', flag:'🇪🇸', pj:3, pg:2, pe:1, pp:0, gf:5, gc:0, pts:7 }, { team:'Cabo Verde', flag:'🇨🇻', pj:3, pg:0, pe:3, pp:0, gf:2, gc:2, pts:3 }, { team:'Uruguay', flag:'🇺🇾', pj:3, pg:0, pe:2, pp:1, gf:3, gc:4, pts:2 }, { team:'Arabia Saudita', flag:'🇸🇦', pj:3, pg:0, pe:2, pp:1, gf:1, gc:5, pts:2 }],
    I: [{ team:'Francia', flag:'🇫🇷', pj:3, pg:3, pe:0, pp:0, gf:10, gc:2, pts:9 }, { team:'Noruega', flag:'🇳🇴', pj:3, pg:2, pe:0, pp:1, gf:8, gc:7, pts:6 }, { team:'Senegal', flag:'🇸🇳', pj:3, pg:1, pe:0, pp:2, gf:8, gc:6, pts:3 }, { team:'Irak', flag:'🇮🇶', pj:3, pg:0, pe:0, pp:3, gf:1, gc:12, pts:0 }]
  },
  scorers: [
    { name:'Lionel Messi', team:'Argentina · Hat-Trick', flag:'🇦🇷', goals:6, highlight:true }
  ],
  yellowCards: [], redCards: [], crazyNumbers: [], noticias: []
};

// State inicial de vistas
let currentPhase = 'semana';
let currentGroup = 'A';

// ══════════════════════════════════════════════════════════
// INTERACTIVE BRACKET LOGIC
// ══════════════════════════════════════════════════════════
function renderBracket() {
  const container = document.getElementById('bracket-render-container');
  if(!container) return;
  const phases = ['dieciseisavos', 'octavos', 'cuartos', 'semis', 'tercer-lugar', 'final'];
  let html = '';

  phases.forEach(p => {
    let list = DATA.matches.filter(m => m.phase === p);
    let title = p === 'tercer-lugar' ? 'Tercer Lugar' : p === 'semis' ? 'Semifinal' : p;
    html += `<div class="bracket-column"><div class="bracket-column-title">${title}</div>`;
    
    list.forEach(m => {
      const isDone = m.status === 'done';
      const isHomeWin = isDone && m.homeScore > m.awayScore;
      const isAwayWin = isDone && m.awayScore > m.homeScore;
      const isPlaceholder = m.home.includes('Por definir') || m.home.includes('Ganador') || m.home.includes('Finalista') || m.home.includes('Perdedor');

      const homeFavTag = (m.fav && !isDone) ? `<span class="fav-badge">${m.fav}</span>` : '';
      const awayFavTag = (m.favAway && !isDone) ? `<span class="fav-badge">${m.favAway}</span>` : '';

      html += `
        <div class="bracket-match-node ${isPlaceholder ? 'unresolved-node' : ''}">
          <div class="node-info-row"><span class="node-match-id">M${m.id}</span><span>${m.date || '—'}</span></div>
          <div class="team-selectable-row ${isHomeWin ? 'selected-winner' : ''}" onclick="advanceTeam(${m.id}, 'home')">
            <span>${m.homeFlag || '⭐'} ${m.home} ${homeFavTag}</span>
            <span class="score-box-display">${m.homeScore !== null ? m.homeScore : '—'}</span>
          </div>
          <div class="team-selectable-row ${isAwayWin ? 'selected-winner' : ''}" onclick="advanceTeam(${m.id}, 'away')">
            <span>${m.awayFlag || '⭐'} ${m.away} ${awayFavTag}</span>
            <span class="score-box-display">${m.awayScore !== null ? m.awayScore : '—'}</span>
          </div>
        </div>`;
    });
    html += `</div>`;
  });
  container.innerHTML = html;
  container.style.transform = `scale(${globalScaleSetting})`;
}

function advanceTeam(matchId, side) {
  if(matchId === 73) return; 
  const m = DATA.matches.find(x => x.id === matchId);
  if(!m || m.home.includes('Por definir') || m.home.includes('Ganador') || m.home.includes('Finalista')) return;

  m.status = 'done';
  m.homeScore = side === 'home' ? 1 : 0;
  m.awayScore = side === 'home' ? 0 : 1;

  const winnerName = side === 'home' ? m.home : m.away;
  const winnerFlag = side === 'home' ? m.homeFlag : m.awayFlag;
  const loserName = side === 'home' ? m.away : m.home;
  const loserFlag = side === 'home' ? m.awayFlag : m.homeFlag;

  if (m.phase === 'semis') {
    const finalMatch = DATA.matches.find(x => x.phase === 'final');
    const thirdMatch = DATA.matches.find(x => x.phase === 'tercer-lugar');
    if(m.id === 101) {
      finalMatch.home = winnerName; finalMatch.homeFlag = winnerFlag;
      thirdMatch.home = loserName; thirdMatch.homeFlag = loserFlag;
    } else {
      finalMatch.away = winnerName; finalMatch.flagAway = winnerFlag;
      thirdMatch.away = loserName; thirdMatch.flagAway = loserFlag;
    }
  } else if(m.nextId) {
    const next = DATA.matches.find(x => x.id === m.nextId);
    if(next) {
      if(m.slot === 'home') { next.home = winnerName; next.homeFlag = winnerFlag; }
      else { next.away = winnerName; next.awayFlag = winnerFlag; }
    }
  }
  renderBracket();
}

function manualZoomAdjust(val) {
  globalScaleSetting = parseFloat(val);
  renderBracket();
}

function resetUserQuiniela() {
  DATA.matches.forEach(m => {
    if(m.id >= 73 && m.id !== 73) {
      m.homeScore = null; m.awayScore = null; m.status = 'scheduled';
      if(m.id >= 89) {
        m.home = m.id === 89 ? 'Canadá' : m.phase === 'octavos' ? 'Por definir' : 'Ganador M';
        m.homeFlag = m.id === 89 ? '🇨🇦' : '⭐';
        m.away = m.phase === 'octavos' ? 'Por definir' : 'Ganador M'; m.awayFlag = '⭐';
      }
    }
  });
  renderBracket();
}

// Vincula el listener táctil de paneo
setTimeout(() => {
  const frameContainer = document.getElementById('canvas-container-scroll');
  if(!frameContainer) return;
  let isDragging = false; let sx, sy, sLeft, sTop;

  const startPan = (e) => {
    isDragging = true;
    const x = e.pageX || e.touches[0].pageX;
    const y = e.pageY || e.touches[0].pageY;
    sx = x - frameContainer.offsetLeft;
    sy = y - frameContainer.offsetTop;
    sLeft = frameContainer.scrollLeft; sTop = frameContainer.scrollTop;
  };
  frameContainer.addEventListener('mousedown', startPan);
  frameContainer.addEventListener('touchstart', startPan);

  const movePan = (e) => {
    if(!isDragging) return;
    const x = e.pageX || e.touches[0].pageX;
    const y = e.pageY || e.touches[0].pageY;
    frameContainer.scrollLeft = sLeft - (x - frameContainer.offsetLeft - sx) * 1.4;
    frameContainer.scrollTop = sTop - (y - frameContainer.offsetTop - sy) * 1.4;
  };
  frameContainer.addEventListener('mousemove', movePan);
  frameContainer.addEventListener('touchmove', movePan);

  window.addEventListener('mouseup', () => isDragging = false);
  frameContainer.addEventListener('touchend', () => isDragging = false);
}, 400);

function renderStats() {}
function renderNoticias() {}
function renderGDL() {}

function init() {
  renderPhasePills();
  renderGroupSelector();
  const wrap = document.getElementById('group-selector-wrap');
  if (wrap) wrap.style.display = currentPhase === 'grupos' ? 'block' : 'none';
  updateResultsSubtitle();
  renderMatches();
  renderStandings();
  renderBracket();
  renderStats();
  renderNoticias();
  renderGDL();
}

init();
</script>
</body>
</html>
