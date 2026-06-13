<title>Mundial 2026 - Calendario</title>
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
  padding: 6px 8px;
  text-align: center;
  font-weight: 400;
  border-bottom: 1px solid var(--border);
}
.standings-table th:first-child { text-align: left; padding-left: 12px; }
.standings-table td {
  padding: 8px 8px;
  text-align: center;
  border-bottom: 1px solid var(--border);
  color: var(--ink2);
}
.standings-table td:first-child { text-align: left; padding-left: 12px; }
.standings-table tr:last-child td { border-bottom: none; }

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

/* ── FOOTER DECO SVG ── */
.footer-deco {
  position: relative;
  width: 100%;
  max-width: 1100px;
  margin: 0 auto 8px;
  height: 88px;
  overflow: hidden;
  border-bottom: 1px solid rgba(255,255,255,.07);
}
.footer-svg { width: 100%; height: 100%; display: block; }
</style>
</head>
<body>

<header class="site-header">
  <div class="header-inner">
    <div class="logo">
      <span class="logo-badge">Mundial FIFA 2026</span>
      <span class="logo-text"><span>¿</span>QUIÉN JUEGA HOY<span>?</span></span>
    </div>
    <div class="live-dot">En vivo</div>
  </div>
</header>

<nav class="main-nav">
  <div class="nav-inner">
    <button class="nav-btn active" onclick="showView('resultados')">Resultados</button>
    <button class="nav-btn" onclick="showView('posiciones')">Posiciones</button>
    <button class="nav-btn" onclick="showView('estadisticas')">Estadística Mundialista</button>
    <button class="nav-btn" onclick="showView('noticias')">Noticias</button>
    <button class="nav-btn" onclick="showView('gdl')">Guadalajara</button>
  </div>
</nav>

<main class="page">

<!-- ══════════════════════════════════════ VIEW: RESULTADOS -->
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

<!-- ══════════════════════════════════════ VIEW: POSICIONES -->
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

<!-- ══════════════════════════════════════ VIEW: ESTADÍSTICAS -->
<div id="view-estadisticas" class="view">
  <div class="section-head">
    <div>
      <div class="section-title">Estadística <span>Mundialista</span></div>
      <div class="section-sub">Goleadores · Tarjetas · Números que importan</div>
    </div>
  </div>

  <div class="stats-grid">
    <!-- Goleadores -->
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

    <!-- Tarjetas Amarillas -->
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

    <!-- Tarjetas Rojas -->
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

    <!-- Dato curioso estadístico -->
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

<!-- ══════════════════════════════════════ VIEW: NOTICIAS -->
<div id="view-noticias" class="view">
  <div class="section-head">
    <div>
      <div class="section-title">La <span>Crónica</span></div>
      <div class="section-sub">Periodismo deportivo · Al estilo de la calle</div>
    </div>
  </div>
  <div class="noticias-list" id="noticias-container"></div>
</div>

<!-- ══════════════════════════════════════ VIEW: GDL -->
<div id="view-gdl" class="view">
  <div class="gdl-hero">
    <div class="gdl-hero-kicker">Ciudad sede · 3 veces mundialista</div>
    <div class="gdl-hero-title">Guadalajara <span>2026</span></div>
    <div class="gdl-hero-text">La ciudad que vio nacer al mariachi, al tequila y a la chingonería mexicana vuelve a ser el centro del mundo. 1970, 1986 y ahora 2026: el Estadio Akron escribe el tercer capítulo de la historia.</div>
    <div class="gdl-stats-row">
      <div class="gdl-stat"><span class="gdl-stat-num">6</span><span class="gdl-stat-label">Partidos sede</span></div>
      <div class="gdl-stat"><span class="gdl-stat-num">3</span><span class="gdl-stat-label">Veces mundialista</span></div>
      <div class="gdl-stat"><span class="gdl-stat-num">49k</span><span class="gdl-stat-label">Capacidad Akron</span></div>
      <div class="gdl-stat"><span class="gdl-stat-num">39</span><span class="gdl-stat-label">Días de fiesta</span></div>
    </div>
  </div>

  <div class="section-head mt-20">
    <div class="section-title">Partidos en <span>Akron</span></div>
  </div>
  <div class="gdl-matches-list" id="gdl-matches"></div>

  <div class="section-head mt-20">
    <div class="section-title">Datos <span>Curiosos</span></div>
    <div class="section-sub">Lo que no sabías de GDL y el Mundial</div>
  </div>
  <div id="curiosidades-container" style="display:flex;flex-direction:column;gap:12px;"></div>
</div>

</main>

