<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <title>Live Match Center</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=JetBrains+Mono:wght@600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-dark: #090d16;
      --card-bg: rgba(18, 24, 38, 0.8);
      --card-border: rgba(255, 255, 255, 0.08);
      --accent-green: #10b981;
      --green-glow: rgba(16, 185, 129, 0.25);
      --accent-red: #f43f5e;
      --accent-amber: #f59e0b;
      --text-main: #f8fafc;
      --text-muted: #64748b;
      --text-sub: #94a3b8;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      -webkit-tap-highlight-color: transparent;
    }

    /* Top empty space fixed by using flex-start and compact padding */
    body {
      background: radial-gradient(circle at 50% 0%, #172554 0%, #090d16 65%);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      padding: 10px 12px;
      font-family: 'Plus Jakarta Sans', sans-serif;
      color: var(--text-main);
    }

    .match-card {
      width: 100%;
      max-width: 420px;
      background: var(--card-bg);
      backdrop-filter: blur(24px);
      -webkit-backdrop-filter: blur(24px);
      border: 1px solid var(--card-border);
      border-radius: 24px;
      padding: 18px 18px 14px;
      box-shadow: 0 20px 40px -10px rgba(0, 0, 0, 0.6), inset 0 1px 0 rgba(255, 255, 255, 0.1);
      position: relative;
      overflow: hidden;
      margin-top: 4px;
    }

    .match-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 50%;
      transform: translateX(-50%);
      width: 160px;
      height: 3px;
      background: linear-gradient(90deg, transparent, rgba(56, 189, 248, 0.8), transparent);
      border-radius: 10px;
    }

    .header-bar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 10px;
    }

    .format-tag {
      font-size: 0.7rem;
      font-weight: 800;
      letter-spacing: 1.2px;
      text-transform: uppercase;
      padding: 4px 10px;
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.08);
      border-radius: 30px;
      color: var(--text-sub);
    }

    .live-badge {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      background: rgba(244, 63, 94, 0.12);
      border: 1px solid rgba(244, 63, 94, 0.3);
      padding: 4px 10px;
      border-radius: 30px;
      font-size: 0.7rem;
      font-weight: 800;
      letter-spacing: 0.8px;
      color: #fda4af;
      text-transform: uppercase;
    }

    .pulse-dot {
      width: 6px;
      height: 6px;
      background-color: var(--accent-red);
      border-radius: 50%;
      box-shadow: 0 0 10px var(--accent-red);
      animation: pulse 1.4s infinite;
    }

    @keyframes pulse {
      0% { transform: scale(0.95); opacity: 0.7; }
      50% { transform: scale(1.3); opacity: 1; }
      100% { transform: scale(0.95); opacity: 0.7; }
    }

    .session-info {
      text-align: center;
      font-size: 0.8rem;
      font-weight: 600;
      color: #38bdf8;
      letter-spacing: 0.3px;
      margin-bottom: 14px;
    }

    .teams-wrap {
      display: flex;
      flex-direction: column;
      gap: 8px;
      margin-bottom: 12px;
    }

    .team-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 12px 14px;
      background: rgba(255, 255, 255, 0.03);
      border: 1px solid rgba(255, 255, 255, 0.04);
      border-radius: 16px;
      transition: all 0.3s ease;
    }

    .team-row.active {
      background: linear-gradient(90deg, rgba(16, 185, 129, 0.08), rgba(255, 255, 255, 0.02));
      border: 1px solid rgba(16, 185, 129, 0.3);
    }

    .team-left {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .team-avatar {
      width: 36px;
      height: 36px;
      border-radius: 50%;
      background: #1e293b;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 700;
      font-size: 0.75rem;
      color: #94a3b8;
      border: 1px solid rgba(255, 255, 255, 0.1);
    }

    .team-meta {
      display: flex;
      flex-direction: column;
    }

    .team-name {
      font-size: 1rem;
      font-weight: 700;
      color: #fff;
    }

    .team-sub {
      font-size: 0.72rem;
      color: var(--text-muted);
    }

    .team-right {
      text-align: right;
    }

    .score-highlight {
      font-family: 'JetBrains Mono', monospace;
      font-size: 1.25rem;
      font-weight: 700;
      color: var(--accent-green);
      letter-spacing: -0.5px;
      text-shadow: 0 0 12px var(--green-glow);
    }

    .overs-highlight {
      font-size: 0.75rem;
      color: var(--text-muted);
      margin-top: 1px;
    }

    .yet-to-bat {
      font-size: 0.88rem;
      font-weight: 600;
      color: #64748b;
    }

    .metrics-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 8px;
      margin-bottom: 12px;
    }

    .metric-card {
      background: rgba(0, 0, 0, 0.25);
      border: 1px solid rgba(255, 255, 255, 0.04);
      padding: 8px 12px;
      border-radius: 12px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .metric-title {
      font-size: 0.7rem;
      color: var(--text-muted);
      font-weight: 600;
      text-transform: uppercase;
    }

    .metric-val {
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.88rem;
      font-weight: 700;
      color: #fff;
    }

    .commentary-banner {
      background: linear-gradient(135deg, rgba(245, 158, 11, 0.08), rgba(245, 158, 11, 0.02));
      border: 1px solid rgba(245, 158, 11, 0.2);
      border-radius: 12px;
      padding: 10px 14px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 12px;
    }

    .commentary-action {
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .ball-badge {
      background: var(--accent-amber);
      color: #000;
      font-size: 0.65rem;
      font-weight: 800;
      padding: 2px 6px;
      border-radius: 5px;
      text-transform: uppercase;
    }

    .commentary-text {
      font-size: 0.82rem;
      font-weight: 600;
      color: #fbbf24;
    }

    .commentary-sub {
      font-size: 0.72rem;
      color: #d97706;
      font-weight: 500;
    }

    .match-note {
      text-align: center;
      font-size: 0.78rem;
      color: var(--text-sub);
      margin-bottom: 12px;
    }

    /* Premium Scorecard Button */
    .btn-container {
      margin-bottom: 12px;
    }

    .scorecard-btn {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      width: 100%;
      padding: 11px 16px;
      background: linear-gradient(135deg, #0284c7, #2563eb);
      color: #ffffff;
      text-decoration: none;
      font-weight: 700;
      font-size: 0.82rem;
      letter-spacing: 0.6px;
      text-transform: uppercase;
      border-radius: 14px;
      border: 1px solid rgba(255, 255, 255, 0.18);
      box-shadow: 0 8px 20px -4px rgba(37, 99, 235, 0.4);
      transition: all 0.2s ease;
    }

    .scorecard-btn:active {
      transform: scale(0.98);
      opacity: 0.9;
    }

    .scorecard-btn svg {
      width: 16px;
      height: 16px;
      stroke: currentColor;
    }

    .footer {
      border-top: 1px solid rgba(255, 255, 255, 0.06);
      padding-top: 10px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 0.68rem;
      color: var(--text-muted);
    }

    .loader {
      text-align: center;
      padding: 30px 0;
      color: var(--text-sub);
      font-size: 0.85rem;
    }
  </style>
</head>
<body>

  <div class="match-card" id="matchWidget">
    <div class="loader">Loading Live Match Data...</div>
  </div>

  <script>
    const API_URL = 'https://api.cricradio.com.au/api/v2/match/mini-match-card?matchId=6a46abf321dc815bb318261b';
    
    // আপোনাৰ Scorecard পেজৰ লিংক ইয়াত দিয়ক
    const SCORECARD_URL = 'scorecard.html'; 

    function getTeamScore(team, prefix) {
      const s1 = team[`${prefix}_1_score`];
      const s2 = team[`${prefix}_2_score`];
      if (s2 && s2.overs) return { runs: s2.runs, wkts: s2.wickets, ovs: s2.overs, batted: true };
      if (s1 && s1.overs) return { runs: s1.runs, wkts: s1.wickets, ovs: s1.overs, batted: true };
      return { runs: 0, wkts: 0, ovs: '0.0', batted: false };
    }

    async function loadCricketData() {
      const card = document.getElementById('matchWidget');
      try {
        const req = await fetch(API_URL);
        const res = await req.json();
        const m = res.responseData.result;

        const currentBatting = m.settingObj?.currentTeam || '';
        const teamA = m.teams.a;
        const teamB = m.teams.b;

        const scoreA = getTeamScore(teamA, 'a');
        const scoreB = getTeamScore(teamB, 'b');

        const session = (m.now.day && m.now.sessionCount) 
          ? `Day ${m.now.day} • Session ${m.now.sessionCount}` 
          : '';

        card.innerHTML = `
          <div class="header-bar">
            <span class="format-tag">${m.format}</span>
            <div class="live-badge">
              <span class="pulse-dot"></span>
              ${m.status}
            </div>
          </div>

          ${session ? `<div class="session-info">${session}</div>` : ''}

          <div class="teams-wrap">
            <!-- Team A -->
            <div class="team-row ${currentBatting === 'a' ? 'active' : ''}">
              <div class="team-left">
                <div class="team-avatar">${teamA.shortName.substring(0, 2)}</div>
                <div class="team-meta">
                  <span class="team-name">${teamA.name}</span>
                  <span class="team-sub">${teamA.shortName}</span>
                </div>
              </div>
              <div class="team-right">
                ${scoreA.batted 
                  ? `<div class="score-highlight">${scoreA.runs}/${scoreA.wkts}</div>
                     <div class="overs-highlight">${scoreA.ovs} Ov</div>`
                  : `<span class="yet-to-bat">Yet to Bat</span>`
                }
              </div>
            </div>

            <!-- Team B -->
            <div class="team-row ${currentBatting === 'b' ? 'active' : ''}">
              <div class="team-left">
                <div class="team-avatar">${teamB.shortName.substring(0, 2)}</div>
                <div class="team-meta">
                  <span class="team-name">${teamB.name}</span>
                  <span class="team-sub">${teamB.shortName}</span>
                </div>
              </div>
              <div class="team-right">
                ${scoreB.batted 
                  ? `<div class="score-highlight">${scoreB.runs}/${scoreB.wkts}</div>
                     <div class="overs-highlight">${scoreB.ovs} Ov</div>`
                  : `<span class="yet-to-bat">Yet to Bat</span>`
                }
              </div>
            </div>
          </div>

          <div class="metrics-grid">
            <div class="metric-card">
              <span class="metric-title">CRR</span>
              <span class="metric-val">${m.now.run_rate || '0.00'}</span>
            </div>
            <div class="metric-card">
              <span class="metric-title">Overs Left</span>
              <span class="metric-val">${m.now.overLeft || '-'}</span>
            </div>
          </div>

          ${m.lastCommentary && m.lastCommentary.primaryText ? `
            <div class="commentary-banner">
              <div class="commentary-action">
                <span class="ball-badge">Last Ball</span>
                <span class="commentary-text">${m.lastCommentary.primaryText}</span>
              </div>
              ${m.lastCommentary.secondaryText ? `<span class="commentary-sub">${m.lastCommentary.secondaryText}</span>` : ''}
            </div>
          ` : ''}

          ${m.announcement1 ? `<div class="match-note">${m.announcement1}</div>` : ''}

          <!-- Scorecard Button -->
          <div class="btn-container">
            <a href="${SCORECARD_URL}" target="_blank" class="scorecard-btn">
              <span>View Full Scorecard</span>
              <svg fill="none" viewBox="0 0 24 24" stroke-width="2.5" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3" />
              </svg>
            </a>
          </div>

          <div class="footer">
            <span>Live Sync: Active</span>
            <span>Update: ${new Date().toLocaleTimeString([], { hour: '2-digit', minute: '2-digit', second: '2-digit' })}</span>
          </div>
        `;
      } catch (e) {
        console.error('Data Sync Error:', e);
      }
    }

    loadCricketData();
    setInterval(loadCricketData, 5000);
  </script>
</body>
</html>
