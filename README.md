
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>2026 버나비247 썸머스쿨 | 여름방학 특강수업</title>
<link href="https://fonts.googleapis.com/css2?family=Noto+Serif+KR:wght@400;600;700;900&family=Noto+Sans+KR:wght@300;400;500;700&family=Playfair+Display:ital,wght=0,700;0,900;1,700&display=swap" rel="stylesheet">
<style>
  :root {
    --primary: #f9d976; /* 따뜻한 노랑 */
    --primary-dark: #f0a04b; /* 주황색 */
    --primary-light: #fff8e1; /* 밝은 크림 */
    --accent: #2196f3; /* 여름 파랑 */
    --accent-dark: #1976d2; /* 짙은 파랑 */
    --accent-light: #bbdefb; /* 밝은 파랑 */
    --green: #2ecc71; /* 후기 버튼용 초록 계열 */
    --green-dark: #27ae60;
    --red: #d94040;
    --gold: #c8a84b;
    --navy: #1a2e3b;
    --off-white: #fdfaf5;
    --text: #1a1a1a;
    --gray: #6b7b80;
    --border: #e0e0e0;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  html { scroll-behavior: smooth; }

  body {
    font-family: 'Noto Sans KR', sans-serif;
    background: var(--off-white);
    color: var(--text);
    overflow-x: hidden;
    -webkit-text-size-adjust: none;
    background-image: url('https://images.unsplash.com/photo-1510414842594-a61c69b5ae57?q=80&w=2070&auto=format&fit=crop'); 
    background-attachment: fixed;
    background-size: cover;
    background-position: center;
  }

  body::before {
    content: '';
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    background: rgba(255, 255, 255, 0.8);
    z-index: -1;
  }

  /* ── 메인 콘텐츠 & 하위 등록 페이지 레이아웃 전환을 위한 설정 ── */
  #main-content, #register-page {
    transition: opacity 0.4s ease, transform 0.4s ease;
    width: 100%;
  }

  /* 숨김 처리 디자인 (슥 사라지는 효과) */
  .page-hidden {
    display: none !important;
    opacity: 0;
    transform: translateY(20px);
  }

  /* ── HERO ── */
  .hero {
    background: linear-gradient(160deg, #fff8e1 0%, #ffecb3 40%, #ffe082 100%);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 80px 20px;
    position: relative;
    overflow: hidden;
    text-align: center;
    border-bottom: 2px solid #ffcc80;
  }

  .hero::before {
    content: '';
    position: absolute;
    top: -120px; right: -120px;
    width: 500px; height: 500px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(255, 213, 79,0.3) 0%, transparent 70%);
    pointer-events: none;
  }
  .hero::after {
    content: '';
    position: absolute;
    bottom: -80px; left: -80px;
    width: 400px; height: 400px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(255, 183, 77,0.2) 0%, transparent 70%);
    pointer-events: none;
  }

  .hero-badge {
    display: inline-block;
    background: var(--primary-dark);
    color: #fff;
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.14em;
    padding: 6px 18px;
    border-radius: 30px;
    margin-bottom: 24px;
    animation: fadeDown 0.7s ease both;
  }

  .hero-title {
    font-family: 'Noto Serif KR', serif;
    font-size: clamp(2.2rem, 7vw, 5rem);
    font-weight: 900;
    line-height: 1.2;
    color: #5d4037;
    margin-bottom: 8px;
    animation: fadeDown 0.8s 0.1s ease both;
    word-break: keep-all;
  }

  .hero-title span {
    color: var(--accent);
    font-style: italic;
  }

  .hero-en {
    font-family: 'Playfair Display', serif;
    font-size: clamp(1.8rem, 6vw, 4.5rem);
    font-weight: 700;
    font-style: italic;
    color: var(--navy);
    letter-spacing: -0.01em;
    margin-bottom: 28px;
    animation: fadeDown 0.8s 0.2s ease both;
  }

  .hero-en em {
    color: var(--primary-dark);
    font-style: normal;
  }

  .hero-date {
    display: inline-block;
    background: var(--accent);
    color: #fff;
    font-size: clamp(0.95rem, 2.2vw, 1.3rem);
    font-weight: 700;
    padding: 12px 32px;
    border-radius: 50px;
    margin-bottom: 24px;
    animation: fadeDown 0.8s 0.3s ease both;
    box-shadow: 0 8px 32px rgba(33, 150, 243,0.25);
  }

  .hero-sub {
    font-size: 0.95rem;
    color: #6d4c41;
    font-weight: 500;
    letter-spacing: 0.02em;
    line-height: 1.5;
    padding: 0 10px;
    animation: fadeDown 0.8s 0.4s ease both;
    word-break: keep-all;
  }

  .hero-cta {
    margin-top: 36px;
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
    justify-content: center;
    animation: fadeDown 0.8s 0.5s ease both;
    width: 100%;
    max-width: 600px;
  }

  .btn-primary, .btn-secondary, .btn-green {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: 14px 28px;
    border-radius: 50px;
    font-size: 0.95rem;
    font-weight: 700;
    text-decoration: none;
    transition: all 0.2s;
    text-align: center;
    width: auto;
    min-width: 160px;
    cursor: pointer;
    border: none;
  }

  .btn-primary {
    background: var(--primary-dark);
    color: #fff;
    box-shadow: 0 6px 24px rgba(240, 160, 75,0.3);
  }
  .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 10px 32px rgba(240, 160, 75,0.4); }

  .btn-secondary {
    background: transparent;
    color: var(--accent);
    border: 2px solid var(--accent);
  }
  .btn-secondary:hover { background: var(--accent); color: #fff; }

  .btn-green {
    background: var(--green);
    color: #fff;
    box-shadow: 0 6px 24px rgba(46, 204, 113, 0.3);
  }
  .btn-green:hover { background: var(--green-dark); transform: translateY(-2px); box-shadow: 0 10px 32px rgba(46, 204, 113, 0.4); }

  /* ── SECTION COMMON ── */
  section { padding: 80px 20px; }

  .container { max-width: 900px; margin: 0 auto; position: relative; z-index: 1; }

  .section-label {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background: var(--primary-light);
    color: #e65100;
    font-size: 0.82rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    padding: 6px 18px;
    border-radius: 30px;
    margin-bottom: 16px;
    border: 1px solid #ffe082;
  }

  .section-title {
    font-family: 'Noto Serif KR', serif;
    font-size: clamp(1.5rem, 4vw, 2.4rem);
    font-weight: 900;
    color: var(--navy);
    margin-bottom: 10px;
    line-height: 1.3;
    word-break: keep-all;
  }

  .section-desc {
    color: var(--gray);
    font-size: 0.95rem;
    line-height: 1.6;
    margin-bottom: 36px;
    word-break: keep-all;
  }

  /* ── INFO GRID ── */
  .info-section { background: rgba(255, 255, 255, 0.9); }

  .info-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 0;
    border: 2px solid #ffe082;
    border-radius: 16px;
    overflow: hidden;
  }

  .info-cell {
    display: flex;
    align-items: flex-start;
    gap: 12px;
    padding: 18px 20px;
    border-bottom: 1px solid #ffe082;
    border-right: 1px solid #ffe082;
  }
  .info-cell:nth-child(2n) { border-right: none; }
  .info-cell:nth-last-child(-n+2) { border-bottom: none; }

  .info-label {
    flex-shrink: 0;
    background: var(--primary-dark);
    color: #fff;
    font-size: 0.72rem;
    font-weight: 700;
    padding: 3px 10px;
    border-radius: 20px;
    white-space: nowrap;
    margin-top: 2px;
  }
  .info-label.red { background: var(--accent); }
  .info-label.outline { background: transparent; color: #e65100; border: 1.5px solid var(--primary-dark); }

  .info-value {
    font-size: 0.92rem;
    font-weight: 500;
    line-height: 1.55;
    color: var(--text);
  }
  .info-value small {
    display: block;
    color: var(--accent);
    font-size: 0.8rem;
    margin-top: 2px;
  }

  /* ── FEATURES ── */
  .features-section { background: rgba(255, 248, 225, 0.9); }

  .features-grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 14px;
    margin-bottom: 14px;
  }
  .features-grid:last-child { margin-bottom: 0; }

  .feature-card {
    background: #fff;
    border-radius: 14px;
    padding: 20px 10px;
    text-align: center;
    box-shadow: 0 2px 12px rgba(240, 160, 75,0.08);
    border: 1px solid #ffe082;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .feature-card:hover { transform: translateY(-4px); box-shadow: 0 8px 28px rgba(240, 160, 75,0.16); }

  .feature-icon {
    font-size: 1.8rem;
    margin-bottom: 8px;
    display: block;
  }

  .feature-card .title {
    font-size: 0.8rem;
    font-weight: 500;
    color: var(--navy);
    line-height: 1.4;
    word-break: keep-all;
  }

  .feature-card .title strong {
    display: block;
    font-size: 0.88rem;
    font-weight: 700;
  }

  /* ── TIMETABLE ── */
  .schedule-section { background: rgba(255, 255, 255, 0.9); }

  .schedule-note {
    background: var(--primary-light);
    border-left: 4px solid var(--primary-dark);
    padding: 12px 16px;
    border-radius: 0 8px 8px 0;
    font-size: 0.85rem;
    color: #e65100;
    font-weight: 500;
    margin-bottom: 24px;
    word-break: keep-all;
  }

  .table-wrapper {
    width: 100%;
    overflow-x: auto;
    -webkit-overflow-scrolling: touch;
    border-radius: 12px;
    box-shadow: 0 2px 16px rgba(0,0,0,0.07);
    border: 1px solid #ffe082;
  }

  .timetable {
    width: 100%;
    border-collapse: collapse;
    font-size: 0.88rem;
    min-width: 580px;
  }

  .timetable thead tr {
    background: var(--primary-dark);
    color: #fff;
  }

  .timetable th {
    padding: 14px 16px;
    text-align: left;
    font-weight: 700;
    font-size: 0.82rem;
    letter-spacing: 0.04em;
  }

  .timetable td {
    padding: 14px 16px;
    border-bottom: 1px solid #ffe082;
    vertical-align: middle;
  }

  .timetable tr:last-child td { border-bottom: none; }
  .timetable tr:nth-child(even) td { background: var(--primary-light); }

  .tag-en { background: var(--accent); color: #fff; padding: 3px 10px; border-radius: 12px; font-size: 0.75rem; font-weight: 700; }
  .tag-math { background: var(--primary-dark); color: #fff; padding: 3px 10px; border-radius: 12px; font-size: 0.75rem; font-weight: 700; }
  .tag-self { background: #e8ecf0; color: var(--gray); padding: 3px 10px; border-radius: 12px; font-size: 0.75rem; }
  .time-str { font-weight: 700; color: #bf360c; white-space: nowrap; }
  .extra { font-size: 0.78rem; color: var(--accent-dark); font-weight: 700; }

  /* ── GALLERY ── */
  .gallery-section { background: var(--navy); }
  .gallery-section .section-title { color: #fff; }
  .gallery-section .section-desc { color: rgba(255,255,255,0.55); }

  .gallery-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 16px;
  }

  .gallery-card {
    border-radius: 16px;
    overflow: hidden;
    background: rgba(255,255,255,0.06);
    aspect-ratio: 16/10;
    display: flex;
    align-items: center;
    justify-content: center;
    border: 1px solid rgba(255,255,255,0.1);
    position: relative;
  }

  .gallery-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
    transition: transform 0.3s ease;
  }

  .gallery-card:hover img {
    transform: scale(1.03);
  }

  /* ── MESSAGE ── */
  .message-section { background: rgba(253, 250, 245, 0.9); }

  .message-card {
    background: #fff;
    border-radius: 20px;
    padding: 40px;
    box-shadow: 0 4px 32px rgba(240, 160, 75,0.06);
    border: 1px solid #ffe082;
    position: relative;
  }

  .message-card::before {
    content: 'TO.';
    font-family: 'Playfair Display', serif;
    font-size: 3.5rem;
    font-weight: 900;
    color: var(--primary-light);
    position: absolute;
    top: 20px; left: 30px;
    z-index: 0;
    line-height: 1;
  }

  .message-heading {
    font-family: 'Noto Serif KR', serif;
    font-size: 1.25rem;
    font-weight: 700;
    color: var(--navy);
    margin-bottom: 20px;
    position: relative;
    z-index: 1;
  }

  .message-body {
    font-size: 0.95rem;
    line-height: 1.8;
    color: #444;
    position: relative;
    z-index: 1;
    word-break: keep-all;
  }

  .message-body p { margin-bottom: 14px; }
  .message-body p:last-child { margin-bottom: 0; }
  .message-body strong { color: #bf360c; font-weight: 700; }

  .message-closing {
    font-family: 'Noto Serif KR', serif;
    font-size: 1.05rem;
    font-weight: 700;
    color: #bf360c;
    margin-top: 24px;
    padding-top: 20px;
    border-top: 1px solid #ffe082;
    position: relative;
    z-index: 1;
  }

  /* ── CTA BANNER ── */
  .cta-section {
    background: linear-gradient(135deg, var(--primary-dark) 0%, var(--primary) 100%);
    padding: 80px 20px;
    text-align: center;
    border-top: 2px solid #ffcc80;
  }

  .cta-section h2 {
    font-family: 'Noto Serif KR', serif;
    font-size: clamp(1.5rem, 4vw, 2.2rem);
    font-weight: 900;
    color: #5d4037;
    margin-bottom: 12px;
    word-break: keep-all;
  }

  .cta-section p {
    color: #6d4c41;
    font-size: 0.95rem;
    margin-bottom: 32px;
  }

  .cta-contact {
    display: flex;
    flex-wrap: wrap;
    gap: 14px;
    justify-content: center;
    align-items: center;
    max-width: 600px;
    margin: 0 auto;
  }

  .contact-chip {
    background: rgba(255,255,255,0.4);
    color: #5d4037;
    padding: 12px 24px;
    border-radius: 50px;
    font-size: 0.92rem;
    font-weight: 700;
    border: 1.5px solid #ffcc80;
    text-decoration: none;
    transition: background 0.2s;
    width: 100%;
    cursor: pointer;
  }
  .contact-chip:hover { background: rgba(255,255,255,0.6); }
  a.contact-chip, button.contact-chip { background: var(--accent); color: #fff; border-color: transparent; box-shadow: 0 4px 15px rgba(0,0,0,0.15); }
  a.contact-chip:hover, button.contact-chip:hover { background: var(--accent-dark); }
  
  a.contact-chip.blog-link { background: var(--green); }
  a.contact-chip.blog-link:hover { background: var(--green-dark); }

  /* ── FOOTER ── */
  footer {
    background: var(--navy);
    padding: 36px 20px;
    text-align: center;
  }

  .footer-logo {
    font-family: 'Playfair Display', serif;
    font-size: 1.05rem;
    font-weight: 700;
    color: var(--primary-light);
    letter-spacing: 0.06em;
    margin-bottom: 8px;
  }

  footer p {
    color: rgba(255,255,255,0.35);
    font-size: 0.78rem;
    line-height: 1.4;
  }

  /* ── REVEAL ANIMATIONS ── */
  @keyframes fadeDown {
    from { opacity: 0; transform: translateY(-12px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  .reveal {
    opacity: 0;
    transform: translateY(30px);
    transition: opacity 0.7s cubic-bezier(0.25, 1, 0.5, 1), transform 0.7s cubic-bezier(0.25, 1, 0.5, 1);
  }
  .reveal.visible {
    opacity: 1;
    transform: translateY(0);
  }

  /* ── 📝 독립된 하위 등록 페이지 디자인 스타일 ── */
  .register-screen {
    min-height: 100vh;
    padding: 60px 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #fff8e1 0%, #ffe082 100%);
  }
  .form-container {
    background: #fff;
    max-width: 550px;
    width: 100%;
    padding: 40px 30px;
    border-radius: 20px;
    box-shadow: 0 10px 40px rgba(0,0,0,0.08);
    border: 1px solid #ffe082;
    animation: fadeDown 0.5s ease both;
  }
  .form-container h2 {
    font-family: 'Noto Serif KR', serif;
    color: var(--navy);
    margin-bottom: 8px;
    font-size: 1.7rem;
    font-weight: 900;
    text-align: center;
  }
  .form-container .form-desc {
    text-align: center;
    font-size: 0.92rem;
    color: var(--gray);
    margin-bottom: 30px;
  }
  .form-group { margin-bottom: 20px; }
  .form-group label {
    display: block;
    font-weight: 700;
    font-size: 0.92rem;
    margin-bottom: 8px;
    color: var(--navy);
  }
  .form-group input[type="text"], .form-group input[type="tel"], .form-group select, .form-group textarea {
    width: 100%;
    padding: 14px;
    border: 1px solid #ffe082;
    border-radius: 10px;
    font-size: 0.95rem;
    font-family: inherit;
    background: #fdfaf5;
    transition: all 0.2s;
  }
  .form-group input:focus, .form-group select:focus, .form-group textarea:focus {
    outline: none;
    border-color: var(--primary-dark);
    background: #fff;
    box-shadow: 0 0 8px rgba(240, 160, 75, 0.2);
  }
  .checkbox-group {
    display: flex;
    gap: 16px;
    flex-wrap: wrap;
    margin-top: 8px;
  }
  .checkbox-group label {
    font-weight: 500;
    cursor: pointer;
    display: flex;
    align-items: center;
    gap: 6px;
  }
  .checkbox-group input[type="checkbox"] {
    width: 16px;
    height: 16px;
    accent-color: var(--primary-dark);
  }
  .form-submit-btn {
    background: var(--primary-dark);
    color: #fff;
    border: none;
    width: 100%;
    padding: 16px;
    font-size: 1.05rem;
    font-weight: 700;
    border-radius: 50px;
    cursor: pointer;
    margin-top: 15px;
    box-shadow: 0 6px 20px rgba(240, 160, 75, 0.3);
    transition: all 0.2s;
  }
  .form-submit-btn:hover { background: #e08f3a; transform: translateY(-2px); }
  .back-to-main-btn {
    display: block;
    text-align: center;
    margin-top: 20px;
    font-size: 0.92rem;
    color: var(--accent-dark);
    text-decoration: none;
    font-weight: 500;
  }
  .back-to-main-btn:hover { text-decoration: underline; }

  @media (max-width: 700px) {
    section { padding: 50px 16px; }
    
    .hero { padding: 60px 16px; }
    .hero-cta { flex-direction: column; align-items: center; width: 100%; }
    .btn-primary, .btn-secondary, .btn-green { width: 100%; max-width: 280px; }

    .info-grid { grid-template-columns: 1fr; border-radius: 12px; }
    .info-cell { border-right: none !important; padding: 14px 16px; border-bottom: 1px solid #ffe082 !important;}
    .info-cell:nth-last-child(-n+2) { border-bottom: 1px solid #ffe082 !important; }
    .info-cell:last-child { border-bottom: none !important; }

    .features-grid {
      grid-template-columns: repeat(2, 1fr);
      gap: 10px;
      margin-bottom: 10px;
    }
    .feature-card { padding: 16px 8px; border-radius: 12px; }
    .feature-icon { font-size: 1.6rem; margin-bottom: 6px; }

    .gallery-grid { grid-template-columns: 1fr; gap: 12px; }

    .message-card { padding: 32px 20px; border-radius: 16px; }
    .message-card::before { font-size: 2.6rem; top: 12px; left: 16px; }
    
    .contact-chip { padding: 12px 16px; font-size: 0.88rem; }
    .form-container { padding: 30px 20px; }
  }
</style>
</head>
<body>

<!-- ── 메인 콘텐츠 영역 ── -->
<div id="main-content">
  <section class="hero">
    <div class="hero-badge">2026 버나비247 STUDY CAMP</div>
    <h1 class="hero-title">여름방학 <span>특강수업</span></h1>
    <div class="hero-en"><em>Summer</em> School</div>
    <div class="hero-date">☀️ 2026년 7월 6일 개강 (예정)</div>
    <p class="hero-sub">뜨거운 열정으로 도약할 기회, 스터디캠프 버나비247에서 시작하세요!</p>
    <div class="hero-cta">
      <a href="#info" class="btn-primary">📋 모집 요강 보기</a>
      <!-- 클릭 시 하위 등록 페이지로 화면 전환 -->
      <button onclick="showRegisterPage()" class="btn-secondary">📞 등록 신청하기</button>
      <a href="https://blog.naver.com/bolton9929/224062244300" target="_blank" class="btn-green">✍️ 생생한 후기 보기</a>
    </div>
  </section>

  <section class="info-section" id="info">
    <div class="container">
      <div class="reveal">
        <div class="section-label">☀️ 모집 요강</div>
        <h2 class="section-title">뜨거운 여름, 몰입할 수험생을 모집합니다</h2>
        <p class="section-desc">예비 고1·고2·고3 및 N수생을 대상으로 수학·영어 집중 특강 및 관리형 자습을 진행합니다.</p>
      </div>
      <div class="info-grid reveal">
        <div class="info-cell">
          <span class="info-label">대상</span>
          <div class="info-value">예비 고1, 고2, 고3, N수생</div>
        </div>
        <div class="info-cell">
          <span class="info-label red">수업과목</span>
          <div class="info-value">수학, 영어, 관리형 자습</div>
        </div>
        <div class="info-cell">
          <span class="info-label">수업기간</span>
          <div class="info-value">26년 7월 6일(월) ~ 26년 8월 14일(금)<br><small style="color:var(--gray);font-size:0.78rem;">총 40일 (예정, 학사일정에 따라 변동 가능)</small></div>
        </div>
        <div class="info-cell">
          <span class="info-label red">운영형태</span>
          <div class="info-value">통학형 (월~금 9:00~22:00, 토 9:00~18:00)</div>
        </div>
        <div class="info-cell">
          <span class="info-label outline">사전예약</span>
          <div class="info-value">26년 5월 1일 ~ 26년 6월 19일</div>
        </div>
        <div class="info-cell">
          <span class="info-label outline">인원</span>
          <div class="info-value">25명 <small style="color:var(--gray);font-size:0.8rem;">(결제순 마감)</small></div>
        </div>
        <div class="info-cell">
          <span class="info-label outline">등록방법</span>
          <div class="info-value">010-2898-9929 문자 또는 온라인 등록</div>
        </div>
        <div class="info-cell">
          <span class="info-label outline">참가비</span>
          <div class="info-value">별도 문의
            <small>수강 과목 및 기간에 따라 상이</small>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="features-section">
    <div class="container">
      <div class="reveal">
        <div class="section-label">⭐ 썸머스쿨 특징</div>
        <h2 class="section-title">지치지 않는 여름, 체계적인 관리</h2>
        <p class="section-desc">버나비247만의 몰입 학습 시스템으로 여름방학을 알차게 보냅니다.</p>
      </div>
      <div class="features-grid reveal">
        <div class="feature-card">
          <span class="feature-icon">💧</span>
          <div class="title">시원하고 쾌적한<strong>학습 환경</strong></div>
        </div>
        <div class="feature-card">
          <span class="feature-icon">📚</span>
          <div class="title">몰입이 가능한<strong>개인별 지정석</strong></div>
        </div>
        <div class="feature-card">
          <span class="feature-icon">☀️</span>
          <div class="title">규칙적인 생활<strong>학습 습관 형성</strong></div>
        </div>
        <div class="feature-card">
          <span class="feature-icon">🤝</span>
          <div class="title">1:1 학습 멘토링<strong>컨설팅</strong></div>
        </div>
        <div class="feature-card">
          <span class="feature-icon">🎯</span>
          <div class="title">단기간 집중<strong>성적 향상 전략</strong></div>
        </div>
      </div>
      <div class="features-grid reveal">
        <div class="feature-card">
          <span class="feature-icon">⏱️</span>
          <div class="title">순공 시간 확보<strong>엄격한 교시제</strong></div>
        </div>
        <div class="feature-card">
          <span class="feature-icon">✅</span>
          <div class="title">실시간 출결·생활<strong>밀착형 관리</strong></div>
        </div>
        <div class="feature-card">
          <span class="feature-icon">📈</span>
          <div class="title">매주 실전 모의고사<strong>성취도 점검</strong></div>
        </div>
        <div class="feature-card">
          <span class="feature-icon">🔥</span>
          <div class="title">공부 자극<strong>강력한 학구열</strong></div>
        </div>
        <div class="feature-card">
          <span class="feature-icon">🍦</span>
          <div class="title">열공 응원<strong>스낵&음료 제공</strong></div>
        </div>
      </div>
    </div>
  </section>

  <section class="schedule-section" id="schedule">
    <div class="container">
      <div class="reveal">
        <div class="section-label">🕐 시간표</div>
        <h2 class="section-title">하루 일과표 (예시)</h2>
      </div>
      <div class="schedule-note reveal">📌 평일 기준 표준 시간표이며, 개별 과목 수강 및 자습 계획에 따라 변동될 수 있습니다.</div>
      <div class="table-wrapper reveal">
        <table class="timetable">
          <thead>
            <tr>
              <th>#</th>
              <th>시간</th>
              <th>과목/활동</th>
              <th>내용</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>—</td>
              <td><span class="time-str">~ 09:00</span></td>
              <td>등원</td>
              <td>등원 및 학습 준비</td>
            </tr>
            <tr>
              <td>1</td>
              <td><span class="time-str">09:00–10:30</span></td>
              <td><span class="tag-en">영어수업/자습</span></td>
              <td>수능/모의고사 독해 실전 및 Q&A</td>
            </tr>
            <tr>
              <td>2</td>
              <td><span class="time-str">10:40–12:10</span></td>
              <td><span class="tag-math">수학수업/자습</span></td>
              <td>핵심 개념 및 유형 정복</td>
            </tr>
            <tr>
              <td>—</td>
              <td><span class="time-str">12:10–13:10</span></td>
              <td>점심</td>
              <td>점심시간</td>
            </tr>
            <tr>
              <td>3</td>
              <td><span class="time-str">13:10–14:40</span></td>
              <td><span class="tag-math">수학수업/자습</span></td>
              <td>심화 문제 해결력 키우기</td>
            </tr>
            <tr>
              <td>4</td>
              <td><span class="time-str">14:50–16:20</span></td>
              <td><span class="tag-self">몰입 자습</span></td>
              <td>자기주도 학습 및 피드백</td>
            </tr>
            <tr>
              <td>5</td>
              <td><span class="time-str">16:30–18:00</span></td>
              <td><span class="tag-self">몰입 자습</span></td>
              <td>자기주도 학습 및 1:1 질의응답</td>
            </tr>
            <tr>
              <td>—</td>
              <td><span class="time-str">18:00–19:00</span></td>
              <td>저녁</td>
              <td>저녁시간</td>
            </tr>
            <tr>
              <td>6</td>
              <td><span class="time-str">19:00–20:30</span></td>
              <td><span class="tag-self">몰입 자습</span></td>
              <td>당일 복습 및 과제 수행</td>
            </tr>
            <tr>
              <td>7</td>
              <td><span class="time-str">20:40–22:00</span></td>
              <td><span class="tag-self">몰입 자습</span></td>
              <td>심화 학습 및 다음날 준비</td>
            </tr>
            <tr>
              <td>—</td>
              <td><span class="time-str">22:00 ~</span></td>
              <td>하원</td>
              <td>하원 및 귀가</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div style="margin-top:18px; font-size:0.82rem; color:var(--gray); line-height:1.8;" class="reveal">
        • 실제 수업 시간표는 학원 사정 및 학생별 수강 신청 현황에 따라 확정됩니다.<br>
        • 토요일은 오전 9시부터 오후 6시까지 자율형 관리 자습이 운영됩니다.
      </div>
    </div>
  </section>

  <section class="gallery-section">
    <div class="container">
      <div class="reveal">
        <div class="section-label" style="background:rgba(255,255,255,0.1);color:rgba(255,255,255,0.8);border-color:rgba(255,255,255,0.2);">📸 현장 사진</div>
        <h2 class="section-title">버나비247 학습 현장</h2>
        <p class="section-desc">시원하고 쾌적한 환경에서 학업에 완전 몰입하고 있는 전경입니다.</p>
      </div>
      <div class="gallery-grid reveal">
        <div class="gallery-card">
          <img src="./344.jpg" alt="버나비247 자습 전경">
        </div>
        <div class="gallery-card">
          <img src="./41123.jpg" alt="버나비247 강의 및 자습 공간">
        </div>
      </div>
    </div>
  </section>

  <section class="message-section">
    <div class="container">
      <div class="reveal">
        <div class="section-label">💌 원장 메시지</div>
        <h2 class="section-title">'더 큰 나'로 성장할 여름을 꿈꾸는 여러분께</h2>
      </div>
      <div class="message-card reveal">
        <div class="message-heading">'더 큰 나'로 성장할 여름을 꿈꾸는 여러분께</div>
        <div class="message-body">
          <p>버나비 247 썸머스쿨은 <strong>무더운 여름, 지치지 않고 학습에 몰입할 수 있도록</strong> 최적의 환경과 <strong>체계적인 학습 관리 시스템을 제공</strong>하여 학생이 스스로 학습을 주도하고 성취감을 맛볼 수 있도록 설계된 프로그램입니다.</p>
          <p><strong>수학과 영어 핵심 개념을 완벽히 정리하고, 실전 문제 해결력을 기르는 특강</strong>과 더불어 <strong>순수 공부 시간을 극대화하는 몰입 자습</strong>을 통해 학업 역량을 단기간에 끌어올립니다.</p>
          <p>이 모든 과정은 <strong>단순한 지식 습득을 넘어, 올바른 학습 습관을 형성하고 자기주도적 학습 능력을 훈련</strong>시키는 데에 초점이 맞춰져 있으며, 1:1 멘토링을 통해 동기 부여와 학습 방향을 지속적으로 점검합니다.</p>
          <p>이번 여름, 버나비247에서 <strong>'성장의 주인공'</strong>이 되어 가을에 더 높은 곳으로 도약하는 경험을 시작해보세요.</p>
        </div>
        <div class="message-closing">여러분의 뜨거운 도전을 응원합니다. 🔥</div>
      </div>
    </div>
  </section>

  <section class="cta-section" id="contact">
    <div class="container">
      <h2>지금 바로 여름을 선점하세요</h2>
      <p>선착순 25명 마감 · 조기 등록 혜택 제공</p>
      <div class="cta-contact">
        <!-- 클릭 시 하위 등록 페이지로 화면 전환 -->
        <button onclick="showRegisterPage()" class="contact-chip">📝 온라인 등록 신청하기</button>
        <a href="https://blog.naver.com/bolton9929/224062244300" target="_blank" class="contact-chip blog-link">✍️ 생생한 후기 보기 (블로그)</a>
        <div class="contact-chip">📅 사전예약: ~26년 6월 19일</div>
        <div class="contact-chip">💰 참가비: 문의 요망</div>
      </div>
    </div>
  </section>

  <footer>
    <div class="footer-logo">☀️ STUDY CAMP BURNABY 247</div>
    <p>2026 버나비247 여름방학 특강수업 &amp; Summer School</p>
  </footer>
</div>


<!-- ── 📝 하위 등록 페이지 영역 (평소에는 완전히 숨겨짐) ── -->
<div id="register-page" class="page-hidden">
  <div class="register-screen">
    <div class="form-container">
      <h2>📝 썸머스쿨 등록 신청</h2>
      <p class="form-desc">학습 매니저가 확인 후 신속하게 연락드리겠습니다.</p>
      
      <!-- 구글 폼, 네이버 폼 등 전송 링크를 넣거나 연락망 구축 가능 -->
      <form onsubmit="alert('등록 신청이 완료되었습니다! 확인 후 연락드리겠습니다.'); hideRegisterPage(); return false;">
        <div class="form-group">
          <label for="student_name">학생 이름</label>
          <input type="text" id="student_name" placeholder="학생 성명을 입력하세요" required>
        </div>
        
        <div class="form-group">
          <label for="phone_number">연락처 (학부모 또는 학생)</label>
          <input type="tel" id="phone_number" placeholder="010-0000-0000" required>
        </div>
        
        <div class="form-group">
          <label for="student_grade">현재 학년</label>
          <select id="student_grade" required>
            <option value="">학년을 선택해주세요</option>
            <option value="예비고1">예비 고1</option>
            <option value="예비고2">예비 고2</option>
            <option value="예비고3">예비 고3</option>
            <option value="N수생">N수생</option>
          </select>
        </div>
        
        <div class="form-group">
          <label>희망 수강 선택</label>
          <div class="checkbox-group">
            <label><input type="checkbox" name="subject" value="수학"> 수학 집중 특강</label>
            <label><input type="checkbox" name="subject" value="영어"> 영어 실전 특강</label>
            <label><input type="checkbox" name="subject" value="자습"> 247 관리형 자습</label>
          </div>
        </div>
        
        <div class="form-group">
          <label for="student_memo">전하고 싶은 말씀 / 문의사항</label>
          <textarea id="student_memo" rows="3" placeholder="상담 시 참고할 내용이나 질문을 적어주세요."></textarea>
        </div>
        
        <button type="submit" class="form-submit-btn">신청서 제출하기</button>
        <button type="button" onclick="hideRegisterPage()" class="back-to-main-btn">← 메인 화면으로 돌아가기</button>
      </form>
    </div>
  </div>
</div>


<script>
  // 스크롤 반응형 애니메이션 (위아래 계속 반응형 구현)
  const reveals = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry) => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
      } else {
        entry.target.classList.remove('visible');
      }
    });
  }, { 
    threshold: 0.1,
    rootMargin: "0px 0px -50px 0px"
  });
  reveals.forEach(el => observer.observe(el));

  // ── 싱글 페이지 전환 자바스크립트 제어 ──
  let lastScrollY = 0; // 메인화면 복귀 시 원래 스크롤 위치 기억용 변수

  function showRegisterPage() {
    lastScrollY = window.scrollY; // 현재 스크롤 위치 저장
    
    document.getElementById('main-content').classList.add('page-hidden');
    document.getElementById('register-page').classList.remove('page-hidden');
    
    window.scrollTo(0, 0); // 하위 페이지 최상단으로 스크롤 이동
  }

  function hideRegisterPage() {
    document.getElementById('register-page').classList.add('page-hidden');
    document.getElementById('main-content').classList.remove('page-hidden');
    
    // 이전에 저장했던 스크롤 위치로 부드럽게 원상 복구
    window.scrollTo({
      top: lastScrollY,
      behavior: 'auto'
    });
  }
</script>
</body>
</html>