<footer class="site-footer">
  <!-- Decoración SVG estilo 123KLAN: plumas + serpiente emplumada sutil -->
  <div class="footer-deco" aria-hidden="true">
    <svg class="footer-svg" viewBox="0 0 1100 90" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet">
      <!-- Serpiente emplumada izquierda -->
      <g opacity="0.18" transform="translate(0,8)">
        <!-- cuerpo serpenteante -->
        <path d="M10,55 C30,20 60,70 90,35 C120,0 150,60 180,30 C200,10 215,40 225,30" stroke="#FF4D1C" stroke-width="5" fill="none" stroke-linecap="round"/>
        <!-- plumas izq -->
        <ellipse cx="30" cy="38" rx="10" ry="3" fill="#C8200A" transform="rotate(-45 30 38)"/>
        <ellipse cx="30" cy="38" rx="8" ry="2" fill="#7A7D82" transform="rotate(-30 30 38)"/>
        <ellipse cx="65" cy="52" rx="11" ry="3" fill="#C8200A" transform="rotate(40 65 52)"/>
        <ellipse cx="65" cy="52" rx="9" ry="2" fill="#7A7D82" transform="rotate(55 65 52)"/>
        <ellipse cx="100" cy="28" rx="10" ry="3" fill="#C8200A" transform="rotate(-50 100 28)"/>
        <ellipse cx="130" cy="48" rx="10" ry="3" fill="#C8200A" transform="rotate(35 130 48)"/>
        <ellipse cx="160" cy="22" rx="9" ry="2.5" fill="#7A7D82" transform="rotate(-40 160 22)"/>
        <!-- cabeza serpiente izq -->
        <polygon points="225,22 238,28 235,36 222,34" fill="#7A7D82"/>
        <circle cx="230" cy="26" r="2.5" fill="#FF4D1C"/>
        <!-- lengua bífida -->
        <path d="M238,29 L248,25 M238,29 L248,33" stroke="#C8200A" stroke-width="1.5" fill="none" stroke-linecap="round"/>
      </g>

      <!-- Plumas sueltas centro-izq -->
      <g opacity="0.14" transform="translate(260,0)">
        <ellipse cx="0" cy="40" rx="14" ry="4" fill="#C8200A" transform="rotate(-60 0 40)"/>
        <ellipse cx="0" cy="40" rx="11" ry="3" fill="#7A7D82" transform="rotate(-45 0 40)"/>
        <line x1="0" y1="26" x2="0" y2="54" stroke="#3A3A3A" stroke-width="1" opacity="0.5"/>

        <ellipse cx="28" cy="55" rx="12" ry="3.5" fill="#C8200A" transform="rotate(30 28 55)"/>
        <ellipse cx="28" cy="55" rx="9" ry="2.5" fill="#7A7D82" transform="rotate(45 28 55)"/>
        <line x1="28" y1="42" x2="28" y2="68" stroke="#3A3A3A" stroke-width="1" opacity="0.5"/>
      </g>

      <!-- Aguila geo centro (silueta angular estilo 123KLAN) -->
      <g opacity="0.22" transform="translate(490,2)">
        <!-- cuerpo angular del águila -->
        <polygon points="60,65 40,35 50,15 70,10 90,15 100,35 80,65" fill="#7A7D82"/>
        <!-- cabeza blanca del águila calva -->
        <polygon points="70,10 58,0 52,8 60,18 80,18 88,8 82,0" fill="#E8E4DB"/>
        <!-- ojo rojo -->
        <circle cx="62" cy="9" r="3" fill="#FF4D1C"/>
        <!-- pico angular -->
        <polygon points="52,12 44,18 52,20" fill="#D4A820"/>
        <!-- ala izquierda -->
        <polygon points="40,35 10,20 18,45 35,50 50,45" fill="#5A5D63"/>
        <polygon points="10,20 0,30 12,40 20,35" fill="#FF4D1C" opacity="0.7"/>
        <!-- ala derecha -->
        <polygon points="100,35 130,20 122,45 105,50 90,45" fill="#5A5D63"/>
        <!-- balón de fútbol integrado en el pecho -->
        <circle cx="70" cy="42" r="14" fill="#3A3D42" opacity="0.9"/>
        <path d="M64,30 L76,30 L82,40 L76,50 L64,50 L58,40 Z" fill="none" stroke="#E8E4DB" stroke-width="1.2" opacity="0.6"/>
        <path d="M70,28 L76,30" stroke="#E8E4DB" stroke-width="1" opacity="0.6"/>
        <path d="M70,54 L64,50" stroke="#E8E4DB" stroke-width="1" opacity="0.6"/>
        <!-- plumas cola rojAs -->
        <ellipse cx="55" cy="68" rx="13" ry="3" fill="#C8200A" transform="rotate(15 55 68)"/>
        <ellipse cx="70" cy="72" rx="14" ry="3.5" fill="#C8200A" transform="rotate(0 70 72)"/>
        <ellipse cx="85" cy="68" rx="13" ry="3" fill="#C8200A" transform="rotate(-15 85 68)"/>
        <ellipse cx="55" cy="68" rx="10" ry="2" fill="#7A7D82" transform="rotate(15 55 68)"/>
        <ellipse cx="70" cy="72" rx="11" ry="2.5" fill="#7A7D82" transform="rotate(0 70 72)"/>
        <ellipse cx="85" cy="68" rx="10" ry="2" fill="#7A7D82" transform="rotate(-15 85 68)"/>
        <!-- texto MUNDIAL sobre el águila -->
        <text x="70" y="-4" font-family="'Barlow Condensed', sans-serif" font-weight="900" font-size="10" fill="#3A3D42" text-anchor="middle" letter-spacing="3" opacity="0.7">MUNDIAL</text>
      </g>

      <!-- Plumas sueltas centro-der -->
      <g opacity="0.14" transform="translate(760,5)">
        <ellipse cx="0" cy="45" rx="13" ry="3.5" fill="#C8200A" transform="rotate(55 0 45)"/>
        <ellipse cx="0" cy="45" rx="10" ry="2.5" fill="#7A7D82" transform="rotate(70 0 45)"/>
        <line x1="-8" y1="35" x2="8" y2="55" stroke="#3A3A3A" stroke-width="1" opacity="0.5"/>

        <ellipse cx="30" cy="30" rx="12" ry="3" fill="#C8200A" transform="rotate(-35 30 30)"/>
        <ellipse cx="30" cy="30" rx="9" ry="2" fill="#7A7D82" transform="rotate(-20 30 30)"/>
        <line x1="22" y1="22" x2="38" y2="38" stroke="#3A3A3A" stroke-width="1" opacity="0.5"/>
      </g>

      <!-- Serpiente emplumada derecha (espejada) -->
      <g opacity="0.18" transform="translate(870,8)">
        <path d="M0,30 C10,10 40,50 70,25 C100,-5 130,55 160,30 C180,14 195,44 210,38" stroke="#FF4D1C" stroke-width="5" fill="none" stroke-linecap="round"/>
        <ellipse cx="30" cy="20" rx="10" ry="3" fill="#C8200A" transform="rotate(-45 30 20)"/>
        <ellipse cx="30" cy="20" rx="8" ry="2" fill="#7A7D82" transform="rotate(-30 30 20)"/>
        <ellipse cx="70" cy="42" rx="11" ry="3" fill="#C8200A" transform="rotate(35 70 42)"/>
        <ellipse cx="110" cy="18" rx="10" ry="3" fill="#C8200A" transform="rotate(-50 110 18)"/>
        <ellipse cx="150" cy="45" rx="9" ry="2.5" fill="#7A7D82" transform="rotate(40 150 45)"/>
        <!-- cabeza serpiente der -->
        <polygon points="0,22 -12,28 -9,36 2,34" fill="#7A7D82"/>
        <circle cx="-5" cy="26" r="2.5" fill="#FF4D1C"/>
        <path d="M-12,29 L-22,25 M-12,29 L-22,33" stroke="#C8200A" stroke-width="1.5" fill="none" stroke-linecap="round"/>
      </g>

      <!-- Maíz azteca izq (símbolo de las imágenes ref) -->
      <g opacity="0.13" transform="translate(200,15)">
        <ellipse cx="0" cy="0" rx="6" ry="18" fill="#D4A820"/>
        <circle cx="-3" cy="-8" r="2.5" fill="#C8200A" opacity="0.7"/>
        <circle cx="3"  cy="-5" r="2.5" fill="#C8200A" opacity="0.7"/>
        <circle cx="-3" cy="0"  r="2.5" fill="#C8200A" opacity="0.7"/>
        <circle cx="3"  cy="3"  r="2.5" fill="#C8200A" opacity="0.7"/>
        <circle cx="-3" cy="8"  r="2.5" fill="#C8200A" opacity="0.7"/>
        <path d="M0,-18 C-8,-25 -6,-32 0,-30 C6,-32 8,-25 0,-18" fill="#3B6D11" opacity="0.7"/>
      </g>

      <!-- Maíz azteca der -->
      <g opacity="0.13" transform="translate(860,20)">
        <ellipse cx="0" cy="0" rx="6" ry="18" fill="#D4A820"/>
        <circle cx="-3" cy="-8" r="2.5" fill="#C8200A" opacity="0.7"/>
        <circle cx="3"  cy="-5" r="2.5" fill="#C8200A" opacity="0.7"/>
        <circle cx="-3" cy="0"  r="2.5" fill="#C8200A" opacity="0.7"/>
        <circle cx="3"  cy="3"  r="2.5" fill="#C8200A" opacity="0.7"/>
        <circle cx="-3" cy="8"  r="2.5" fill="#C8200A" opacity="0.7"/>
        <path d="M0,-18 C-8,-25 -6,-32 0,-30 C6,-32 8,-25 0,-18" fill="#3B6D11" opacity="0.7"/>
      </g>
    </svg>
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
// Sedes en México (para resaltado especial)
const MEXICO_VENUES = ['Estadio Guadalajara', 'Estadio Ciudad de México', 'Estadio Monterrey'];

// Helper: convierte "11 Jun" + "13:00" en un valor numérico ordenable
const MONTH_MAP = { Jun:6, Jul:7 };
function matchSortKey(m) {
  const parts = m.date.split(' ');
  const day = parseInt(parts[0], 10) || 0;
  const month = MONTH_MAP[parts[1]] || 6;
  const timeStr = (m.time || '00:00').replace(' hrs','').split(':');
  const hh = parseInt(timeStr[0], 10) || 0;
  const mm = parseInt(timeStr[1], 10) || 0;
  return month * 100000 + day * 1000 + hh * 10 + (mm >= 30 ? 5 : 0);
}
// Helper: solo la parte de fecha (sin hora), para comparar contra rangos de semana
function dateOnlyKey(dateStr) {
  const parts = dateStr.split(' ');
  const day = parseInt(parts[0], 10) || 0;
  const month = MONTH_MAP[parts[1]] || 6;
  return month * 100 + day;
}

