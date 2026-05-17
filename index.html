<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <title>Polla Mundial 2026 🏆</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:wght@300;400;500;600&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
  <script src="https://cdnjs.cloudflare.com/ajax/libs/crypto-js/4.2.0/crypto-js.min.js"></script>
  <style>
    :root {
      --green: #00C853;
      --green-dark: #00962e;
      --gold: #FFD600;
      --gold-dark: #c9a800;
      --red: #FF1744;
      --orange: #FF6D00;
      --navy: #0a0f1e;
      --navy-mid: #111827;
      --navy-light: #1a2540;
      --card: #141d33;
      --card-border: rgba(255,255,255,0.07);
      --text: #f0f4ff;
      --muted: #8892aa;
      --colombia: #FFD700;
      --radius: 12px;
      --radius-lg: 18px;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    html, body { height: 100%; width: 100%; }

    body {
      font-family: 'DM Sans', sans-serif;
      background: var(--navy);
      color: var(--text);
      min-height: 100vh;
      overflow-x: hidden;
      -webkit-user-select: none;
      user-select: none;
    }

    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background:
        radial-gradient(ellipse 60% 40% at 20% 0%, rgba(0,200,83,0.12) 0%, transparent 70%),
        radial-gradient(ellipse 50% 40% at 80% 100%, rgba(255,214,0,0.08) 0%, transparent 70%);
      pointer-events: none;
      z-index: 0;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(10,15,30,0.9);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--card-border);
      padding: 0.75rem 1rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.4rem;
      letter-spacing: 2px;
      background: linear-gradient(90deg, var(--green), var(--gold));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      white-space: nowrap;
    }

    .header-right {
      display: flex;
      align-items: center;
      gap: 0.75rem;
    }

    .user-badge {
      display: flex;
      align-items: center;
      gap: 8px;
      font-size: 0.75rem;
      color: var(--muted);
    }

    .user-badge .avatar {
      width: 32px;
      height: 32px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--green-dark), var(--green));
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 600;
      font-size: 0.7rem;
      color: #fff;
      flex-shrink: 0;
    }

    .admin-badge {
      background: rgba(255,214,0,0.15);
      border: 1px solid rgba(255,214,0,0.3);
      color: var(--gold);
      padding: 2px 6px;
      border-radius: 20px;
      font-size: 0.6rem;
      font-weight: 600;
      letter-spacing: 0.3px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 6px;
      padding: 8px 16px;
      border-radius: 8px;
      border: none;
      cursor: pointer;
      font-family: 'DM Sans', sans-serif;
      font-size: 0.85rem;
      font-weight: 500;
      transition: all 0.18s;
      white-space: nowrap;
      touch-action: manipulation;
    }

    .btn-primary { background: var(--green); color: #fff; }
    .btn-primary:active { background: var(--green-dark); }

    .btn-ghost { background: transparent; border: 1px solid var(--card-border); color: var(--muted); }
    .btn-ghost:active { border-color: var(--green); color: var(--text); }

    .btn-gold { background: var(--gold); color: #0a0f1e; font-weight: 600; }
    .btn-gold:active { background: var(--gold-dark); }

    .btn-sm { padding: 6px 12px; font-size: 0.75rem; }
    .btn:disabled { opacity: 0.4; cursor: not-allowed; }

    .app { position: relative; z-index: 1; }
    .container { max-width: 1200px; margin: 0 auto; padding: 1rem; }

    .nav-tabs {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(80px, 1fr));
      gap: 4px;
      background: var(--card);
      border: 1px solid var(--card-border);
      border-radius: var(--radius);
      padding: 4px;
      margin-bottom: 1.5rem;
    }

    .nav-tab {
      padding: 10px 8px;
      border-radius: 6px;
      border: none;
      background: transparent;
      color: var(--muted);
      font-family: 'DM Sans', sans-serif;
      font-size: 0.75rem;
      font-weight: 500;
      cursor: pointer;
      transition: all 0.18s;
      text-align: center;
      line-height: 1.2;
    }

    .nav-tab.active {
      background: var(--navy-light);
      color: var(--text);
      box-shadow: 0 1px 3px rgba(0,0,0,0.3);
    }

    .card {
      background: var(--card);
      border: 1px solid var(--card-border);
      border-radius: var(--radius-lg);
      padding: 1rem;
      margin-bottom: 1rem;
    }

    .card-title {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.2rem;
      letter-spacing: 1px;
      margin-bottom: 1rem;
      color: var(--text);
    }

    #auth-screen {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 1rem;
    }

    .auth-box { width: 100%; max-width: 400px; }

    .auth-logo {
      text-align: center;
      margin-bottom: 2rem;
    }

    .auth-logo h1 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 2.5rem;
      letter-spacing: 3px;
      background: linear-gradient(90deg, var(--green), var(--gold));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      line-height: 1;
      margin-bottom: 0.5rem;
    }

    .auth-logo p {
      color: var(--muted);
      font-size: 0.8rem;
    }

    .auth-tabs {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 4px;
      background: var(--card);
      border: 1px solid var(--card-border);
      border-radius: var(--radius);
      padding: 4px;
      margin-bottom: 1.5rem;
    }

    .auth-tab {
      padding: 8px;
      border-radius: 6px;
      border: none;
      background: transparent;
      color: var(--muted);
      font-family: 'DM Sans', sans-serif;
      font-size: 0.7rem;
      font-weight: 500;
      cursor: pointer;
      transition: all 0.18s;
    }

    .auth-tab.active { background: var(--navy-light); color: var(--text); }

    .form-group { margin-bottom: 1rem; }

    label {
      display: block;
      font-size: 0.7rem;
      font-weight: 500;
      color: var(--muted);
      margin-bottom: 6px;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    input, select, textarea {
      width: 100%;
      background: var(--navy-light);
      border: 1px solid var(--card-border);
      border-radius: 8px;
      padding: 10px;
      color: var(--text);
      font-family: 'DM Sans', sans-serif;
      font-size: 1rem;
      transition: border-color 0.18s;
      outline: none;
    }

    input:focus, select:focus { border-color: var(--green); box-shadow: 0 0 0 3px rgba(0,200,83,0.12); }
    input::placeholder { color: var(--muted); }

    .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; }

    .error-msg, .success-msg {
      font-size: 0.8rem;
      margin-top: 8px;
      display: none;
      padding: 8px;
      border-radius: 6px;
    }

    .error-msg { color: var(--red); background: rgba(255,23,68,0.1); }
    .success-msg { color: var(--green); background: rgba(0,200,83,0.1); }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
      gap: 10px;
      margin-bottom: 1.5rem;
    }

    .stat-card {
      background: var(--navy-light);
      border: 1px solid var(--card-border);
      border-radius: var(--radius);
      padding: 1rem;
      text-align: center;
    }

    .stat-value {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.8rem;
      color: var(--green);
      line-height: 1;
    }

    .stat-label {
      font-size: 0.65rem;
      color: var(--muted);
      margin-top: 0.5rem;
      text-transform: uppercase;
      letter-spacing: 0.3px;
    }

    .leaderboard { display: flex; flex-direction: column; gap: 8px; }

    .lb-row {
      display: grid;
      grid-template-columns: 40px 1fr auto;
      align-items: center;
      gap: 1rem;
      padding: 0.75rem;
      background: var(--navy-light);
      border: 1px solid var(--card-border);
      border-radius: var(--radius);
      animation: slideIn 0.3s ease both;
    }

    .rank-num {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.2rem;
      text-align: center;
    }

    .rank-1 { border-color: rgba(255,214,0,0.35); background: rgba(255,214,0,0.05); }
    .rank-1 .rank-num { color: var(--gold); }

    .lb-avatar {
      width: 32px;
      height: 32px;
      border-radius: 50%;
      background: var(--card);
      border: 1px solid var(--card-border);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.65rem;
      font-weight: 600;
      color: var(--green);
      flex-shrink: 0;
    }

    .lb-name {
      display: flex;
      align-items: center;
      gap: 8px;
      font-weight: 500;
      font-size: 0.85rem;
    }

    .lb-pts {
      font-family: 'DM Mono', monospace;
      font-size: 1.2rem;
      font-weight: 600;
      color: var(--green);
      text-align: right;
    }

    .matches-grid { display: flex; flex-direction: column; gap: 10px; }

    .match-card {
      background: var(--navy-light);
      border: 2px solid var(--card-border);
      border-radius: var(--radius);
      padding: 1rem;
      transition: all 0.18s;
    }

    .match-card.locked { opacity: 0.65; border-color: rgba(255,214,0,0.3); }

    .match-card.colombia {
      border-color: rgba(255,215,0,0.6);
      background: rgba(255,215,0,0.08);
      box-shadow: 0 0 15px rgba(255,215,0,0.1);
    }

    .match-card.colombia:active { background: rgba(255,215,0,0.15); }

    .match-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: 0.5rem;
      margin-bottom: 0.75rem;
      flex-wrap: wrap;
      font-size: 0.75rem;
      color: var(--muted);
    }

    .match-stage {
      font-size: 0.65rem;
      background: rgba(0,200,83,0.15);
      color: var(--green);
      padding: 2px 8px;
      border-radius: 12px;
      font-weight: 500;
    }

    .match-teams {
      display: grid;
      grid-template-columns: 1.2fr auto 1.2fr;
      align-items: center;
      gap: 0.75rem;
      margin-bottom: 0.75rem;
      font-weight: 500;
      font-size: 0.95rem;
    }

    .team-name { word-break: break-word; }
    .team-home { text-align: right; }
    .team-away { text-align: left; }

    .match-score {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 4px;
    }

    .score-display {
      font-family: 'DM Mono', monospace;
      font-size: 1.4rem;
      font-weight: 600;
    }

    .score-inputs {
      display: flex;
      align-items: center;
      gap: 6px;
      justify-content: center;
    }

    .score-input {
      width: 40px !important;
      height: 40px;
      padding: 0 !important;
      text-align: center;
      font-size: 1rem !important;
      font-family: 'DM Mono', monospace !important;
    }

    .score-sep { font-size: 1.1rem; color: var(--muted); }

    .status-badge {
      display: inline-flex;
      align-items: center;
      gap: 4px;
      font-size: 0.65rem;
      padding: 3px 8px;
      border-radius: 12px;
      font-weight: 500;
      white-space: nowrap;
    }

    .status-pending { background: rgba(136,146,170,0.15); color: var(--muted); }
    .status-finished { background: rgba(0,200,83,0.12); color: var(--green); }
    .status-locked { background: rgba(255,214,0,0.12); color: var(--gold); }

    .countdown {
      font-family: 'DM Mono', monospace;
      font-size: 0.8rem;
      color: var(--orange);
      font-weight: 500;
      margin-top: 0.5rem;
    }

    .hidden { display: none !important; }

    @keyframes slideIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .modal {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.7);
      z-index: 200;
      align-items: center;
      justify-content: flex-end;
      padding: 0;
    }

    .modal.active { display: flex; }

    .modal-content {
      background: var(--card);
      width: 100%;
      height: 100%;
      display: flex;
      flex-direction: column;
      overflow-y: auto;
      padding: 1.5rem 1rem;
      max-width: 100%;
    }

    @media (min-width: 600px) {
      .modal-content {
        width: 90%;
        max-width: 500px;
        height: auto;
        border-radius: var(--radius-lg) 0 0 var(--radius-lg);
      }
    }

    .modal-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 1.5rem;
      padding-bottom: 1rem;
      border-bottom: 1px solid var(--card-border);
    }

    .modal-header h2 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.3rem;
      letter-spacing: 1px;
    }

    .close-btn {
      background: none;
      border: none;
      color: var(--muted);
      font-size: 1.5rem;
      cursor: pointer;
      padding: 0;
      width: 32px;
      height: 32px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .filter-group {
      display: flex;
      gap: 8px;
      margin-bottom: 1rem;
      overflow-x: auto;
      -webkit-overflow-scrolling: touch;
      padding-bottom: 0.5rem;
    }

    .filter-btn {
      padding: 6px 12px;
      border-radius: 6px;
      border: 1px solid var(--card-border);
      background: transparent;
      color: var(--muted);
      cursor: pointer;
      font-size: 0.75rem;
      font-weight: 500;
      transition: all 0.18s;
      white-space: nowrap;
      flex-shrink: 0;
    }

    .filter-btn.active {
      background: var(--green);
      color: #fff;
      border-color: var(--green);
    }

    .match-actions {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 8px;
      margin-top: 0.75rem;
    }

    .pred-result {
      display: inline-flex;
      align-items: center;
      gap: 4px;
      font-size: 0.7rem;
      padding: 3px 8px;
      border-radius: 12px;
      margin-top: 0.5rem;
    }

    .pred-exact { background: rgba(255,214,0,0.15); color: var(--gold); }
    .pred-correct { background: rgba(0,200,83,0.12); color: var(--green); }
    .pred-wrong { background: rgba(255,23,68,0.1); color: var(--red); }

    .my-pred {
      font-size: 0.8rem;
      color: var(--muted);
      margin-top: 0.5rem;
      padding: 6px 8px;
      background: rgba(0,200,83,0.07);
      border-left: 2px solid var(--green);
    }

    .admin-section {
      background: rgba(255,214,0,0.05);
      border: 1px solid rgba(255,214,0,0.2);
      border-radius: var(--radius-lg);
      padding: 1rem;
      margin-bottom: 1.5rem;
    }

    .number-input-group {
      display: flex;
      align-items: center;
      gap: 8px;
      margin-bottom: 1rem;
    }

    .number-input-group input {
      max-width: 80px;
      text-align: center;
    }

    .number-input-group label { margin: 0; font-size: 0.85rem; white-space: nowrap; }

    @media (max-width: 600px) {
      header { padding: 0.6rem 0.75rem; }
      .logo { font-size: 1.1rem; }
      .user-badge { font-size: 0.65rem; }
      .nav-tabs { grid-template-columns: repeat(auto-fit, minmax(60px, 1fr)); }
      .nav-tab { padding: 8px 4px; font-size: 0.65rem; }
      .card { padding: 0.75rem; }
      .card-title { font-size: 1rem; }
      .form-row { grid-template-columns: 1fr; }
      .match-card { padding: 0.75rem; }
      .match-header { font-size: 0.7rem; }
      .btn { padding: 7px 12px; font-size: 0.7rem; }
      .stat-value { font-size: 1.5rem; }
      .lb-row { grid-template-columns: 35px 1fr auto; padding: 0.6rem; gap: 0.75rem; }
      .lb-name { font-size: 0.8rem; }
      .lb-pts { font-size: 1rem; }
    }
  </style>
</head>
<body>

  <div id="auth-screen" class="app">
    <div class="auth-box">
      <div class="auth-logo">
        <h1>⚽ MUNDIAL<br>2026</h1>
        <p>Polla de Predicciones</p>
      </div>

      <div class="auth-tabs">
        <button class="auth-tab active" onclick="switchAuthTab('login')">Login</button>
        <button class="auth-tab" onclick="switchAuthTab('register')">Registro</button>
        <button class="auth-tab" onclick="switchAuthTab('forgot')">Olvidé</button>
      </div>

      <div id="login-form" class="card">
        <div class="form-group">
          <label>Usuario</label>
          <input type="text" id="login-username" placeholder="Tu usuario">
        </div>
        <div class="form-group">
          <label>Contraseña</label>
          <input type="password" id="login-password" placeholder="Tu contraseña">
        </div>
        <button class="btn btn-primary" style="width: 100%;" onclick="handleLogin()">Entrar</button>
        <div class="error-msg" id="login-error"></div>
      </div>

      <div id="register-form" class="card hidden">
        <div class="form-group">
          <label>Nombre</label>
          <input type="text" id="register-name" placeholder="Tu nombre">
        </div>
        <div class="form-group">
          <label>Usuario</label>
          <input type="text" id="register-username" placeholder="Elige un usuario">
        </div>
        <div class="form-group">
          <label>Contraseña</label>
          <input type="password" id="register-password" placeholder="6+ caracteres">
        </div>
        <div class="form-group">
          <label>Confirmar</label>
          <input type="password" id="register-password-confirm" placeholder="Repite">
        </div>
        <div class="form-group">
          <label>¿Admin?</label>
          <select id="register-admin-select" onchange="toggleAdminPassword()">
            <option value="no">No</option>
            <option value="yes">Sí (contraseña requerida)</option>
          </select>
        </div>
        <div class="form-group hidden" id="admin-password-group">
          <label>Contraseña Admin</label>
          <input type="password" id="register-admin-password" placeholder="Contraseña de admin">
        </div>
        <button class="btn btn-primary" style="width: 100%;" onclick="handleRegister()">Registrarse</button>
        <div class="error-msg" id="register-error"></div>
      </div>

      <div id="forgot-form" class="card hidden">
        <div class="form-group">
          <label>Usuario</label>
          <input type="text" id="forgot-username" placeholder="Tu usuario">
        </div>
        <div class="form-group">
          <label>Nueva Contraseña</label>
          <input type="password" id="forgot-new-password" placeholder="Nueva contraseña">
        </div>
        <div class="form-group">
          <label>Confirmar</label>
          <input type="password" id="forgot-new-password-confirm" placeholder="Repite">
        </div>
        <button class="btn btn-primary" style="width: 100%;" onclick="handleForgotPassword()">Cambiar</button>
        <div class="error-msg" id="forgot-error"></div>
      </div>
    </div>
  </div>

  <div id="app-screen" class="app hidden">
    <header>
      <div class="logo">⚽ 2026</div>
      <div class="header-right">
        <div class="user-badge">
          <div class="avatar" id="user-avatar">U</div>
          <span class="admin-badge hidden" id="admin-badge">👑</span>
        </div>
        <button class="btn btn-ghost btn-sm" onclick="handleLogout()">Salir</button>
      </div>
    </header>

    <div class="container">
      <div class="nav-tabs">
        <button class="nav-tab active" onclick="switchTab('leaderboard')">🏆</button>
        <button class="nav-tab" onclick="switchTab('matches')">📋</button>
        <button class="nav-tab" onclick="switchTab('all-matches')">⚽</button>
        <button class="nav-tab hidden" id="admin-tab" onclick="switchTab('admin')">⚙️</button>
      </div>

      <div id="leaderboard-tab" class="tab-content">
        <div class="card">
          <div class="card-title">🏆 Clasificación</div>
          <div class="stats-grid">
            <div class="stat-card">
              <div class="stat-value" id="total-matches">0</div>
              <div class="stat-label">Partidos</div>
            </div>
            <div class="stat-card">
              <div class="stat-value" id="my-points">0</div>
              <div class="stat-label">Mis Pts</div>
            </div>
            <div class="stat-card">
              <div class="stat-value" id="my-rank">-</div>
              <div class="stat-label">Posición</div>
            </div>
          </div>
          <div class="leaderboard" id="leaderboard-list"></div>
        </div>
      </div>

      <div id="matches-tab" class="tab-content hidden">
        <div class="card">
          <div class="card-title">📋 Mis Predicciones</div>
          <div class="matches-grid" id="my-predictions-list"></div>
        </div>
      </div>

      <div id="all-matches-tab" class="tab-content hidden">
        <div class="card">
          <div class="card-title">⚽ Todos los Partidos</div>
          <div class="filter-group" id="filter-group"></div>
          <div class="matches-grid" id="all-matches-list"></div>
        </div>
      </div>

      <div id="admin-tab-content" class="tab-content hidden">
        <div class="admin-section">
          <div class="card-title">⚙️ Administración</div>
          <div class="filter-group" id="admin-filter-group"></div>
          <div class="matches-grid" id="admin-matches-list"></div>
        </div>
      </div>
    </div>
  </div>

  <div id="result-modal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Registrar Resultado</h2>
        <button class="close-btn" onclick="closeModal('result-modal')">&times;</button>
      </div>
      <div style="flex: 1;">
        <div class="form-group">
          <label>Goles Local</label>
          <input type="number" id="result-home" min="0" placeholder="0">
        </div>
        <div class="form-group">
          <label>Goles Visitante</label>
          <input type="number" id="result-away" min="0" placeholder="0">
        </div>
      </div>
      <button class="btn btn-gold" style="width: 100%;" onclick="handleRegisterResult()">Guardar</button>
      <div class="error-msg" id="result-error"></div>
    </div>
  </div>

  <div id="deadline-modal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Cerrar Apuestas</h2>
        <button class="close-btn" onclick="closeModal('deadline-modal')">&times;</button>
      </div>
      <div style="flex: 1;">
        <div class="number-input-group">
          <label for="hours-before-input">Horas antes del partido:</label>
          <input type="number" id="hours-before-input" min="0" max="72" value="1" placeholder="1">
        </div>
        <p style="font-size: 0.8rem; color: var(--muted); margin-bottom: 1rem;">
          Si el partido es a las 18:00 e ingresas 1, las apuestas cierran a las 17:00
        </p>
      </div>
      <button class="btn btn-gold" style="width: 100%;" onclick="handleSetDeadline()">Establecer</button>
      <div class="error-msg" id="deadline-error"></div>
    </div>
  </div>

  <div id="points-modal" class="modal">
    <div class="modal-content">
      <div class="modal-header">
        <h2>Asignar Puntos</h2>
        <button class="close-btn" onclick="closeModal('points-modal')">&times;</button>
      </div>
      <div style="flex: 1; overflow-y: auto;">
        <div id="points-list" style="display: flex; flex-direction: column; gap: 1rem;"></div>
      </div>
    </div>
  </div>

  <script>
    const STORAGE_KEYS = {
      users: 'mw26_users',
      matches: 'mw26_matches',
      predictions: 'mw26_predictions',
      scores: 'mw26_scores',
      currentUser: 'mw26_current_user'
    };

    const ADMIN_PASSWORD = 'admin2026';
    let currentUser = null;
    let allMatches = [];
    let allPredictions = {};
    let allScores = {};

    const WORLD_CUP_2026_MATCHES = [
      { home: "México", away: "Canadá", date: "2026-06-12", time: "18:00", stage: "Grupos", group: "A" },
      { home: "Uruguay", away: "Panamá", date: "2026-06-12", time: "20:30", stage: "Grupos", group: "A" },
      { home: "Colombia", away: "Grecia", date: "2026-06-16", time: "18:00", stage: "Grupos", group: "I" },
      { home: "Perú", away: "Nueva Zelanda", date: "2026-06-16", time: "20:30", stage: "Grupos", group: "I" },
      { home: "Colombia", away: "Perú", date: "2026-06-21", time: "18:00", stage: "Grupos", group: "I" },
      { home: "Nueva Zelanda", away: "Grecia", date: "2026-06-21", time: "20:30", stage: "Grupos", group: "I" },
      { home: "Grecia", away: "Perú", date: "2026-06-26", time: "18:00", stage: "Grupos", group: "I" },
      { home: "Nueva Zelanda", away: "Colombia", date: "2026-06-26", time: "18:00", stage: "Grupos", group: "I" },
      { home: "España", away: "Costa Rica", date: "2026-06-13", time: "18:00", stage: "Grupos", group: "B" },
      { home: "Alemania", away: "Japón", date: "2026-06-13", time: "20:30", stage: "Grupos", group: "B" },
      { home: "Francia", away: "Países Bajos", date: "2026-06-14", time: "18:00", stage: "Grupos", group: "D" },
      { home: "Brasil", away: "Serbia", date: "2026-06-14", time: "18:00", stage: "Grupos", group: "E" },
      { home: "Argentina", away: "Marruecos", date: "2026-06-13", time: "18:00", stage: "Grupos", group: "C" },
    ];

    function hashPassword(password) {
      return CryptoJS.SHA256('mundial2026_' + password).toString();
    }

    function initializeMatches() {
      try {
        const stored = localStorage.getItem(STORAGE_KEYS.matches);
        const parsedMatches = stored ? JSON.parse(stored) : [];
        
        if (!parsedMatches || parsedMatches.length === 0) {
          const matches = WORLD_CUP_2026_MATCHES.map((m, idx) => ({
            id: 'match_' + idx + '_' + Date.now(),
            home: m.home,
            away: m.away,
            date: m.date,
            time: m.time,
            stage: m.stage,
            group: m.group,
            status: 'pending',
            scoreHome: null,
            scoreAway: null,
            deadline: null,
            locked: false,
            createdAt: new Date().toISOString()
          }));
          localStorage.setItem(STORAGE_KEYS.matches, JSON.stringify(matches));
        }
      } catch (e) {
        console.error('Error:', e);
        localStorage.removeItem(STORAGE_KEYS.matches);
        const matches = WORLD_CUP_2026_MATCHES.map((m, idx) => ({
          id: 'match_' + idx,
          home: m.home,
          away: m.away,
          date: m.date,
          time: m.time,
          stage: m.stage,
          group: m.group,
          status: 'pending',
          scoreHome: null,
          scoreAway: null,
          deadline: null,
          locked: false
        }));
        localStorage.setItem(STORAGE_KEYS.matches, JSON.stringify(matches));
      }
    }

    function init() {
      initializeMatches();
      loadCurrentUser();
      if (currentUser) {
        showAppScreen();
        loadAllData();
        renderLeaderboard();
        renderMyPredictions();
        renderAllMatches();
        renderAdminPanel();
        startCountdownUpdates();
      } else {
        showAuthScreen();
      }
    }

    function switchAuthTab(tab) {
      document.querySelectorAll('.auth-tab').forEach(t => t.classList.remove('active'));
      event.target.classList.add('active');
      document.getElementById('login-form').classList.toggle('hidden', tab !== 'login');
      document.getElementById('register-form').classList.toggle('hidden', tab !== 'register');
      document.getElementById('forgot-form').classList.toggle('hidden', tab !== 'forgot');
    }

    function toggleAdminPassword() {
      const show = document.getElementById('register-admin-select').value === 'yes';
      document.getElementById('admin-password-group').classList.toggle('hidden', !show);
    }

    function handleRegister() {
      const name = document.getElementById('register-name').value.trim();
      const username = document.getElementById('register-username').value.trim().toLowerCase();
      const password = document.getElementById('register-password').value;
      const confirmPassword = document.getElementById('register-password-confirm').value;
      const adminSelect = document.getElementById('register-admin-select').value;
      const adminPassword = document.getElementById('register-admin-password').value;
      const errorEl = document.getElementById('register-error');

      errorEl.style.display = 'none';

      if (!name || !username || !password) {
        showError(errorEl, 'Completa todos los campos');
        return;
      }

      if (password !== confirmPassword) {
        showError(errorEl, 'Las contraseñas no coinciden');
        return;
      }

      if (password.length < 6) {
        showError(errorEl, 'Mínimo 6 caracteres');
        return;
      }

      let isAdmin = false;
      if (adminSelect === 'yes') {
        if (!adminPassword || adminPassword !== ADMIN_PASSWORD) {
          showError(errorEl, 'Contraseña de admin incorrecta');
          return;
        }
        isAdmin = true;
      }

      const users = JSON.parse(localStorage.getItem(STORAGE_KEYS.users) || '[]');
      if (users.some(u => u.username === username)) {
        showError(errorEl, 'Usuario ya existe');
        return;
      }

      users.push({
        id: Date.now().toString(),
        name,
        username,
        passwordHash: hashPassword(password),
        isAdmin: isAdmin,
        createdAt: new Date().toISOString()
      });

      localStorage.setItem(STORAGE_KEYS.users, JSON.stringify(users));
      currentUser = users[users.length - 1];
      localStorage.setItem(STORAGE_KEYS.currentUser, JSON.stringify(currentUser));

      showAppScreen();
      loadAllData();
      render();
    }

    function handleLogin() {
      const username = document.getElementById('login-username').value.trim().toLowerCase();
      const password = document.getElementById('login-password').value;
      const errorEl = document.getElementById('login-error');

      errorEl.style.display = 'none';

      if (!username || !password) {
        showError(errorEl, 'Usuario y contraseña requeridos');
        return;
      }

      const users = JSON.parse(localStorage.getItem(STORAGE_KEYS.users) || '[]');
      const user = users.find(u => u.username === username && u.passwordHash === hashPassword(password));

      if (!user) {
        showError(errorEl, 'Credenciales incorrectas');
        return;
      }

      currentUser = user;
      localStorage.setItem(STORAGE_KEYS.currentUser, JSON.stringify(currentUser));
      showAppScreen();
      loadAllData();
      render();
    }

    function handleForgotPassword() {
      const username = document.getElementById('forgot-username').value.trim().toLowerCase();
      const newPassword = document.getElementById('forgot-new-password').value;
      const confirmPassword = document.getElementById('forgot-new-password-confirm').value;
      const errorEl = document.getElementById('forgot-error');

      errorEl.style.display = 'none';

      if (!username || !newPassword || !confirmPassword) {
        showError(errorEl, 'Completa todos los campos');
        return;
      }

      if (newPassword !== confirmPassword) {
        showError(errorEl, 'Las contraseñas no coinciden');
        return;
      }

      const users = JSON.parse(localStorage.getItem(STORAGE_KEYS.users) || '[]');
      const user = users.find(u => u.username === username);

      if (!user) {
        showError(errorEl, 'Usuario no encontrado');
        return;
      }

      user.passwordHash = hashPassword(newPassword);
      localStorage.setItem(STORAGE_KEYS.users, JSON.stringify(users));
      alert('✅ Contraseña actualizada. Inicia sesión.');
      switchAuthTab('login');
    }

    function handleLogout() {
      currentUser = null;
      localStorage.removeItem(STORAGE_KEYS.currentUser);
      showAuthScreen();
      document.getElementById('login-username').value = '';
      document.getElementById('login-password').value = '';
    }

    function showError(el, msg) {
      el.textContent = msg;
      el.style.display = 'block';
    }

    function showAuthScreen() {
      document.getElementById('auth-screen').classList.remove('hidden');
      document.getElementById('app-screen').classList.add('hidden');
    }

    function showAppScreen() {
      document.getElementById('auth-screen').classList.add('hidden');
      document.getElementById('app-screen').classList.remove('hidden');
      document.getElementById('user-avatar').textContent = currentUser.name[0].toUpperCase();
      if (currentUser.isAdmin) {
        document.getElementById('admin-badge').classList.remove('hidden');
        document.getElementById('admin-tab').classList.remove('hidden');
      }
    }

    function loadCurrentUser() {
      const stored = localStorage.getItem(STORAGE_KEYS.currentUser);
      if (stored) {
        currentUser = JSON.parse(stored);
      }
    }

    function loadAllData() {
      try {
        allMatches = JSON.parse(localStorage.getItem(STORAGE_KEYS.matches) || '[]');
        allPredictions = JSON.parse(localStorage.getItem(STORAGE_KEYS.predictions) || '{}');
        allScores = JSON.parse(localStorage.getItem(STORAGE_KEYS.scores) || '{}');
      } catch (e) {
        console.error('Error loading:', e);
        allMatches = [];
        allPredictions = {};
        allScores = {};
      }
    }

    function saveData() {
      localStorage.setItem(STORAGE_KEYS.matches, JSON.stringify(allMatches));
      localStorage.setItem(STORAGE_KEYS.predictions, JSON.stringify(allPredictions));
      localStorage.setItem(STORAGE_KEYS.scores, JSON.stringify(allScores));
    }

    function isMatchLocked(match) {
      if (match.locked) return true;
      if (match.deadline) {
        const now = new Date();
        const deadline = new Date(match.deadline);
        if (now >= deadline) {
          match.locked = true;
          saveData();
          return true;
        }
      }
      return false;
    }

    function getTimeToDeadline(match) {
      if (!match.deadline) return null;
      const now = new Date();
      const deadline = new Date(match.deadline);
      const diff = deadline - now;
      if (diff <= 0) return null;
      
      const hours = Math.floor(diff / (1000 * 60 * 60));
      const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
      
      if (hours > 0) return `${hours}h ${minutes}m`;
      return `${minutes}m`;
    }

    function switchTab(name) {
      document.querySelectorAll('.nav-tab').forEach(t => t.classList.remove('active'));
      document.querySelectorAll('.tab-content').forEach(t => t.classList.add('hidden'));
      event.target.classList.add('active');
      
      const tabMap = {
        'leaderboard': 'leaderboard-tab',
        'matches': 'matches-tab',
        'all-matches': 'all-matches-tab',
        'admin': 'admin-tab-content'
      };
      
      if (tabMap[name]) {
        document.getElementById(tabMap[name]).classList.remove('hidden');
        if (name === 'leaderboard') renderLeaderboard();
        else if (name === 'matches') renderMyPredictions();
        else if (name === 'all-matches') renderAllMatches();
        else if (name === 'admin') renderAdminPanel();
      }
    }

    function renderLeaderboard() {
      const users = JSON.parse(localStorage.getItem(STORAGE_KEYS.users) || '[]');
      const rankings = users.map(u => ({
        name: u.name,
        username: u.username,
        points: allScores[u.username] || 0
      })).sort((a, b) => b.points - a.points);

      const myRank = rankings.findIndex(r => r.username === currentUser.username) + 1;
      const myPoints = allScores[currentUser.username] || 0;
      const finished = allMatches.filter(m => m.status === 'finished').length;

      document.getElementById('total-matches').textContent = finished;
      document.getElementById('my-points').textContent = myPoints;
      document.getElementById('my-rank').textContent = myRank > 0 ? '#' + myRank : '-';

      document.getElementById('leaderboard-list').innerHTML = rankings.map((r, i) => `
        <div class="lb-row ${i === 0 ? 'rank-1' : ''}">
          <div class="rank-num">${i + 1}</div>
          <div class="lb-name">
            <div class="lb-avatar">${r.name[0].toUpperCase()}</div>
            <span>${r.name}</span>
          </div>
          <div class="lb-pts">${r.points}</div>
        </div>
      `).join('');
    }

    function renderMyPredictions() {
      const myMatches = allMatches.filter(m => {
        const pred = allPredictions[m.id]?.[currentUser.username];
        return pred || m.status === 'finished';
      });

      document.getElementById('my-predictions-list').innerHTML = myMatches.map(m => {
        const pred = allPredictions[m.id]?.[currentUser.username];
        const locked = isMatchLocked(m);
        const timeLeft = getTimeToDeadline(m);

        let scoreHtml = '';
        if (m.status === 'finished') {
          scoreHtml = `<div class="score-display">${m.scoreHome} - ${m.scoreAway}</div>`;
        }

        let resultHtml = '';
        if (pred && m.status === 'finished') {
          const isExact = pred.home === m.scoreHome && pred.away === m.scoreAway;
          const isCorrect = !isExact && ((m.scoreHome > m.scoreAway && pred.home > pred.away) || 
                                         (m.scoreHome < m.scoreAway && pred.home < pred.away) ||
                                         (m.scoreHome === m.scoreAway && pred.home === pred.away));
          const resultClass = isExact ? 'pred-exact' : isCorrect ? 'pred-correct' : 'pred-wrong';
          const resultText = isExact ? '⭐ +5 pts' : isCorrect ? '✓ +3 pts' : '❌ 0 pts';
          resultHtml = `<span class="pred-result ${resultClass}">${resultText}</span>`;
        }

        const isColombia = m.home === 'Colombia' || m.away === 'Colombia';

        return `
          <div class="match-card ${locked ? 'locked' : ''} ${isColombia ? 'colombia' : ''}">
            <div class="match-header">
              <span class="match-stage">${m.stage}</span>
              <span class="status-badge status-${m.status}">${m.status === 'finished' ? '✓' : '⏱'}</span>
            </div>
            <div class="match-teams">
              <div class="team-home team-name">${m.home}</div>
              <div class="match-score">${scoreHtml}</div>
              <div class="team-away team-name">${m.away}</div>
            </div>
            ${pred ? `<div class="my-pred">Tu predicción: ${pred.home} - ${pred.away} ${resultHtml}</div>` : ''}
            ${timeLeft ? `<div class="countdown">Cierra en ${timeLeft}</div>` : ''}
          </div>
        `;
      }).join('');
    }

    function renderAllMatches() {
      const stages = [...new Set(allMatches.map(m => m.stage))].sort();
      const filterGroup = document.getElementById('filter-group');
      
      if (filterGroup.innerHTML === '') {
        filterGroup.innerHTML = stages.map(s => `
          <button class="filter-btn ${s === 'Grupos' ? 'active' : ''}" onclick="filterMatches('${s}')" data-stage="${s}">${s}</button>
        `).join('');
      }

      const active = filterGroup.querySelector('.filter-btn.active');
      const currentStage = active?.getAttribute('data-stage') || 'Grupos';
      const matches = allMatches.filter(m => m.stage === currentStage);

      document.getElementById('all-matches-list').innerHTML = matches.map(m => {
        const pred = allPredictions[m.id]?.[currentUser.username];
        const locked = isMatchLocked(m);
        const timeLeft = getTimeToDeadline(m);
        const isColombia = m.home === 'Colombia' || m.away === 'Colombia';

        let inputsHtml = '';
        if (!locked && m.status !== 'finished') {
          inputsHtml = `
            <div class="score-inputs">
              <input type="number" class="score-input" id="h-${m.id}" min="0" value="${pred?.home || ''}">
              <span class="score-sep">-</span>
              <input type="number" class="score-input" id="a-${m.id}" min="0" value="${pred?.away || ''}">
              <button class="btn btn-primary btn-sm" onclick="savePred('${m.id}')">✓</button>
            </div>
          `;
        } else if (m.status === 'finished') {
          inputsHtml = `<div class="score-display">${m.scoreHome} - ${m.scoreAway}</div>`;
        }

        return `
          <div class="match-card ${locked ? 'locked' : ''} ${isColombia ? 'colombia' : ''}">
            <div class="match-header">
              <span style="font-size: 0.75rem;">${m.date} ${m.time}</span>
              <span class="match-stage">${m.stage}</span>
            </div>
            <div class="match-teams">
              <div class="team-home team-name">${m.home}</div>
              <div class="match-score">${inputsHtml}</div>
              <div class="team-away team-name">${m.away}</div>
            </div>
            ${timeLeft ? `<div class="countdown">Cierra en ${timeLeft}</div>` : ''}
            ${locked ? `<span class="status-badge status-locked">🔒</span>` : ''}
          </div>
        `;
      }).join('');
    }

    function filterMatches(stage) {
      document.querySelectorAll('#all-matches-tab .filter-btn').forEach(b => b.classList.remove('active'));
      event.target.classList.add('active');
      renderAllMatches();
    }

    function savePred(matchId) {
      const home = parseInt(document.getElementById(`h-${matchId}`).value);
      const away = parseInt(document.getElementById(`a-${matchId}`).value);

      if (isNaN(home) || isNaN(away)) {
        alert('Ingresa números válidos');
        return;
      }

      const match = allMatches.find(m => m.id === matchId);
      if (isMatchLocked(match)) {
        alert('Partido cerrado');
        return;
      }

      if (!allPredictions[matchId]) allPredictions[matchId] = {};
      allPredictions[matchId][currentUser.username] = { home, away, points: 0, exact: false };
      saveData();
      renderAllMatches();
    }

    function renderAdminPanel() {
      if (!currentUser.isAdmin) return;

      const stages = [...new Set(allMatches.map(m => m.stage))].sort();
      const filterGroup = document.getElementById('admin-filter-group');
      
      if (filterGroup.innerHTML === '') {
        filterGroup.innerHTML = stages.map(s => `
          <button class="filter-btn ${s === 'Grupos' ? 'active' : ''}" onclick="filterAdminMatches('${s}')" data-stage="${s}">${s}</button>
        `).join('');
      }

      const active = filterGroup.querySelector('.filter-btn.active');
      const currentStage = active?.getAttribute('data-stage') || 'Grupos';
      const matches = allMatches.filter(m => m.stage === currentStage);

      document.getElementById('admin-matches-list').innerHTML = matches.map(m => {
        const timeLeft = getTimeToDeadline(m);
        const isColombia = m.home === 'Colombia' || m.away === 'Colombia';

        return `
          <div class="match-card ${isColombia ? 'colombia' : ''}">
            <div class="match-header">
              <span style="font-size: 0.75rem;">${m.date} ${m.time}</span>
              <span class="status-badge status-${m.status}">${m.status === 'finished' ? '✓' : '⏱'}</span>
            </div>
            <div class="match-teams">
              <div class="team-home team-name">${m.home}</div>
              <div class="score-display">${m.scoreHome !== null ? `${m.scoreHome} - ${m.scoreAway}` : '-'}</div>
              <div class="team-away team-name">${m.away}</div>
            </div>
            ${timeLeft ? `<div class="countdown">Cierra en ${timeLeft}</div>` : ''}
            <div class="match-actions">
              ${m.status !== 'finished' ? `<button class="btn btn-primary btn-sm" onclick="openResultModal('${m.id}')">Resultado</button>` : ''}
              <button class="btn btn-ghost btn-sm" onclick="openDeadlineModal('${m.id}')">Límite</button>
              ${m.status === 'finished' && Object.keys(allPredictions[m.id] || {}).length > 0 ? `<button class="btn btn-gold btn-sm" onclick="openPointsModal('${m.id}')">Puntos</button>` : ''}
            </div>
          </div>
        `;
      }).join('');
    }

    function filterAdminMatches(stage) {
      document.querySelectorAll('#admin-tab-content .filter-btn').forEach(b => b.classList.remove('active'));
      event.target.classList.add('active');
      renderAdminPanel();
    }

    function openResultModal(matchId) {
      const match = allMatches.find(m => m.id === matchId);
      document.getElementById('result-modal').dataset.matchId = matchId;
      document.getElementById('result-home').value = match.scoreHome || '';
      document.getElementById('result-away').value = match.scoreAway || '';
      document.getElementById('result-error').style.display = 'none';
      document.getElementById('result-modal').classList.add('active');
    }

    function handleRegisterResult() {
      const matchId = document.getElementById('result-modal').dataset.matchId;
      const home = parseInt(document.getElementById('result-home').value);
      const away = parseInt(document.getElementById('result-away').value);
      const errorEl = document.getElementById('result-error');

      if (isNaN(home) || isNaN(away)) {
        showError(errorEl, 'Ingresa números válidos');
        return;
      }

      const match = allMatches.find(m => m.id === matchId);
      match.scoreHome = home;
      match.scoreAway = away;
      match.status = 'finished';
      
      saveData();
      closeModal('result-modal');
      renderAdminPanel();
      renderAllMatches();
      renderMyPredictions();
      renderLeaderboard();
    }

    function openDeadlineModal(matchId) {
      document.getElementById('deadline-modal').dataset.matchId = matchId;
      document.getElementById('hours-before-input').value = '1';
      document.getElementById('deadline-error').style.display = 'none';
      document.getElementById('deadline-modal').classList.add('active');
    }

    function handleSetDeadline() {
      const matchId = document.getElementById('deadline-modal').dataset.matchId;
      const hours = parseInt(document.getElementById('hours-before-input').value);
      const errorEl = document.getElementById('deadline-error');

      if (isNaN(hours) || hours < 0) {
        showError(errorEl, 'Ingresa un número válido');
        return;
      }

      const match = allMatches.find(m => m.id === matchId);
      const matchTime = new Date(`${match.date}T${match.time}`);
      const deadline = new Date(matchTime.getTime() - hours * 60 * 60 * 1000);

      match.deadline = deadline.toISOString();
      saveData();
      closeModal('deadline-modal');
      renderAdminPanel();
      renderAllMatches();
      renderMyPredictions();
    }

    function openPointsModal(matchId) {
      const match = allMatches.find(m => m.id === matchId);
      const preds = allPredictions[matchId] || {};
      const users = JSON.parse(localStorage.getItem(STORAGE_KEYS.users) || '[]');

      let html = '';
      Object.keys(preds).forEach(username => {
        const pred = preds[username];
        const user = users.find(u => u.username === username);
        const isExact = pred.home === match.scoreHome && pred.away === match.scoreAway;
        const isCorrect = !isExact && ((match.scoreHome > match.scoreAway && pred.home > pred.away) || 
                                       (match.scoreHome < match.scoreAway && pred.home < pred.away) ||
                                       (match.scoreHome === match.scoreAway && pred.home === pred.away));

        html += `
          <div style="padding: 1rem; background: var(--navy-light); border-radius: var(--radius); border: 1px solid var(--card-border);">
            <div style="font-weight: 500; margin-bottom: 0.75rem;">${user.name}</div>
            <div style="font-size: 0.85rem; color: var(--muted); margin-bottom: 0.75rem;">
              Predicción: ${pred.home} - ${pred.away}
            </div>
            <div class="form-group" style="margin-bottom: 0;">
              <label>Puntos Manuales</label>
              <input type="number" class="points-input" id="pts-${username}" value="${pred.points || 0}" min="0" max="10">
            </div>
          </div>
        `;
      });

      document.getElementById('points-list').innerHTML = html;
      document.getElementById('points-modal').dataset.matchId = matchId;
      document.getElementById('points-modal').classList.add('active');

      // Botón para guardar al final
      const btn = document.createElement('button');
      btn.className = 'btn btn-gold';
      btn.style.width = '100%';
      btn.style.marginTop = '1rem';
      btn.textContent = 'Guardar Puntos';
      btn.onclick = () => saveManualPoints(matchId);
      document.getElementById('points-list').parentElement.appendChild(btn);
    }

    function saveManualPoints(matchId) {
      const preds = allPredictions[matchId] || {};
      Object.keys(preds).forEach(username => {
        const inputVal = document.getElementById(`pts-${username}`);
        if (inputVal) {
          const points = parseInt(inputVal.value) || 0;
          preds[username].points = points;
          if (!allScores[username]) allScores[username] = 0;
          allScores[username] += points;
        }
      });
      saveData();
      closeModal('points-modal');
      renderAdminPanel();
      renderLeaderboard();
    }

    function closeModal(modalId) {
      document.getElementById(modalId).classList.remove('active');
    }

    function render() {
      renderLeaderboard();
      renderMyPredictions();
      renderAllMatches();
      renderAdminPanel();
    }

    function startCountdownUpdates() {
      setInterval(() => {
        if (!currentUser) return;
        renderAllMatches();
        renderMyPredictions();
      }, 30000);
    }

    window.addEventListener('DOMContentLoaded', init);
  </script>
</body>
</html>