const DATA = {
  // Rango de la semana activa (lunes a domingo). Actualizar cada semana.
  currentWeek: { startDate: '11 Jun', endDate: '15 Jun', label: 'Semana del 11 al 15 de junio' },

  phases: [
    { id: 'semana', label: 'Esta Semana' },
    { id: 'grupos', label: 'Fase de Grupos' },
    { id: 'dieciseisavos', label: 'Dieciseisavos' },
    { id: 'cuartos', label: 'Cuartos de Final' },
    { id: 'semis', label: 'Semifinales' },
    { id: 'final', label: 'Final' },
  ],

  groups: ['A','B','C','D','E','F','G','H','I','J','K','L'],

  matches: [
    // ── GRUPO A: México · Sudáfrica · Rep. de Corea · Rep. Checa
    { id:1,  phase:'grupos', group:'A', home:'México',        homeFlag:'🇲🇽', away:'Sudáfrica',     awayFlag:'🇿🇦', homeScore:2, awayScore:0, date:'11 Jun', time:'13:00', venue:'Estadio Ciudad de México', status:'done' },
    { id:2,  phase:'grupos', group:'A', home:'Rep. de Corea', homeFlag:'🇰🇷', away:'Rep. Checa',    awayFlag:'🇨🇿', homeScore:2, awayScore:1, date:'11 Jun', time:'20:00', venue:'Estadio Guadalajara',      status:'done' },
    { id:3,  phase:'grupos', group:'A', home:'Rep. Checa',    homeFlag:'🇨🇿', away:'Sudáfrica',     awayFlag:'🇿🇦', homeScore:null, awayScore:null, date:'18 Jun', time:'10:00', venue:'Estadio Atlanta',          status:'scheduled' },
    { id:4,  phase:'grupos', group:'A', home:'México',        homeFlag:'🇲🇽', away:'Rep. de Corea', awayFlag:'🇰🇷', homeScore:null, awayScore:null, date:'18 Jun', time:'19:00', venue:'Estadio Guadalajara',      status:'scheduled' },
    { id:5,  phase:'grupos', group:'A', home:'Rep. Checa',    homeFlag:'🇨🇿', away:'México',        awayFlag:'🇲🇽', homeScore:null, awayScore:null, date:'24 Jun', time:'19:00', venue:'Estadio Ciudad de México', status:'scheduled' },
    { id:6,  phase:'grupos', group:'A', home:'Sudáfrica',     homeFlag:'🇿🇦', away:'Rep. de Corea', awayFlag:'🇰🇷', homeScore:null, awayScore:null, date:'24 Jun', time:'19:00', venue:'Estadio Monterrey',        status:'scheduled' },
    // ── GRUPO B: Canadá · Bosnia y Herzegovina · Catar · Suiza
    { id:7,  phase:'grupos', group:'B', home:'Canadá',               homeFlag:'🇨🇦', away:'Bosnia y Herzegovina', awayFlag:'🇧🇦', homeScore:1, awayScore:1, date:'12 Jun', time:'13:00', venue:'Estadio Toronto',               status:'done' },
    { id:8,  phase:'grupos', group:'B', home:'Catar',                homeFlag:'🇶🇦', away:'Suiza',                awayFlag:'🇨🇭', homeScore:null, awayScore:null, date:'13 Jun', time:'13:00', venue:'Estadio Bahía de San Francisco', status:'scheduled' },
    { id:9,  phase:'grupos', group:'B', home:'Suiza',                homeFlag:'🇨🇭', away:'Bosnia y Herzegovina', awayFlag:'🇧🇦', homeScore:null, awayScore:null, date:'18 Jun', time:'13:00', venue:'Estadio Los Ángeles',            status:'scheduled' },
    { id:10, phase:'grupos', group:'B', home:'Canadá',               homeFlag:'🇨🇦', away:'Catar',                awayFlag:'🇶🇦', homeScore:null, awayScore:null, date:'18 Jun', time:'16:00', venue:'Estadio BC Place Vancouver',    status:'scheduled' },
    { id:11, phase:'grupos', group:'B', home:'Suiza',                homeFlag:'🇨🇭', away:'Canadá',               awayFlag:'🇨🇦', homeScore:null, awayScore:null, date:'24 Jun', time:'13:00', venue:'Estadio BC Place Vancouver',    status:'scheduled' },
    { id:12, phase:'grupos', group:'B', home:'Bosnia y Herzegovina', homeFlag:'🇧🇦', away:'Catar',                awayFlag:'🇶🇦', homeScore:null, awayScore:null, date:'24 Jun', time:'13:00', venue:'Estadio Seattle',               status:'scheduled' },
    // ── GRUPO C: Brasil · Marruecos · Haití · Escocia
    { id:13, phase:'grupos', group:'C', home:'Brasil',    homeFlag:'🇧🇷', away:'Marruecos', awayFlag:'🇲🇦', homeScore:null, awayScore:null, date:'13 Jun', time:'16:00', venue:'Estadio Nueva York',            status:'scheduled' },
    { id:14, phase:'grupos', group:'C', home:'Haití',     homeFlag:'🇭🇹', away:'Escocia',   awayFlag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', homeScore:null, awayScore:null, date:'13 Jun', time:'19:00', venue:'Estadio Boston',                status:'scheduled' },
    { id:15, phase:'grupos', group:'C', home:'Escocia',   homeFlag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', away:'Marruecos', awayFlag:'🇲🇦', homeScore:null, awayScore:null, date:'19 Jun', time:'16:00', venue:'Estadio Boston',                status:'scheduled' },
    { id:16, phase:'grupos', group:'C', home:'Brasil',    homeFlag:'🇧🇷', away:'Haití',     awayFlag:'🇭🇹', homeScore:null, awayScore:null, date:'19 Jun', time:'18:30', venue:'Estadio Filadelfia',            status:'scheduled' },
    { id:17, phase:'grupos', group:'C', home:'Marruecos', homeFlag:'🇲🇦', away:'Haití',     awayFlag:'🇭🇹', homeScore:null, awayScore:null, date:'24 Jun', time:'16:00', venue:'Estadio Atlanta',               status:'scheduled' },
    { id:18, phase:'grupos', group:'C', home:'Escocia',   homeFlag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', away:'Brasil',    awayFlag:'🇧🇷', homeScore:null, awayScore:null, date:'24 Jun', time:'16:00', venue:'Estadio Miami',                 status:'scheduled' },
    // ── GRUPO D: Estados Unidos · Paraguay · Australia · Turquía
    { id:19, phase:'grupos', group:'D', home:'Estados Unidos', homeFlag:'🇺🇸', away:'Paraguay',       awayFlag:'🇵🇾', homeScore:null, awayScore:null, date:'12 Jun', time:'19:00', venue:'Estadio Los Ángeles',            status:'scheduled' },
    { id:20, phase:'grupos', group:'D', home:'Australia',      homeFlag:'🇦🇺', away:'Turquía',        awayFlag:'🇹🇷', homeScore:null, awayScore:null, date:'13 Jun', time:'22:00', venue:'Estadio BC Place Vancouver',    status:'scheduled' },
    { id:21, phase:'grupos', group:'D', home:'Estados Unidos', homeFlag:'🇺🇸', away:'Australia',      awayFlag:'🇦🇺', homeScore:null, awayScore:null, date:'19 Jun', time:'13:00', venue:'Estadio Seattle',               status:'scheduled' },
    { id:22, phase:'grupos', group:'D', home:'Turquía',        homeFlag:'🇹🇷', away:'Paraguay',       awayFlag:'🇵🇾', homeScore:null, awayScore:null, date:'19 Jun', time:'22:00', venue:'Estadio Bahía de San Francisco', status:'scheduled' },
    { id:23, phase:'grupos', group:'D', home:'Turquía',        homeFlag:'🇹🇷', away:'Estados Unidos', awayFlag:'🇺🇸', homeScore:null, awayScore:null, date:'25 Jun', time:'20:00', venue:'Estadio Los Ángeles',            status:'scheduled' },
    { id:24, phase:'grupos', group:'D', home:'Paraguay',       homeFlag:'🇵🇾', away:'Australia',      awayFlag:'🇦🇺', homeScore:null, awayScore:null, date:'25 Jun', time:'20:00', venue:'Estadio Bahía de San Francisco', status:'scheduled' },
    // ── GRUPO E: Alemania · Curazao · Costa de Marfil · Ecuador
    { id:25, phase:'grupos', group:'E', home:'Alemania',        homeFlag:'🇩🇪', away:'Curazao',        awayFlag:'🇨🇼', homeScore:null, awayScore:null, date:'14 Jun', time:'11:00', venue:'Estadio Houston',    status:'scheduled' },
    { id:26, phase:'grupos', group:'E', home:'Costa de Marfil', homeFlag:'🇨🇮', away:'Ecuador',        awayFlag:'🇪🇨', homeScore:null, awayScore:null, date:'14 Jun', time:'17:00', venue:'Estadio Filadelfia', status:'scheduled' },
    { id:27, phase:'grupos', group:'E', home:'Alemania',        homeFlag:'🇩🇪', away:'Costa de Marfil',awayFlag:'🇨🇮', homeScore:null, awayScore:null, date:'20 Jun', time:'14:00', venue:'Estadio Toronto',    status:'scheduled' },
    { id:28, phase:'grupos', group:'E', home:'Ecuador',         homeFlag:'🇪🇨', away:'Curazao',        awayFlag:'🇨🇼', homeScore:null, awayScore:null, date:'20 Jun', time:'17:00', venue:'Estadio Kansas City', status:'scheduled' },
    { id:29, phase:'grupos', group:'E', home:'Curazao',         homeFlag:'🇨🇼', away:'Costa de Marfil',awayFlag:'🇨🇮', homeScore:null, awayScore:null, date:'25 Jun', time:'14:00', venue:'Estadio Filadelfia', status:'scheduled' },
    { id:30, phase:'grupos', group:'E', home:'Ecuador',         homeFlag:'🇪🇨', away:'Alemania',       awayFlag:'🇩🇪', homeScore:null, awayScore:null, date:'25 Jun', time:'14:00', venue:'Estadio Nueva York', status:'scheduled' },
    // ── GRUPO F: Países Bajos · Japón · Suecia · Túnez
    { id:31, phase:'grupos', group:'F', home:'Países Bajos', homeFlag:'🇳🇱', away:'Japón',  awayFlag:'🇯🇵', homeScore:null, awayScore:null, date:'14 Jun', time:'14:00', venue:'Estadio Dallas',    status:'scheduled' },
    { id:32, phase:'grupos', group:'F', home:'Suecia',       homeFlag:'🇸🇪', away:'Túnez',  awayFlag:'🇹🇳', homeScore:null, awayScore:null, date:'14 Jun', time:'20:00', venue:'Estadio Monterrey',  status:'scheduled' },
    { id:33, phase:'grupos', group:'F', home:'Países Bajos', homeFlag:'🇳🇱', away:'Suecia', awayFlag:'🇸🇪', homeScore:null, awayScore:null, date:'20 Jun', time:'11:00', venue:'Estadio Houston',    status:'scheduled' },
    { id:34, phase:'grupos', group:'F', home:'Túnez',        homeFlag:'🇹🇳', away:'Japón',  awayFlag:'🇯🇵', homeScore:null, awayScore:null, date:'20 Jun', time:'20:00', venue:'Estadio Monterrey',  status:'scheduled' },
    { id:35, phase:'grupos', group:'F', home:'Túnez',        homeFlag:'🇹🇳', away:'Países Bajos', awayFlag:'🇳🇱', homeScore:null, awayScore:null, date:'25 Jun', time:'17:00', venue:'Estadio Kansas City', status:'scheduled' },
    { id:36, phase:'grupos', group:'F', home:'Japón',        homeFlag:'🇯🇵', away:'Suecia', awayFlag:'🇸🇪', homeScore:null, awayScore:null, date:'25 Jun', time:'17:00', venue:'Estadio Dallas',    status:'scheduled' },
    // ── GRUPO G: Bélgica · Egipto · RI de Irán · Nueva Zelanda
    { id:37, phase:'grupos', group:'G', home:'Bélgica',      homeFlag:'🇧🇪', away:'Egipto',       awayFlag:'🇪🇬', homeScore:null, awayScore:null, date:'15 Jun', time:'13:00', venue:'Estadio Seattle',            status:'scheduled' },
    { id:38, phase:'grupos', group:'G', home:'RI de Irán',   homeFlag:'🇮🇷', away:'Nueva Zelanda', awayFlag:'🇳🇿', homeScore:null, awayScore:null, date:'15 Jun', time:'19:00', venue:'Estadio Los Ángeles',        status:'scheduled' },
    { id:39, phase:'grupos', group:'G', home:'Bélgica',      homeFlag:'🇧🇪', away:'RI de Irán',   awayFlag:'🇮🇷', homeScore:null, awayScore:null, date:'21 Jun', time:'13:00', venue:'Estadio Los Ángeles',        status:'scheduled' },
    { id:40, phase:'grupos', group:'G', home:'Nueva Zelanda',homeFlag:'🇳🇿', away:'Egipto',       awayFlag:'🇪🇬', homeScore:null, awayScore:null, date:'21 Jun', time:'19:00', venue:'Estadio BC Place Vancouver',  status:'scheduled' },
    { id:41, phase:'grupos', group:'G', home:'Egipto',       homeFlag:'🇪🇬', away:'RI de Irán',   awayFlag:'🇮🇷', homeScore:null, awayScore:null, date:'26 Jun', time:'21:00', venue:'Estadio Seattle',            status:'scheduled' },
    { id:42, phase:'grupos', group:'G', home:'Nueva Zelanda',homeFlag:'🇳🇿', away:'Bélgica',      awayFlag:'🇧🇪', homeScore:null, awayScore:null, date:'26 Jun', time:'21:00', venue:'Estadio Los Ángeles',        status:'scheduled' },
    // ── GRUPO H: España · Cabo Verde · Arabia Saudita · Uruguay
    { id:43, phase:'grupos', group:'H', home:'España',        homeFlag:'🇪🇸', away:'Cabo Verde',     awayFlag:'🇨🇻', homeScore:null, awayScore:null, date:'15 Jun', time:'10:00', venue:'Estadio Atlanta',  status:'scheduled' },
    { id:44, phase:'grupos', group:'H', home:'Arabia Saudita',homeFlag:'🇸🇦', away:'Uruguay',        awayFlag:'🇺🇾', homeScore:null, awayScore:null, date:'15 Jun', time:'16:00', venue:'Estadio Miami',    status:'scheduled' },
    { id:45, phase:'grupos', group:'H', home:'España',        homeFlag:'🇪🇸', away:'Arabia Saudita', awayFlag:'🇸🇦', homeScore:null, awayScore:null, date:'21 Jun', time:'10:00', venue:'Estadio Atlanta',  status:'scheduled' },
    { id:46, phase:'grupos', group:'H', home:'Uruguay',       homeFlag:'🇺🇾', away:'Cabo Verde',     awayFlag:'🇨🇻', homeScore:null, awayScore:null, date:'21 Jun', time:'16:00', venue:'Estadio Miami',    status:'scheduled' },
    { id:47, phase:'grupos', group:'H', home:'Uruguay',       homeFlag:'🇺🇾', away:'España',         awayFlag:'🇪🇸', homeScore:null, awayScore:null, date:'26 Jun', time:'18:00', venue:'Estadio Guadalajara', status:'scheduled' },
    { id:48, phase:'grupos', group:'H', home:'Cabo Verde',    homeFlag:'🇨🇻', away:'Arabia Saudita', awayFlag:'🇸🇦', homeScore:null, awayScore:null, date:'26 Jun', time:'18:00', venue:'Estadio Houston',  status:'scheduled' },
    // ── GRUPO I: Francia · Senegal · Irak · Noruega
    { id:49, phase:'grupos', group:'I', home:'Francia',  homeFlag:'🇫🇷', away:'Senegal', awayFlag:'🇸🇳', homeScore:null, awayScore:null, date:'16 Jun', time:'13:00', venue:'Estadio Nueva York',            status:'scheduled' },
    { id:50, phase:'grupos', group:'I', home:'Irak',     homeFlag:'🇮🇶', away:'Noruega', awayFlag:'🇳🇴', homeScore:null, awayScore:null, date:'16 Jun', time:'16:00', venue:'Estadio Boston',                status:'scheduled' },
    { id:51, phase:'grupos', group:'I', home:'Francia',  homeFlag:'🇫🇷', away:'Irak',    awayFlag:'🇮🇶', homeScore:null, awayScore:null, date:'22 Jun', time:'15:00', venue:'Estadio Filadelfia',            status:'scheduled' },
    { id:52, phase:'grupos', group:'I', home:'Noruega',  homeFlag:'🇳🇴', away:'Senegal', awayFlag:'🇸🇳', homeScore:null, awayScore:null, date:'22 Jun', time:'18:00', venue:'Estadio Nueva York',            status:'scheduled' },
    { id:53, phase:'grupos', group:'I', home:'Noruega',  homeFlag:'🇳🇴', away:'Francia', awayFlag:'🇫🇷', homeScore:null, awayScore:null, date:'26 Jun', time:'13:00', venue:'Estadio Boston',                status:'scheduled' },
    { id:54, phase:'grupos', group:'I', home:'Senegal',  homeFlag:'🇸🇳', away:'Irak',    awayFlag:'🇮🇶', homeScore:null, awayScore:null, date:'26 Jun', time:'13:00', venue:'Estadio Toronto',               status:'scheduled' },
    // ── GRUPO J: Argentina · Argelia · Austria · Jordania
    { id:55, phase:'grupos', group:'J', home:'Argentina', homeFlag:'🇦🇷', away:'Argelia',  awayFlag:'🇩🇿', homeScore:null, awayScore:null, date:'16 Jun', time:'19:00', venue:'Estadio Kansas City',           status:'scheduled' },
    { id:56, phase:'grupos', group:'J', home:'Austria',   homeFlag:'🇦🇹', away:'Jordania', awayFlag:'🇯🇴', homeScore:null, awayScore:null, date:'16 Jun', time:'22:00', venue:'Estadio Bahía de San Francisco', status:'scheduled' },
    { id:57, phase:'grupos', group:'J', home:'Argentina', homeFlag:'🇦🇷', away:'Austria',  awayFlag:'🇦🇹', homeScore:null, awayScore:null, date:'22 Jun', time:'11:00', venue:'Estadio Dallas',                status:'scheduled' },
    { id:58, phase:'grupos', group:'J', home:'Jordania',  homeFlag:'🇯🇴', away:'Argelia',  awayFlag:'🇩🇿', homeScore:null, awayScore:null, date:'22 Jun', time:'21:00', venue:'Estadio Bahía de San Francisco', status:'scheduled' },
    { id:59, phase:'grupos', group:'J', home:'Jordania',  homeFlag:'🇯🇴', away:'Argentina',awayFlag:'🇦🇷', homeScore:null, awayScore:null, date:'27 Jun', time:'20:00', venue:'Estadio Kansas City',           status:'scheduled' },
    { id:60, phase:'grupos', group:'J', home:'Argelia',   homeFlag:'🇩🇿', away:'Austria',  awayFlag:'🇦🇹', homeScore:null, awayScore:null, date:'27 Jun', time:'20:00', venue:'Estadio Dallas',                status:'scheduled' },
    // ── GRUPO K: Portugal · RD Congo · Uzbekistán · Colombia
    { id:61, phase:'grupos', group:'K', home:'Portugal',   homeFlag:'🇵🇹', away:'RD Congo',   awayFlag:'🇨🇩', homeScore:null, awayScore:null, date:'17 Jun', time:'11:00', venue:'Estadio Houston',         status:'scheduled' },
    { id:62, phase:'grupos', group:'K', home:'Uzbekistán', homeFlag:'🇺🇿', away:'Colombia',   awayFlag:'🇨🇴', homeScore:null, awayScore:null, date:'17 Jun', time:'20:00', venue:'Estadio Ciudad de México', status:'scheduled' },
    { id:63, phase:'grupos', group:'K', home:'Portugal',   homeFlag:'🇵🇹', away:'Uzbekistán', awayFlag:'🇺🇿', homeScore:null, awayScore:null, date:'23 Jun', time:'11:00', venue:'Estadio Houston',         status:'scheduled' },
    { id:64, phase:'grupos', group:'K', home:'Colombia',   homeFlag:'🇨🇴', away:'RD Congo',   awayFlag:'🇨🇩', homeScore:null, awayScore:null, date:'23 Jun', time:'20:00', venue:'Estadio Guadalajara',     status:'scheduled' },
    { id:65, phase:'grupos', group:'K', home:'RD Congo',   homeFlag:'🇨🇩', away:'Uzbekistán', awayFlag:'🇺🇿', homeScore:null, awayScore:null, date:'27 Jun', time:'17:30', venue:'Estadio Atlanta',         status:'scheduled' },
    { id:66, phase:'grupos', group:'K', home:'Colombia',   homeFlag:'🇨🇴', away:'Portugal',   awayFlag:'🇵🇹', homeScore:null, awayScore:null, date:'27 Jun', time:'17:30', venue:'Estadio Miami',           status:'scheduled' },
    // ── GRUPO L: Inglaterra · Croacia · Ghana · Panamá
    { id:67, phase:'grupos', group:'L', home:'Inglaterra', homeFlag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', away:'Croacia', awayFlag:'🇭🇷', homeScore:null, awayScore:null, date:'17 Jun', time:'14:00', venue:'Estadio Dallas',     status:'scheduled' },
    { id:68, phase:'grupos', group:'L', home:'Ghana',      homeFlag:'🇬🇭', away:'Panamá',  awayFlag:'🇵🇦', homeScore:null, awayScore:null, date:'17 Jun', time:'17:00', venue:'Estadio Toronto',    status:'scheduled' },
    { id:69, phase:'grupos', group:'L', home:'Inglaterra', homeFlag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', away:'Ghana',  awayFlag:'🇬🇭', homeScore:null, awayScore:null, date:'23 Jun', time:'14:00', venue:'Estadio Boston',     status:'scheduled' },
    { id:70, phase:'grupos', group:'L', home:'Panamá',     homeFlag:'🇵🇦', away:'Croacia', awayFlag:'🇭🇷', homeScore:null, awayScore:null, date:'23 Jun', time:'17:00', venue:'Estadio Toronto',    status:'scheduled' },
    { id:71, phase:'grupos', group:'L', home:'Croacia',    homeFlag:'🇭🇷', away:'Ghana',   awayFlag:'🇬🇭', homeScore:null, awayScore:null, date:'27 Jun', time:'15:00', venue:'Estadio Monterrey',  status:'scheduled' },
    { id:72, phase:'grupos', group:'L', home:'Panamá',     homeFlag:'🇵🇦', away:'Inglaterra',awayFlag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', homeScore:null, awayScore:null, date:'27 Jun', time:'15:00', venue:'Estadio Filadelfia', status:'scheduled' },
    // ── DIECISEISAVOS DE FINAL
    { id:73,  phase:'dieciseisavos', group:null, home:'2° Grupo A', homeFlag:'🥈', away:'2° Grupo B', awayFlag:'🥈', homeScore:null, awayScore:null, date:'28 Jun', time:'19:00', venue:'Estadio Los Ángeles',            status:'scheduled' },
    { id:74,  phase:'dieciseisavos', group:null, home:'1° Grupo E', homeFlag:'🏆', away:'3° A/B/C/D/F',awayFlag:'⭐', homeScore:null, awayScore:null, date:'29 Jun', time:'13:00', venue:'Estadio Boston',                status:'scheduled' },
    { id:75,  phase:'dieciseisavos', group:null, home:'1° Grupo F', homeFlag:'🏆', away:'2° Grupo C',  awayFlag:'🥈', homeScore:null, awayScore:null, date:'29 Jun', time:'18:00', venue:'Estadio Monterrey',              status:'scheduled' },
    { id:76,  phase:'dieciseisavos', group:null, home:'1° Grupo C', homeFlag:'🏆', away:'2° Grupo F',  awayFlag:'🥈', homeScore:null, awayScore:null, date:'29 Jun', time:'19:00', venue:'Estadio Houston',               status:'scheduled' },
    { id:77,  phase:'dieciseisavos', group:null, home:'1° Grupo I', homeFlag:'🏆', away:'3° C/D/F/G/H',awayFlag:'⭐', homeScore:null, awayScore:null, date:'30 Jun', time:'15:00', venue:'Estadio Nueva York',            status:'scheduled' },
    { id:78,  phase:'dieciseisavos', group:null, home:'2° Grupo E', homeFlag:'🥈', away:'2° Grupo I',  awayFlag:'🥈', homeScore:null, awayScore:null, date:'30 Jun', time:'12:00', venue:'Estadio Dallas',               status:'scheduled' },
    { id:79,  phase:'dieciseisavos', group:null, home:'1° Grupo A', homeFlag:'🏆', away:'3° C/E/F/H/I',awayFlag:'⭐', homeScore:null, awayScore:null, date:'30 Jun', time:'19:00', venue:'Estadio Ciudad de México',      status:'scheduled' },
    { id:80,  phase:'dieciseisavos', group:null, home:'1° Grupo L', homeFlag:'🏆', away:'3° E/H/I/J/K',awayFlag:'⭐', homeScore:null, awayScore:null, date:'01 Jul', time:'10:00', venue:'Estadio Atlanta',               status:'scheduled' },
    { id:81,  phase:'dieciseisavos', group:null, home:'1° Grupo D', homeFlag:'🏆', away:'3° B/E/F/I/J',awayFlag:'⭐', homeScore:null, awayScore:null, date:'01 Jul', time:'13:00', venue:'Estadio Bahía de San Francisco', status:'scheduled' },
    { id:82,  phase:'dieciseisavos', group:null, home:'1° Grupo G', homeFlag:'🏆', away:'3° A/E/H/I/J',awayFlag:'⭐', homeScore:null, awayScore:null, date:'01 Jul', time:'19:00', venue:'Estadio Seattle',               status:'scheduled' },
    { id:83,  phase:'dieciseisavos', group:null, home:'2° Grupo K', homeFlag:'🥈', away:'2° Grupo L',  awayFlag:'🥈', homeScore:null, awayScore:null, date:'02 Jul', time:'13:00', venue:'Estadio Toronto',               status:'scheduled' },
    { id:84,  phase:'dieciseisavos', group:null, home:'1° Grupo H', homeFlag:'🏆', away:'2° Grupo J',  awayFlag:'🥈', homeScore:null, awayScore:null, date:'02 Jul', time:'17:30', venue:'Estadio Los Ángeles',           status:'scheduled' },
    { id:85,  phase:'dieciseisavos', group:null, home:'1° Grupo B', homeFlag:'🏆', away:'3° E/F/G/I/J',awayFlag:'⭐', homeScore:null, awayScore:null, date:'02 Jul', time:'20:30', venue:'Estadio BC Place Vancouver',    status:'scheduled' },
    { id:86,  phase:'dieciseisavos', group:null, home:'1° Grupo J', homeFlag:'🏆', away:'2° Grupo H',  awayFlag:'🥈', homeScore:null, awayScore:null, date:'03 Jul', time:'18:00', venue:'Estadio Miami',                 status:'scheduled' },
    { id:87,  phase:'dieciseisavos', group:null, home:'1° Grupo K', homeFlag:'🏆', away:'3° D/E/I/J/L',awayFlag:'⭐', homeScore:null, awayScore:null, date:'03 Jul', time:'18:00', venue:'Estadio Kansas City',           status:'scheduled' },
    { id:88,  phase:'dieciseisavos', group:null, home:'2° Grupo D', homeFlag:'🥈', away:'2° Grupo G',  awayFlag:'🥈', homeScore:null, awayScore:null, date:'03 Jul', time:'14:00', venue:'Estadio Dallas',               status:'scheduled' },
    // ── CUARTOS DE FINAL
    { id:89,  phase:'cuartos', group:null, home:'Ganador 74', homeFlag:'⚽', away:'Ganador 77', awayFlag:'⚽', homeScore:null, awayScore:null, date:'04 Jul', time:'14:00', venue:'Estadio Filadelfia', status:'scheduled' },
    { id:90,  phase:'cuartos', group:null, home:'Ganador 73', homeFlag:'⚽', away:'Ganador 75', awayFlag:'⚽', homeScore:null, awayScore:null, date:'04 Jul', time:'19:00', venue:'Estadio Houston',    status:'scheduled' },
    { id:91,  phase:'cuartos', group:null, home:'Ganador 76', homeFlag:'⚽', away:'Ganador 78', awayFlag:'⚽', homeScore:null, awayScore:null, date:'05 Jul', time:'14:00', venue:'Estadio Nueva York', status:'scheduled' },
    { id:92,  phase:'cuartos', group:null, home:'Ganador 79', homeFlag:'⚽', away:'Ganador 80', awayFlag:'⚽', homeScore:null, awayScore:null, date:'05 Jul', time:'18:00', venue:'Estadio Ciudad de México', status:'scheduled' },
    { id:93,  phase:'cuartos', group:null, home:'Ganador 83', homeFlag:'⚽', away:'Ganador 84', awayFlag:'⚽', homeScore:null, awayScore:null, date:'06 Jul', time:'18:00', venue:'Estadio Dallas',     status:'scheduled' },
    { id:94,  phase:'cuartos', group:null, home:'Ganador 81', homeFlag:'⚽', away:'Ganador 82', awayFlag:'⚽', homeScore:null, awayScore:null, date:'06 Jul', time:'15:00', venue:'Estadio Seattle',    status:'scheduled' },
    { id:95,  phase:'cuartos', group:null, home:'Ganador 86', homeFlag:'⚽', away:'Ganador 88', awayFlag:'⚽', homeScore:null, awayScore:null, date:'07 Jul', time:'10:00', venue:'Estadio Atlanta',    status:'scheduled' },
    { id:96,  phase:'cuartos', group:null, home:'Ganador 85', homeFlag:'⚽', away:'Ganador 87', awayFlag:'⚽', homeScore:null, awayScore:null, date:'07 Jul', time:'14:00', venue:'Estadio BC Place Vancouver', status:'scheduled' },
    // ── CUARTOS DE FINAL (ronda propia)
    { id:97,  phase:'cuartos', group:null, home:'Ganador 89', homeFlag:'⚽', away:'Ganador 90', awayFlag:'⚽', homeScore:null, awayScore:null, date:'09 Jul', time:'13:00', venue:'Estadio Boston',     status:'scheduled' },
    { id:98,  phase:'cuartos', group:null, home:'Ganador 93', homeFlag:'⚽', away:'Ganador 94', awayFlag:'⚽', homeScore:null, awayScore:null, date:'10 Jul', time:'13:00', venue:'Estadio Los Ángeles', status:'scheduled' },
    { id:99,  phase:'cuartos', group:null, home:'Ganador 91', homeFlag:'⚽', away:'Ganador 92', awayFlag:'⚽', homeScore:null, awayScore:null, date:'11 Jul', time:'13:00', venue:'Estadio Miami',      status:'scheduled' },
    { id:100, phase:'cuartos', group:null, home:'Ganador 95', homeFlag:'⚽', away:'Ganador 96', awayFlag:'⚽', homeScore:null, awayScore:null, date:'11 Jul', time:'19:00', venue:'Estadio Kansas City', status:'scheduled' },
    // ── SEMIFINALES
    { id:101, phase:'semis', group:null, home:'Ganador 97', homeFlag:'⚽', away:'Ganador 98', awayFlag:'⚽', homeScore:null, awayScore:null, date:'14 Jul', time:'18:00', venue:'Estadio Dallas',   status:'scheduled' },
    { id:102, phase:'semis', group:null, home:'Ganador 99', homeFlag:'⚽', away:'Ganador 100',awayFlag:'⚽', homeScore:null, awayScore:null, date:'15 Jul', time:'13:00', venue:'Estadio Atlanta',  status:'scheduled' },
    // ── TERCER PUESTO
    { id:103, phase:'semis', group:null, home:'Perdedor 101',homeFlag:'🥉', away:'Perdedor 102',awayFlag:'🥉', homeScore:null, awayScore:null, date:'18 Jul', time:'13:00', venue:'Estadio Miami',   status:'scheduled' },
    // ── GRAN FINAL
    { id:104, phase:'final', group:null, home:'Ganador 101', homeFlag:'🌎', away:'Ganador 102', awayFlag:'🌎', homeScore:null, awayScore:null, date:'19 Jul', time:'13:00', venue:'Estadio Nueva York', status:'scheduled' },
  ],

  standings: {
    A: [
      { team:'México',        flag:'🇲🇽', pj:1, pg:1, pe:0, pp:0, gf:2, gc:0, pts:3 },
      { team:'Rep. de Corea', flag:'🇰🇷', pj:1, pg:1, pe:0, pp:0, gf:2, gc:1, pts:3 },
      { team:'Rep. Checa',    flag:'🇨🇿', pj:1, pg:0, pe:0, pp:1, gf:1, gc:2, pts:0 },
      { team:'Sudáfrica',     flag:'🇿🇦', pj:1, pg:0, pe:0, pp:1, gf:0, gc:2, pts:0 },
    ],
    B: [
      { team:'Canadá',               flag:'🇨🇦', pj:1, pg:0, pe:1, pp:0, gf:1, gc:1, pts:1 },
      { team:'Bosnia y Herzegovina', flag:'🇧🇦', pj:1, pg:0, pe:1, pp:0, gf:1, gc:1, pts:1 },
      { team:'Catar',                flag:'🇶🇦', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Suiza',                flag:'🇨🇭', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    C: [
      { team:'Brasil',    flag:'🇧🇷', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Marruecos', flag:'🇲🇦', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Haití',     flag:'🇭🇹', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Escocia',   flag:'🏴󠁧󠁢󠁳󠁣󠁴󠁿', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    D: [
      { team:'Estados Unidos', flag:'🇺🇸', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Paraguay',       flag:'🇵🇾', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Australia',      flag:'🇦🇺', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Turquía',        flag:'🇹🇷', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    E: [
      { team:'Alemania',        flag:'🇩🇪', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Curazao',         flag:'🇨🇼', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Costa de Marfil', flag:'🇨🇮', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Ecuador',         flag:'🇪🇨', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    F: [
      { team:'Países Bajos', flag:'🇳🇱', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Japón',        flag:'🇯🇵', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Suecia',       flag:'🇸🇪', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Túnez',        flag:'🇹🇳', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    G: [
      { team:'Bélgica',      flag:'🇧🇪', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Egipto',       flag:'🇪🇬', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'RI de Irán',   flag:'🇮🇷', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Nueva Zelanda',flag:'🇳🇿', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    H: [
      { team:'España',        flag:'🇪🇸', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Cabo Verde',    flag:'🇨🇻', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Arabia Saudita',flag:'🇸🇦', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Uruguay',       flag:'🇺🇾', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    I: [
      { team:'Francia',  flag:'🇫🇷', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Senegal',  flag:'🇸🇳', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Irak',     flag:'🇮🇶', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Noruega',  flag:'🇳🇴', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    J: [
      { team:'Argentina', flag:'🇦🇷', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Argelia',   flag:'🇩🇿', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Austria',   flag:'🇦🇹', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Jordania',  flag:'🇯🇴', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    K: [
      { team:'Portugal',   flag:'🇵🇹', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'RD Congo',   flag:'🇨🇩', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Uzbekistán', flag:'🇺🇿', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Colombia',   flag:'🇨🇴', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
    L: [
      { team:'Inglaterra', flag:'🏴󠁧󠁢󠁥󠁮󠁧󠁿', pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Croacia',    flag:'🇭🇷',        pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Ghana',      flag:'🇬🇭',        pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
      { team:'Panamá',     flag:'🇵🇦',        pj:0, pg:0, pe:0, pp:0, gf:0, gc:0, pts:0 },
    ],
  },

  scorers: [
    { name:'Julián Quiñones', team:'México (Primer gol del Mundial)', flag:'🇲🇽', goals:1, highlight:true },
    { name:'Raúl Jiménez', team:'México', flag:'🇲🇽', goals:1 },
    { name:'Hwang In-beom', team:'Corea del Sur', flag:'🇰🇷', goals:1 },
    { name:'Oh Hyeon-gyu', team:'Corea del Sur', flag:'🇰🇷', goals:1 },
    { name:'Ladislav Krejčí', team:'Chequia', flag:'🇨🇿', goals:1 },
    { name:'Cyle Larin', team:'Canadá', flag:'🇨🇦', goals:1 },
    { name:'Jovo Lukić', team:'Bosnia y Herzegovina', flag:'🇧🇦', goals:1 },
  ],

  yellowCards: [
    { player:'Teboho Mokoena', team:'Sudáfrica', flag:'🇿🇦', qty:1, min:'—' },
    { player:'Nkosinathi Sibisi', team:'Sudáfrica', flag:'🇿🇦', qty:1, min:'—' },
    { player:'Ermedin Demirović', team:'Bosnia y Herzegovina', flag:'🇧🇦', qty:1, min:'—' },
    { player:'Alistair Johnston', team:'Canadá', flag:'🇨🇦', qty:1, min:'—' },
  ],

  redCards: [
    { player:'Yaya Sithole', team:'Sudáfrica', flag:'🇿🇦', min:'Doble amarilla', desc:'Expulsado por doble amonestación tras faltas consecutivas.' },
    { player:'Themba Zwane', team:'Sudáfrica', flag:'🇿🇦', min:'Roja directa', desc:'Tarjeta roja tras un altercado y manotazo a un rival.' },
    { player:'César Montes', team:'México', flag:'🇲🇽', min:'Roja directa', desc:'Expulsado sobre la hora por una fuerte entrada tardía.' },
  ],

  crazyNumbers: [
    { num:'1°', label:'Gol de Julián Quiñones para México', sub:'El primer gol oficial del Mundial 2026' },
    { num:'3', label:'Tarjetas rojas en la jornada inaugural', sub:'Un arbitraje extremadamente estricto desde el silbatazo' },
    { num:'72', label:'Partidos en la fase de grupos', sub:'Parte del formato histórico de 48 selecciones' },
    { num:'2-0', label:'México arrancó con triunfo en el Azteca', sub:'Ante Sudáfrica, en el partido inaugural' },
  ],


  noticias: [
    {
      accentColor: '',
      kicker: '🔥 Jornada 1 · Grupo A',
      kickerClass: '',
      title: 'México despertó al mundo: "La Copa ya está aquí y El Tri tiene hambre de gloria"',
      text: 'El Estadio Ciudad de México tembló desde los cimientos. No fue un debut cualquiera; fue el inicio de nuestra Copa del Mundo y la explosión de un país entero que vio nacer una nueva era. Con el regreso de la máxima fiesta a suelo nacional, la cancha se llenó de una electricidad única, impulsada por el descaro y la frescura de la juventud mexicana. Armando "Hormiga" González demostró que el área tiene un nuevo dueño con un golazo de garra que rompió el hielo, mientras que el niño prodigio de solo 17 años, Gilberto Mora, entró a mover los hilos del mediocampo con la madurez de un veterano, contagiando un entusiasmo que borró cualquier fantasma del pasado. México no solo debutó ganando; recuperó su identidad con una selección vertical, intensa y con un veneno juvenil que invita a soñar en grande. La fiesta en Guadalajara duró hasta el amanecer: el mariachi tocó dentro del Akron y el mundo entero entendió que el gigante ha despertado.',
      jugadorFlag: '🇲🇽',
      jugadorName: 'Gilberto Mora',
      jugadorLabel: 'Joya del Partido',
      tags: ['#LaCopaEstáAquí', '#HormigaGonzález', '#Mora17', '#GDL2026'],
      momento: 'Min. 72 — El debut histórico de Mora que desató la magia en el mediocampo.',
      impacto: 'México inaugura su Mundial con 3 puntos de oro y una ilusión renovada.',
    },
    {
      accentColor: 'lime',
      kicker: '🚑 Parte Médico · Las Bajas del Torneo',
      kickerClass: 'lime',
      title: 'El Mundial de las lesiones: las estrellas que se quedaron fuera antes de empezar',
      text: 'Si algo nos enseñó esta previa es que el cuerpo humano tiene límites, aunque la agenda FIFA no quiera saberlo. El parte médico previo al arranque ha sido durísimo y supera con creces el índice de lesionados de torneos anteriores, todo por la carga brutal de la temporada europea de clubes. Brasil es, sin duda, el más golpeado: perdió a Rodrygo Goes, a Éder Militão y a la joven promesa Estevão justo antes de viajar, mientras su lateral Noussair Mazraoui quedó descartado para el arranque de grupos por una luxación de hombro. Japón sufrió un golpe devastador con la baja de su capitán Wataru Endo, quien además anunció su retiro de la selección, sumándose a las ausencias previas de Kaoru Mitoma y Takumi Minamino. Países Bajos perdió por completo su columna vertebral creativa tras las roturas de ligamentos de Xavi Simons y Jerdy Schouten. Los vigentes campeones de España sufrieron la baja de Fermín López, y del lado inglés las alarmas se encendieron al perder a Jack Grealish por fractura por estrés y a Ben White. Canadá, como anfitrión, también paga el precio: se quedó sin su atacante Marcelo Flores por una rotura de ligamento cruzado. México tampoco se salvó: su portero titular, Luis Malagón, quedó fuera de la convocatoria por una lesión de último momento, abriendo la portería para el debut. La lista sigue creciendo y todavía no se ha jugado ni una semana completa.',
      jugadorFlag: '🇧🇷',
      jugadorName: 'Rodrygo, Militão, Estevão',
      jugadorLabel: 'Bajas confirmadas · Brasil',
      tags: ['#PartesMedicos', '#Mundial2026', '#FuerzaCampeones'],
      momento: 'Brasil llega al torneo sin tres piezas clave de su ofensiva y su defensa.',
      impacto: 'Cada selección golpeada deberá reconfigurar su plan de juego desde la jornada 1. El nivel competitivo del grupo puede cambiar drásticamente.',
    },
    {
      accentColor: 'blue',
      kicker: '🏆 Dato de cultura general',
      kickerClass: 'blue',
      title: 'El Mundial más grande de la historia tiene 48 equipos. ¿Cómo funciona el formato?',
      text: 'Por primera vez, el Mundial tiene 48 selecciones divididas en 12 grupos de 4. Los primeros dos de cada grupo avanzan directo a los octavos de final. Los ocho mejores terceros lugares también clasifican. Eso significa 32 equipos en octavos — exactamente el formato que conocías como la ronda completa de 1998-2022, pero ahora es solo el punto de partida. El total de partidos pasa de 64 a 104, lo que significa más drama, más sorpresas y más posibilidades de que selecciones como México, Colombia o Ecuador lleguen lejos. La sede triple (México, Estados Unidos, Canadá) garantiza que cada zona horaria latinoamericana tenga partidos a buena hora. Y sí: Guadalajara tiene sus 6 partidos, incluyendo uno de octavos.',
      jugadorFlag: '🌎',
      jugadorName: 'El formato 2026',
      jugadorLabel: '104 partidos · 48 selecciones',
      tags: ['#Mundial2026', '#FormatoNuevo', '#48Teams'],
      momento: 'El Mundial más largo de la historia: 39 días de fútbol continuo.',
      impacto: '16 selecciones adicionales vs. Qatar 2022. CONCACAF tiene 6 cupos (vs. 3.5 antes).',
    },
  ],

  gdlMatches: [
    // ── Estadio Ciudad de México
    { id:1,  phase:'Grupos A · CDMX',    home:'México',      homeFlag:'🇲🇽', away:'Sudáfrica',   awayFlag:'🇿🇦', homeScore:2, awayScore:0, date:'11 Jun', time:'13:00', status:'done' },
    { id:62, phase:'Grupos K · CDMX',    home:'Uzbekistán',  homeFlag:'🇺🇿', away:'Colombia',    awayFlag:'🇨🇴', homeScore:null, awayScore:null, date:'17 Jun', time:'20:00', status:'scheduled' },
    { id:5,  phase:'Grupos A · CDMX',    home:'Rep. Checa',  homeFlag:'🇨🇿', away:'México',      awayFlag:'🇲🇽', homeScore:null, awayScore:null, date:'24 Jun', time:'19:00', status:'scheduled' },
    { id:79, phase:'Dieciseisavos · CDMX',home:'1° Grupo A', homeFlag:'🏆',  away:'3° C/E/F/H/I',awayFlag:'⭐',  homeScore:null, awayScore:null, date:'30 Jun', time:'19:00', status:'scheduled' },
    { id:92, phase:'Cuartos · CDMX',     home:'Ganador 79',  homeFlag:'⚽',  away:'Ganador 80',  awayFlag:'⚽',  homeScore:null, awayScore:null, date:'05 Jul', time:'18:00', status:'scheduled' },
    // ── Estadio Guadalajara
    { id:2,  phase:'Grupos A · GDL',     home:'Rep. de Corea',homeFlag:'🇰🇷', away:'Rep. Checa', awayFlag:'🇨🇿', homeScore:2, awayScore:1, date:'11 Jun', time:'20:00', status:'done' },
    { id:4,  phase:'Grupos A · GDL',     home:'México',      homeFlag:'🇲🇽', away:'Rep. de Corea',awayFlag:'🇰🇷', homeScore:null, awayScore:null, date:'18 Jun', time:'19:00', status:'scheduled' },
    { id:64, phase:'Grupos K · GDL',     home:'Colombia',    homeFlag:'🇨🇴', away:'RD Congo',    awayFlag:'🇨🇩', homeScore:null, awayScore:null, date:'23 Jun', time:'20:00', status:'scheduled' },
    { id:47, phase:'Grupos H · GDL',     home:'Uruguay',     homeFlag:'🇺🇾', away:'España',      awayFlag:'🇪🇸', homeScore:null, awayScore:null, date:'26 Jun', time:'18:00', status:'scheduled' },
    { id:75, phase:'Dieciseisavos · GDL',home:'1° Grupo F',  homeFlag:'🏆',  away:'2° Grupo C',  awayFlag:'🥈',  homeScore:null, awayScore:null, date:'29 Jun', time:'18:00', status:'scheduled' },
    // ── Estadio Monterrey
    { id:32, phase:'Grupos F · MTY',     home:'Suecia',      homeFlag:'🇸🇪', away:'Túnez',       awayFlag:'🇹🇳', homeScore:null, awayScore:null, date:'14 Jun', time:'20:00', status:'scheduled' },
    { id:34, phase:'Grupos F · MTY',     home:'Túnez',       homeFlag:'🇹🇳', away:'Japón',       awayFlag:'🇯🇵', homeScore:null, awayScore:null, date:'20 Jun', time:'20:00', status:'scheduled' },
    { id:6,  phase:'Grupos A · MTY',     home:'Sudáfrica',   homeFlag:'🇿🇦', away:'Rep. de Corea',awayFlag:'🇰🇷', homeScore:null, awayScore:null, date:'24 Jun', time:'19:00', status:'scheduled' },
    { id:71, phase:'Grupos L · MTY',     home:'Croacia',     homeFlag:'🇭🇷', away:'Ghana',       awayFlag:'🇬🇭', homeScore:null, awayScore:null, date:'27 Jun', time:'15:00', status:'scheduled' },
    { id:75, phase:'Dieciseisavos · MTY',home:'1° Grupo F',  homeFlag:'🏆',  away:'2° Grupo C',  awayFlag:'🥈',  homeScore:null, awayScore:null, date:'29 Jun', time:'18:00', status:'scheduled' },
  ],

  curiosidades: [
    { emoji:'⚡', titulo:'El Chucky puede ser el héroe que necesitamos', texto:'Si México llega a octavos y Lozano repite su nivel, estaría disputando su tercer Mundial consecutivo siendo el máximo goleador de la Selección. A sus 30 años, este es su último tren para ser leyenda.' },
    { emoji:'🏟️', titulo:'El Akron tiene historia propia', texto:'El estadio de Chivas ha sido sede de Mundiales solo en la mente de sus aficionados... hasta 2026. Antes del Akron, el Jalisco fue escenario del "Gol del Siglo" de Maradona en 1986. GDL lleva la historia en el ADN.' },
    { emoji:'📍', titulo:'Zapopan, no Guadalajara', texto:'Técnicamente el Estadio Akron está en Zapopan, no en Guadalajara. Pero no le digan eso a los tapatíos o se arma. El área metropolitana de Guadalajara es la segunda más grande de México con 5.3 millones de personas.' },
    { emoji:'🌵', titulo:'1970, 1986, 2026: trinidad mundialista', texto:'Solo una docena de ciudades en el mundo han sido sede del Mundial tres veces. GDL se une al club con Ciudad de México, Roma y París. Para una ciudad que también produjo a Cardenal, Rulfo y al mariachi, el fútbol es el menor de sus logros.' },
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
function showView(id) {
  document.querySelectorAll('.view').forEach(v => v.classList.remove('active'));
  document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
  document.getElementById('view-' + id).classList.add('active');
  event.target.classList.add('active');
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
function renderMatches() {
  const container = document.getElementById('matches-container');
  let filtered;

  if (currentPhase === 'semana') {
    const startKey = dateOnlyKey(DATA.currentWeek.startDate);
    const endKey = dateOnlyKey(DATA.currentWeek.endDate);
    filtered = DATA.matches.filter(m => {
      const k = dateOnlyKey(m.date);
      return k >= startKey && k <= endKey;
    });
  } else {
    filtered = DATA.matches.filter(m => m.phase === currentPhase);
    if (currentPhase === 'grupos') filtered = filtered.filter(m => m.group === currentGroup);
  }

  // Orden cronológico
  filtered = [...filtered].sort((a, b) => matchSortKey(a) - matchSortKey(b));

  if (!filtered.length) {
    container.innerHTML = `<div style="padding:40px;text-align:center;font-family:var(--font-mono);font-size:11px;color:var(--ink3);letter-spacing:.1em;text-transform:uppercase;">Partidos por confirmar</div>`;
    return;
  }

  let html = '';
  let lastDate = null;

  filtered.forEach(m => {
    const isDone = m.status === 'done';
    const isLive = m.status === 'live';
    const hasScore = m.homeScore !== null && m.awayScore !== null;
    const isMexico = MEXICO_VENUES.some(v => m.venue.includes(v));

    // Separador de día (solo en vista "Esta semana")
    if (currentPhase === 'semana' && m.date !== lastDate) {
      html += `<div class="day-separator"><span class="day-separator-label">${m.date}</span></div>`;
      lastDate = m.date;
    }

    const scoreHTML = hasScore
      ? `<div class="score-block">
           <div class="score-box home ${isLive ? 'fire' : ''}">${m.homeScore}</div>
           <div class="score-sep"><span>-</span></div>
           <div class="score-box away ${isLive ? 'fire' : ''}">${m.awayScore}</div>
         </div>`
      : `<div class="score-pending">${m.time} hrs</div>`;

    const statusLabel = isLive
      ? `<span class="match-status live-status">● En vivo</span>`
      : isDone
        ? `<span class="match-status done">✓ Finalizado</span>`
        : `<span class="match-status">${m.date}</span>`;

    const mexicoBadge = isMexico
      ? `<span class="mexico-badge">🇲🇽 México</span>`
      : '';

    html += `
      <div class="match-card ${isLive ? 'live' : ''} ${isMexico ? 'mexico-venue' : ''}">
        <div class="match-label-bar">
          <span class="match-label">${m.venue}${mexicoBadge}</span>
          ${statusLabel}
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
      </div>
    `;
  });

  container.innerHTML = html;
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
      const dgStr = dg > 0 ? '+' + dg : String(dg);
      let posClass = i === 0 ? 'pos-q2' : i === 1 ? 'pos-q2' : i === 2 ? 'pos-q3' : 'pos-out';
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
          <td>${t.pj}</td>
          <td>${t.pg}</td>
          <td>${t.pe}</td>
          <td>${t.pp}</td>
          <td>${t.gf}</td>
          <td>${t.gc}</td>
          <td>${dgStr}</td>
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
            <th style="width:50%">Selección</th>
            <th>PJ</th><th>PG</th><th>PE</th><th>PP</th>
            <th>GF</th><th>GC</th><th>DG</th><th>Pts</th>
          </tr></thead>
          <tbody>${rows}</tbody>
        </table>
      </div>
    `;
  }).join('');
}

// ══════════════════════════════════════════════════════════
// RENDER: STATS
// ══════════════════════════════════════════════════════════
function renderStats() {
  // Scorers
  document.getElementById('scorers-list').innerHTML = DATA.scorers.map((s,i) => `
    <div class="scorer-row" style="${s.highlight ? 'background:var(--fire-light);' : ''}">
      <span class="scorer-rank ${i < 3 || s.highlight ? 'top' : ''}">${i+1}</span>
      <div class="scorer-info">
        <div class="scorer-name">${s.flag} ${s.name}</div>
        <div class="scorer-team">${s.team}</div>
      </div>
      <div style="text-align:right;">
        <div class="goals-num">${s.goals}</div>
        <div class="goals-label">gol${s.goals !== 1 ? 'es' : ''}</div>
      </div>
    </div>
  `).join('');

  // Yellow cards
  document.getElementById('yellow-list').innerHTML = DATA.yellowCards.map(c => `
    <div class="card-row">
      <span class="tarjeta tarjeta-amarilla"></span>
      <div class="card-info">
        <div class="card-player">${c.flag} ${c.player}</div>
        <div class="card-team">${c.team}</div>
      </div>
    </div>
  `).join('');

  // Red cards
  document.getElementById('red-list').innerHTML = DATA.redCards.length
    ? DATA.redCards.map(c => `
        <div class="card-row" style="align-items:flex-start;">
          <span class="tarjeta tarjeta-roja" style="margin-top:2px;"></span>
          <div class="card-info">
            <div class="card-player">${c.flag} ${c.player}</div>
            <div class="card-team">${c.team}</div>
            <div style="font-family:var(--font-body);font-size:11px;color:var(--ink2);margin-top:3px;line-height:1.4;">${c.desc || ''}</div>
          </div>
          <span class="card-min" style="flex-shrink:0;">${c.min}</span>
        </div>
      `).join('')
    : `<div style="padding:20px;text-align:center;font-family:var(--font-mono);font-size:10px;color:var(--ink3);letter-spacing:.08em;text-transform:uppercase;">Sin expulsados aún</div>`;

  // Crazy numbers
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
  document.getElementById('gdl-matches').innerHTML = DATA.gdlMatches.map(m => {
    const hasScore = m.homeScore !== null && m.awayScore !== null;
    const isDone = m.status === 'done';
    const scoreHTML = hasScore
      ? `<div class="score-block">
           <div class="score-box home">${m.homeScore}</div>
           <div class="score-sep"><span>-</span></div>
           <div class="score-box away">${m.awayScore}</div>
         </div>`
      : `<div class="score-pending">${m.time}</div>`;

    return `
      <div class="match-card mexico-venue">
        <div class="match-label-bar">
          <span class="match-label">${m.phase} · Estadio Guadalajara <span class="mexico-badge">🇲🇽 México</span></span>
          <span class="match-status ${isDone ? 'done' : ''}">${isDone ? '✓ Finalizado' : m.date}</span>
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
      </div>
    `;
  }).join('');

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
// INIT
// ══════════════════════════════════════════════════════════
function init() {
  renderPhasePills();
  renderGroupSelector();
  document.getElementById('group-selector-wrap').style.display = currentPhase === 'grupos' ? 'block' : 'none';
  updateResultsSubtitle();
  renderMatches();
  renderStandings();
  renderStats();
  renderNoticias();
  renderGDL();
}

init();
</script>
</body>
</html>
