<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Hypno-coaching en visio — Karl Kandot</title>
  <meta name="description" content="Hypno-coaching en visioconférence : combinez l'hypnose éricksonienne et le coaching pour retrouver calme, clarté et ressources. Séances en visio, partout en France." />
  <meta property="og:title" content="Hypno-coaching en visio — Karl Kandot" />
  <meta property="og:description" content="Retrouvez calme, clarté et ressources grâce à l'hypno-coaching en visio. Coaching + hypnose éricksonienne, partout en France." />
  <meta property="og:type" content="website" />
  <script>
    // Applique le thème mémorisé avant le premier rendu (évite le flash visuel)
    (function() {
      try {
        var stored = localStorage.getItem('theme');
        var theme = stored || (matchMedia('(prefers-color-scheme:dark)').matches ? 'dark' : 'light');
        document.documentElement.setAttribute('data-theme', theme);
      } catch (e) {}
    })();
  </script>
  <link rel="icon" type="image/svg+xml" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 32 32'%3E%3Ccircle cx='16' cy='16' r='14' fill='%23F2F5F8' stroke='%23CA3C66' stroke-width='1.5'/%3E%3Cpath d='M10 16 Q16 8, 22 16 Q16 24, 10 16' stroke='%23D65F82' stroke-width='1.5' fill='none'/%3E%3Ccircle cx='16' cy='16' r='3' fill='%23CA3C66'/%3E%3C/svg%3E" />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600&family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet" />

  <style>
    /* ============================================================
       DESIGN TOKENS — Charte graphique Karl Kandot
       Quiet Luxury — Blanc Albâtre, encre, accent bordeaux
       ============================================================ */
    :root {
      --text-xs: clamp(0.75rem, 0.7rem + 0.25vw, 0.875rem);
      --text-sm: clamp(0.875rem, 0.8rem + 0.35vw, 1rem);
      --text-base: clamp(1rem, 0.95rem + 0.25vw, 1.125rem);
      --text-lg: clamp(1.125rem, 1rem + 0.75vw, 1.5rem);
      --text-xl: clamp(1.5rem, 1.2rem + 1.25vw, 2.25rem);
      --text-2xl: clamp(2rem, 1.2rem + 2.5vw, 3.5rem);

      --space-1: 0.25rem; --space-2: 0.5rem; --space-3: 0.75rem;
      --space-4: 1rem; --space-5: 1.25rem; --space-6: 1.5rem;
      --space-8: 2rem; --space-10: 2.5rem; --space-12: 3rem;
      --space-16: 4rem; --space-20: 5rem; --space-24: 6rem;
      --space-32: 8rem;

      /* Palette — Blanc pur en fond, reste inchangé (Quiet Luxury) */
      --color-bg: #FFFFFF;
      --color-surface: #FFFFFF;
      --color-surface-2: #EBEFF4;
      --color-card: #B6D8F2;
      --color-border: #DDE3EC;
      --color-divider: #E4E9F0;

      --color-text: #1C1B19;
      --color-text-muted: #6B6964;
      --color-text-faint: #A09E98;

      --color-accent: #CA3C66;
      --color-accent-hover: #A62C50;
      --color-accent-light: #D65F82;
      /* Fond (glow) en vieux rose / blush — harmonisé clair/sombre */
      --color-accent-glow: rgba(216, 167, 177, 0.18);

      --color-gold: #B8941E;

      --radius-sm: 0.375rem;
      --radius-md: 0.5rem;
      --radius-lg: 0.75rem;
      --radius-xl: 1rem;
      --radius-full: 9999px;

      --transition: 250ms cubic-bezier(0.16, 1, 0.3, 1);

      /* Ombres chaudes, angle droit comme un soleil à peine perceptible */
      --shadow-sm: -1px 2px 4px rgba(80,65,45,0.05);
      --shadow-md: -3px 4px 12px rgba(80,65,45,0.07);
      --shadow-lg: -6px 8px 28px rgba(80,65,45,0.09);
      --shadow-glow: 0 0 40px var(--color-accent-glow);

      --content-narrow: 640px;
      --content-default: 960px;
      --content-wide: 1200px;

      --font-display: 'Cormorant Garamond', Georgia, serif;
      --font-body: 'Inter', -apple-system, BlinkMacSystemFont, 'SF Pro Display', sans-serif;
    }

    /* Dark mode (optionnel, via toggle) */
    [data-theme='dark'] {
      --color-bg: #0B1020;
      --color-surface: #131A2E;
      --color-surface-2: #1A2238;
      --color-card: #B6D8F2;
      --color-border: #2D3548;
      --color-divider: #252D40;

      --color-text: #E8E9ED;
      --color-text-muted: #9CA3B4;
      --color-text-faint: #6B7180;

      --color-accent: #CA3C66;
      --color-accent-hover: #E0567D;
      --color-accent-light: #E0779A;
      --color-accent-glow: rgba(216, 167, 177, 0.18);

      --color-gold: #C9A961;
      /* Ombres lunaires — Or sablé, angle droit, lueur pleine lune */
      --shadow-sm: -1px 2px 6px rgba(201,169,97,0.12);
      --shadow-md: -3px 5px 16px rgba(201,169,97,0.15);
      --shadow-lg: -6px 10px 36px rgba(201,169,97,0.18);
    }

    /* ============================================================
       BASE STYLES
       ============================================================ */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html {
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      text-rendering: optimizeLegibility;
      scroll-behavior: smooth;
      scroll-padding-top: 80px;
    }

    body {
      min-height: 100dvh;
      line-height: 1.65;
      font-family: var(--font-body);
      font-size: var(--text-base);
      color: var(--color-text);
      background-color: var(--color-bg);
    }

    h1, h2, h3, h4 {
      text-wrap: balance;
      line-height: 1.15;
      font-family: var(--font-display);
      font-weight: 500;
      letter-spacing: -0.01em;
    }
    p, li { text-wrap: pretty; max-width: 72ch; }

    a { color: var(--color-accent-light); text-decoration: none; transition: color var(--transition); }
    a:hover { color: var(--color-accent-hover); }

    img, picture, svg { display: block; max-width: 100%; height: auto; }

    ::selection { background: var(--color-accent); color: #fff; }

    :focus-visible { outline: 2px solid var(--color-accent-light); outline-offset: 3px; border-radius: var(--radius-sm); }

    button { cursor: pointer; background: none; border: none; font: inherit; color: inherit; }

    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after { animation-duration: 0.01ms !important; transition-duration: 0.01ms !important; scroll-behavior: auto !important; }
    }

    /* ============================================================
       LAYOUT
       ============================================================ */
    .container {
      width: 100%;
      max-width: var(--content-wide);
      margin-inline: auto;
      padding-inline: var(--space-6);
    }
    .container-narrow { max-width: var(--content-narrow); }

    section { padding-block: clamp(var(--space-12), 6vw, var(--space-24)); }

    .section-label {
      font-family: var(--font-body);
      font-size: var(--text-xs);
      font-weight: 600;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--color-accent-light);
      margin-bottom: var(--space-4);
    }

    .section-title {
      font-family: var(--font-display);
      font-size: var(--text-xl);
      font-weight: 500;
      letter-spacing: -0.01em;
      color: var(--color-text);
      margin-bottom: var(--space-3);
    }

    .section-intro {
      font-family: var(--font-body);
      font-weight: 400;
      color: var(--color-text-muted);
      font-size: var(--text-base);
      max-width: 60ch;
      margin-bottom: var(--space-10);
    }

    /* ============================================================
       HEADER
       ============================================================ */
    .header {
      position: sticky;
      top: 0;
      z-index: 50;
      background: color-mix(in oklab, var(--color-bg) 90%, transparent);
      backdrop-filter: blur(16px);
      border-bottom: 1px solid var(--color-divider);
    }
    .header__inner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding-block: var(--space-4);
    }
    .logo {
      display: flex;
      align-items: center;
      gap: var(--space-3);
      font-family: var(--font-display);
      font-size: var(--text-lg);
      color: var(--color-text);
      font-weight: 600;
      letter-spacing: 0.05em;
      text-transform: uppercase;
    }
    .logo svg { width: 32px; height: 32px; }
    .nav { display: flex; align-items: center; gap: var(--space-6); }
    .nav a {
      font-family: var(--font-body);
      font-size: var(--text-xs);
      font-weight: 400;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--color-text-muted);
    }
    .nav a:hover { color: var(--color-text); }
    .nav__toggle {
      display: none;
      width: 40px; height: 40px;
      align-items: center; justify-content: center;
    }
    .nav__toggle svg { width: 24px; height: 24px; }

    .theme-toggle {
      width: 36px; height: 36px;
      display: flex; align-items: center; justify-content: center;
      border-radius: var(--radius-full);
      color: var(--color-text-muted);
      transition: all var(--transition);
    }
    .theme-toggle:hover { color: var(--color-text); background: var(--color-surface); }

    @media (max-width: 768px) {
      .nav { display: none; }
      .nav__toggle { display: flex; }
    }

    /* ============================================================
       HERO
       ============================================================ */
    .hero {
      position: relative;
      padding-block: clamp(var(--space-20), 10vw, var(--space-32));
      overflow: hidden;
    }
    .hero::before {
      content: '';
      position: absolute;
      top: -20%; right: -10%;
      width: 600px; height: 600px;
      background: radial-gradient(circle, var(--color-accent-glow), transparent 70%);
      pointer-events: none;
    }
    .hero__content { position: relative; z-index: 1; max-width: 720px; }
    .hero .container {
      display: grid;
      grid-template-columns: 1.3fr 1fr;
      gap: var(--space-12);
      align-items: center;
    }
    .hero__visual {
      position: relative;
      z-index: 1;
      aspect-ratio: 4/5;
      border-radius: var(--radius-xl);
      overflow: hidden;
      border: 1px solid var(--color-border);
      box-shadow: var(--shadow-lg);
    }
    .hero__visual img {
      width: 100%; height: 100%;
      object-fit: cover;
      display: block;
    }
    @media (max-width: 900px) {
      .hero .container { grid-template-columns: 1fr; }
      .hero__visual { max-width: 420px; margin-inline: auto; order: -1; }
    }
    .hero__label {
      display: inline-flex;
      align-items: center;
      gap: var(--space-2);
      font-family: var(--font-body);
      font-size: var(--text-xs);
      font-weight: 600;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--color-accent-light);
      padding: var(--space-2) var(--space-4);
      border: 1px solid var(--color-accent);
      border-radius: var(--radius-full);
      margin-bottom: var(--space-6);
    }
    .hero h1 {
      font-family: var(--font-display);
      font-size: var(--text-2xl);
      font-weight: 500;
      letter-spacing: -0.02em;
      line-height: 1.1;
      margin-bottom: var(--space-6);
    }
    .hero h1 em {
      color: var(--color-accent-light);
      font-style: italic;
      font-weight: 500;
    }
    .hero__subtitle {
      font-family: var(--font-body);
      font-size: var(--text-lg);
      font-weight: 300;
      color: var(--color-text-muted);
      max-width: 56ch;
      margin-bottom: var(--space-8);
    }
    .hero__actions { display: flex; gap: var(--space-4); flex-wrap: wrap; }

    .btn {
      display: inline-flex;
      align-items: center;
      gap: var(--space-2);
      padding: var(--space-4) var(--space-8);
      font-family: var(--font-body);
      font-size: var(--text-xs);
      font-weight: 600;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      border-radius: var(--radius-full);
      transition: all var(--transition);
      text-decoration: none;
    }
    .btn--primary {
      background: var(--color-accent);
      color: #fff;
    }
    .btn--primary:hover {
      background: var(--color-accent-hover);
      color: #fff;
      transform: translateY(-2px);
      box-shadow: var(--shadow-md);
    }
    .btn--ghost {
      color: var(--color-text);
      border: 1px solid var(--color-border);
    }
    .btn--ghost:hover {
      border-color: var(--color-accent);
      color: var(--color-accent-light);
    }

    .hero__quote {
      margin-top: var(--space-12);
      padding-left: var(--space-6);
      border-left: 3px solid var(--color-accent);
      max-width: 520px;
    }
    .hero__quote p {
      font-family: var(--font-display);
      font-size: var(--text-base);
      font-style: italic;
      font-weight: 400;
      color: var(--color-text-muted);
      line-height: 1.6;
    }
    .hero__quote cite {
      display: block;
      margin-top: var(--space-2);
      font-family: var(--font-body);
      font-size: var(--text-xs);
      color: var(--color-text-faint);
      font-style: normal;
      font-weight: 400;
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }

    /* ============================================================
       POUR QUI
       ============================================================ */
    .for-whom__visual {
      width: 100%;
      max-height: 340px;
      border-radius: var(--radius-xl);
      overflow: hidden;
      margin-bottom: var(--space-10);
      border: 1px solid var(--color-border);
    }
    .for-whom__visual img {
      width: 100%; height: 340px;
      object-fit: cover;
      object-position: center 25%;
      display: block;
    }
    .for-whom__grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: var(--space-6);
    }
    .for-whom__card {
      background: var(--color-card);
      border: 1px solid var(--color-border);
      border-radius: var(--radius-lg);
      padding: var(--space-6);
      transition: all var(--transition);
    }
    .for-whom__card:hover {
      border-color: var(--color-accent);
      transform: translateY(-4px);
      box-shadow: var(--shadow-md);
    }
    .for-whom__icon {
      width: 40px; height: 40px;
      display: flex; align-items: center; justify-content: center;
      border-radius: var(--radius-md);
      background: var(--color-accent-glow);
      color: var(--color-accent-light);
      margin-bottom: var(--space-4);
    }
    .for-whom__card h3 {
      font-family: var(--font-display);
      font-size: var(--text-lg);
      font-weight: 600;
      margin-bottom: var(--space-2);
    }
    .for-whom__card p {
      font-size: var(--text-sm);
      color: var(--color-text-muted);
    }

    /* ============================================================
       CE QUE CE N'EST PAS
       ============================================================ */
    .not-section {
      background: var(--color-surface);
    }
    .not-section__box {
      background: var(--color-card);
      border: 1px solid var(--color-border);
      border-left: 3px solid var(--color-gold);
      border-radius: var(--radius-lg);
      padding: var(--space-8);
    }
    .not-section__box p {
      color: var(--color-text-muted);
      font-size: var(--text-sm);
    }
    .not-section__box strong { color: var(--color-text); }

    /* ============================================================
       PACKS / OFFRES
       ============================================================ */
    .packs__grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: var(--space-6);
    }
    .pack {
      background: var(--color-card);
      border: 1px solid var(--color-border);
      border-radius: var(--radius-lg);
      padding: var(--space-8);
      display: flex;
      flex-direction: column;
      transition: all var(--transition);
      position: relative;
    }
    .pack:hover {
      border-color: var(--color-accent);
      transform: translateY(-4px);
      box-shadow: var(--shadow-lg), var(--shadow-glow);
    }
    .pack--featured {
      border-color: var(--color-accent);
      box-shadow: var(--shadow-glow);
    }
    .pack__badge {
      position: absolute;
      top: -12px; right: var(--space-6);
      background: var(--color-accent);
      color: #fff;
      font-family: var(--font-body);
      font-size: 0.625rem;
      font-weight: 600;
      padding: var(--space-1) var(--space-4);
      border-radius: var(--radius-full);
      letter-spacing: 0.15em;
      text-transform: uppercase;
    }
    .pack__name {
      font-family: var(--font-display);
      font-size: var(--text-xl);
      font-weight: 600;
      margin-bottom: var(--space-2);
      letter-spacing: -0.01em;
    }
    .pack__tagline {
      font-size: var(--text-sm);
      color: var(--color-text-muted);
      margin-bottom: var(--space-6);
    }
    .pack__price {
      font-size: var(--text-xl);
      font-weight: 700;
      color: var(--color-text);
      margin-bottom: var(--space-1);
    }
    .pack__price-detail {
      font-size: var(--text-xs);
      color: var(--color-text-faint);
      margin-bottom: var(--space-6);
    }
    .pack__features {
      list-style: none;
      flex: 1;
      margin-bottom: var(--space-6);
    }
    .pack__features li {
      display: flex;
      align-items: flex-start;
      gap: var(--space-3);
      font-size: var(--text-sm);
      color: var(--color-text-muted);
      margin-bottom: var(--space-3);
    }
    .pack__features li::before {
      content: '';
      flex-shrink: 0;
      width: 6px; height: 6px;
      border-radius: 50%;
      background: var(--color-accent-light);
      margin-top: 8px;
    }
    .pack__btn {
      width: 100%;
      justify-content: center;
    }

    .packs__note {
      text-align: center;
      margin-top: var(--space-8);
      font-size: var(--text-sm);
      color: var(--color-text-faint);
    }

    /* Séance unitaire */
    .single-session {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-6);
      background: var(--color-card);
      border: 1px solid var(--color-border);
      border-radius: var(--radius-lg);
      padding: var(--space-6) var(--space-8);
      margin-top: var(--space-6);
      flex-wrap: wrap;
    }
    .single-session__info h3 {
      font-family: var(--font-display);
      font-size: var(--text-lg);
      font-weight: 600;
      margin-bottom: var(--space-1);
    }
    .single-session__info p {
      font-size: var(--text-sm);
      color: var(--color-text-muted);
    }
    .single-session__price {
      font-size: var(--text-lg);
      font-weight: 700;
    }

    /* ============================================================
       DÉROULÉ
       ============================================================ */
    .process__steps {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: var(--space-6);
      counter-reset: step;
    }
    .process__step {
      position: relative;
      padding-top: var(--space-12);
    }
    .process__step::before {
      counter-increment: step;
      content: counter(step);
      position: absolute;
      top: 0; left: 0;
      width: 36px; height: 36px;
      display: flex; align-items: center; justify-content: center;
      font-family: var(--font-display);
      font-size: var(--text-lg);
      color: var(--color-accent-light);
      border: 1px solid var(--color-accent);
      border-radius: 50%;
    }
    .process__step h3 {
      font-family: var(--font-display);
      font-size: var(--text-lg);
      font-weight: 600;
      margin-bottom: var(--space-2);
    }
    .process__step p {
      font-size: var(--text-sm);
      color: var(--color-text-muted);
    }

    /* ============================================================
       À PROPOS
       ============================================================ */
    .about {
      background: var(--color-surface);
    }
    .about__grid {
      display: grid;
      grid-template-columns: 1fr 1.5fr;
      gap: var(--space-12);
      align-items: center;
    }
    @media (max-width: 768px) {
      .about__grid { grid-template-columns: 1fr; }
    }
    .about__visual {
      aspect-ratio: 1;
      border-radius: var(--radius-xl);
      background: linear-gradient(135deg, var(--color-surface-2), var(--color-card));
      border: 1px solid var(--color-border);
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }
    .about__visual svg { width: 60%; height: auto; opacity: 0.9; }
    .about__text h2 {
      font-family: var(--font-display);
      font-size: var(--text-xl);
      font-weight: 500;
      margin-bottom: var(--space-4);
    }
    .about__text p {
      color: var(--color-text-muted);
      margin-bottom: var(--space-4);
    }
    .about__credentials {
      display: flex;
      flex-wrap: wrap;
      gap: var(--space-3);
      margin-top: var(--space-6);
    }
    .about__credential {
      display: inline-flex;
      align-items: center;
      gap: var(--space-2);
      font-family: var(--font-body);
      font-size: 0.6875rem;
      font-weight: 400;
      letter-spacing: 0.05em;
      color: var(--color-text-muted);
      padding: var(--space-2) var(--space-4);
      border: 1px solid var(--color-border);
      border-radius: var(--radius-full);
    }
    .about__credential svg { width: 14px; height: 14px; color: var(--color-accent-light); }

    /* ============================================================
       FAQ
       ============================================================ */
    .faq__list { max-width: var(--content-narrow); margin-inline: auto; }
    .faq__item {
      border-bottom: 1px solid var(--color-divider);
    }
    .faq__summary {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: var(--space-4);
      padding: var(--space-5) 0;
      font-family: var(--font-body);
      font-size: var(--text-sm);
      font-weight: 400;
      cursor: pointer;
      list-style: none;
      color: var(--color-text);
    }
    .faq__summary::-webkit-details-marker { display: none; }
    .faq__icon {
      flex-shrink: 0;
      width: 20px; height: 20px;
      color: var(--color-text-faint);
      transition: transform var(--transition);
    }
    details[open] .faq__icon { transform: rotate(45deg); }
    .faq__answer {
      padding-bottom: var(--space-5);
      color: var(--color-text-muted);
      font-size: var(--text-sm);
    }

    /* ============================================================
       CTA FINAL
       ============================================================ */
    .cta-final {
      text-align: center;
      position: relative;
      overflow: hidden;
    }
    .cta-final::before {
      content: '';
      position: absolute;
      top: 50%; left: 50%;
      transform: translate(-50%, -50%);
      width: 500px; height: 500px;
      background: radial-gradient(circle, var(--color-accent-glow), transparent 70%);
      pointer-events: none;
    }
    .cta-final__content { position: relative; z-index: 1; }
    .cta-final h2 {
      font-family: var(--font-display);
      font-size: var(--text-2xl);
      font-weight: 500;
      letter-spacing: -0.02em;
      margin-bottom: var(--space-4);
    }
    .cta-final p {
      color: var(--color-text-muted);
      max-width: 48ch;
      margin-inline: auto;
      margin-bottom: var(--space-8);
    }

    /* ============================================================
       FOOTER
       ============================================================ */
    .footer {
      border-top: 1px solid var(--color-divider);
      padding-block: var(--space-12);
      background: var(--color-surface);
    }
    .footer__inner {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: var(--space-8);
      flex-wrap: wrap;
    }
    .footer__brand {
      font-family: var(--font-display);
      font-size: var(--text-lg);
      font-weight: 600;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      margin-bottom: var(--space-2);
    }
    .footer__info {
      font-size: var(--text-sm);
      color: var(--color-text-muted);
      max-width: 40ch;
    }
    .footer__links {
      display: flex;
      gap: var(--space-6);
      flex-wrap: wrap;
    }
    .footer__links a {
      font-family: var(--font-body);
      font-size: var(--text-xs);
      font-weight: 400;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--color-text-muted);
    }
    .footer__links a:hover { color: var(--color-text); }
    .footer__legal {
      margin-top: var(--space-8);
      padding-top: var(--space-6);
      border-top: 1px solid var(--color-divider);
      font-size: var(--text-xs);
      color: var(--color-text-faint);
      max-width: var(--content-wide);
    }

    /* ============================================================
       MENTION LÉGALE
       ============================================================ */
    .legal-notice {
      background: var(--color-card);
      padding: var(--space-6) var(--space-8);
      border-radius: var(--radius-lg);
      border: 1px solid var(--color-border);
      font-size: var(--text-xs);
      color: var(--color-text-faint);
      max-width: var(--content-narrow);
      margin-inline: auto;
      text-align: center;
    }
    .legal-notice strong { color: var(--color-text-muted); font-weight: 600; }

    /* ============================================================
       FORMULAIRE DE RÉSERVATION
       ============================================================ */
    .booking {
      position: relative;
      overflow: hidden;
    }
    .booking::before {
      content: '';
      position: absolute;
      top: 50%; left: 50%;
      transform: translate(-50%, -50%);
      width: 600px; height: 600px;
      background: radial-gradient(circle, var(--color-accent-glow), transparent 70%);
      pointer-events: none;
    }
    .booking__inner {
      position: relative;
      z-index: 1;
      max-width: 560px;
      margin-inline: auto;
    }
    .booking__header {
      text-align: center;
      margin-bottom: var(--space-10);
    }
    .booking__header h2 {
      font-family: var(--font-display);
      font-size: var(--text-2xl);
      font-weight: 500;
      letter-spacing: -0.02em;
      margin-bottom: var(--space-3);
    }
    .booking__header p {
      color: var(--color-text-muted);
      max-width: 48ch;
      margin-inline: auto;
    }

    .form-card {
      background: var(--color-card);
      border: 1px solid var(--color-border);
      border-radius: var(--radius-lg);
      padding: clamp(var(--space-6), 4vw, var(--space-10));
      box-shadow: var(--shadow-lg);
    }

    .form-row {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: var(--space-4);
    }
    @media (max-width: 540px) {
      .form-row { grid-template-columns: 1fr; }
    }

    .form-group {
      margin-bottom: var(--space-5);
    }
    .form-group label {
      display: block;
      font-family: var(--font-body);
      font-size: var(--text-sm);
      font-weight: 400;
      color: var(--color-text);
      margin-bottom: var(--space-2);
    }
    .form-group label .req { color: var(--color-accent-light); }
    .form-group label .opt { color: var(--color-text-faint); font-weight: 400; font-size: var(--text-xs); }

    .form-input,
    .form-select,
    .form-textarea {
      width: 100%;
      padding: var(--space-3) var(--space-4);
      font-family: var(--font-body);
      font-size: var(--text-sm);
      color: var(--color-text);
      background: var(--color-surface);
      border: 1px solid var(--color-border);
      border-radius: var(--radius-md);
      transition: border-color var(--transition), box-shadow var(--transition);
      -webkit-appearance: none;
      -moz-appearance: none;
      appearance: none;
    }
    .form-input:focus,
    .form-select:focus,
    .form-textarea:focus {
      outline: none;
      border-color: var(--color-accent);
      box-shadow: 0 0 0 3px var(--color-accent-glow);
    }
    .form-input::placeholder,
    .form-textarea::placeholder {
      color: var(--color-text-faint);
    }
    .form-textarea {
      min-height: 100px;
      resize: vertical;
    }
    .form-select {
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 24 24' fill='none' stroke='%236B6964' stroke-width='2'%3E%3Cpolyline points='6 9 12 15 18 9'/%3E%3C/svg%3E");
      background-repeat: no-repeat;
      background-position: right var(--space-4) center;
      padding-right: var(--space-10);
    }
    .form-select:invalid:not(:focus):not(:placeholder-shown) { border-color: var(--color-text-faint); }

    .form-checkbox {
      display: flex;
      align-items: flex-start;
      gap: var(--space-3);
      margin-bottom: var(--space-6);
    }
    .form-checkbox input[type="checkbox"] {
      flex-shrink: 0;
      width: 18px; height: 18px;
      margin-top: 2px;
      accent-color: var(--color-accent);
      cursor: pointer;
    }
    .form-checkbox label {
      font-size: var(--text-xs);
      color: var(--color-text-muted);
      cursor: pointer;
      margin: 0;
      line-height: 1.5;
    }
    .form-checkbox label a { color: var(--color-accent-light); text-decoration: underline; }

    .form-submit {
      width: 100%;
      padding: var(--space-4) var(--space-8);
      font-family: var(--font-body);
      font-size: var(--text-xs);
      font-weight: 600;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      justify-content: center;
    }
    .form-submit:disabled {
      opacity: 0.6;
      cursor: not-allowed;
    }

    .form-error {
      display: none;
      align-items: center;
      gap: var(--space-2);
      padding: var(--space-3) var(--space-4);
      margin-bottom: var(--space-4);
      font-size: var(--text-sm);
      color: #E07090;
      background: color-mix(in oklab, var(--color-accent) 12%, transparent);
      border: 1px solid color-mix(in oklab, var(--color-accent) 30%, transparent);
      border-radius: var(--radius-md);
    }
    .form-error--visible { display: flex; }
    .form-error svg { width: 18px; height: 18px; flex-shrink: 0; }

    .form-success {
      display: none;
      text-align: center;
      padding: var(--space-8) var(--space-6);
    }
    .form-success--visible { display: block; }
    .form-success__icon {
      width: 64px; height: 64px;
      margin: 0 auto var(--space-6);
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      background: color-mix(in oklab, var(--color-accent) 15%, transparent);
      color: var(--color-accent-light);
    }
    .form-success__icon svg { width: 32px; height: 32px; }
    .form-success h3 {
      font-family: var(--font-display);
      font-size: var(--text-xl);
      font-weight: 600;
      margin-bottom: var(--space-3);
    }
    .form-success p {
      color: var(--color-text-muted);
      margin-bottom: var(--space-4);
    }
    .form-success__detail {
      display: inline-flex;
      flex-direction: column;
      gap: var(--space-2);
      padding: var(--space-4) var(--space-6);
      background: var(--color-card);
      border: 1px solid var(--color-border);
      border-radius: var(--radius-md);
      margin-bottom: var(--space-6);
      font-size: var(--text-sm);
      color: var(--color-text-muted);
      text-align: left;
    }
    .form-success__detail strong { color: var(--color-text); }

    .form-loading {
      display: inline-block;
      width: 16px; height: 16px;
      border: 2px solid color-mix(in oklab, #fff 30%, transparent);
      border-top-color: #fff;
      border-radius: 50%;
      animation: spin 0.6s linear infinite;
    }
    @keyframes spin { to { transform: rotate(360deg); } }

    /* ============================================================
       RESPONSIVE
       ============================================================ */
    @media (max-width: 640px) {
      .hero__actions { flex-direction: column; }
      .btn { width: 100%; justify-content: center; }
      .single-session { flex-direction: column; text-align: center; }
    }
  </style>
</head>
<body>

  <!-- ============================================================
       HEADER
       ============================================================ -->
  <header class="header">
    <div class="container header__inner">
      <a href="/" class="logo" aria-label="Karl Kandot — Accueil">
        <svg viewBox="0 0 32 32" fill="none" stroke="currentColor" stroke-width="1.5" aria-hidden="true">
          <circle cx="16" cy="16" r="14" stroke="var(--color-accent)" />
          <path d="M10 16 Q16 8, 22 16 Q16 24, 10 16" stroke="var(--color-accent-light)" fill="none" />
          <circle cx="16" cy="16" r="3" fill="var(--color-accent)" />
        </svg>
        Karl Kandot
      </a>
      <nav class="nav" aria-label="Navigation principale">
        <a href="#offres">Offres</a>
        <a href="#deroule">Déroulé</a>
        <a href="#apropos">À propos</a>
        <a href="#faq">FAQ</a>
        <button class="theme-toggle" data-theme-toggle aria-label="Changer de thème">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="5"/><path d="M12 1v2M12 21v2M4.22 4.22l1.42 1.42M18.36 18.36l1.42 1.42M1 12h2M21 12h2M4.22 19.78l1.42-1.42M18.36 5.64l1.42-1.42"/></svg>
        </button>
      </nav>
      <button class="nav__toggle" aria-label="Menu">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="3" y1="6" x2="21" y2="6"/><line x1="3" y1="12" x2="21" y2="12"/><line x1="3" y1="18" x2="21" y2="18"/></svg>
      </button>
    </div>
  </header>

  <main>

    <!-- ============================================================
         HERO
         ============================================================ -->
    <section class="hero">
      <div class="container">
        <div class="hero__content">
          <span class="hero__label">Hypno-coaching en visio</span>
          <h1>Retrouvez <em>calme</em>, clarté<br />et ressources intérieures</h1>
          <p class="hero__subtitle">
            Une approche unique qui combine l'hypnose éricksonienne et le coaching professionnel.
            En visioconférence, partout en France, pour avancer avec sérénité et confiance.
          </p>
          <div class="hero__actions">
            <a href="#offres" class="btn btn--primary">Découvrir les offres</a>
            <a href="#deroule" class="btn btn--ghost">Comment ça marche</a>
          </div>
          <blockquote class="hero__quote">
            <p>« Laissez votre inconscient découvrir ses propres ressources et vous serez surpris de la profondeur de votre capacité à changer. »</p>
            <cite>— Milton H. Erickson, père de l'hypnose thérapeutique</cite>
          </blockquote>
        </div>
        <div class="hero__visual">
          <img src="https://images.unsplash.com/photo-1752650733337-cb0189176fb9?auto=format&fit=crop&w=900&q=80" alt="Séance d'hypno-coaching en visioconférence" loading="eager" />
        </div>
      </div>
    </section>

    <!-- ============================================================
         POUR QUI
         ============================================================ -->
    <section id="pour-qui">
      <div class="container">
        <p class="section-label">Pour qui ?</p>
        <h2 class="section-title">Ces accompagnements s'adressent à vous si…</h2>
        <p class="section-intro">
          Vous ressentez une pression constante, un besoin de retrouver de l'équilibre, ou vous préparez un moment important. L'hypno-coaching vous aide à mobiliser vos ressources intérieures.
        </p>
        <div class="for-whom__visual">
          <img src="https://images.unsplash.com/photo-1674504502895-3ac04ab2943e?auto=format&fit=crop&w=1400&q=80" alt="Personne sereine en état de relâchement, casque audio" loading="lazy" />
        </div>
        <div class="for-whom__grid">
          <div class="for-whom__card">
            <div class="for-whom__icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 12h-4l-3 9L9 3l-3 9H2"/></svg>
            </div>
            <h3>Stress & pression</h3>
            <p>Vous vivez avec un niveau de tension élevé et cherchez à retrouver du calme au quotidien.</p>
          </div>
          <div class="for-whom__card">
            <div class="for-whom__icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
            </div>
            <h3>Équilibre pro / perso</h3>
            <p>Vous souhaitez réconcilier vos ambitions professionnelles avec votre bien-être personnel.</p>
          </div>
          <div class="for-whom__card">
            <div class="for-whom__icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><circle cx="12" cy="12" r="6"/><circle cx="12" cy="12" r="2"/></svg>
            </div>
            <h3>Préparation mentale</h3>
            <p>Vous abordez un événement important et voulez être au meilleur de vos capacités.</p>
          </div>
          <div class="for-whom__card">
            <div class="for-whom__icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s-8-4.5-8-11.8A5.2 5.2 0 0 1 12 5a5.2 5.2 0 0 1 8 5.2c0 7.3-8 11.8-8 11.8z"/></svg>
            </div>
            <h3>Confiance en soi</h3>
            <p>Vous voulez renforcer votre assurance et votre posture, personnellement et professionnellement.</p>
          </div>
          <div class="for-whom__card">
            <div class="for-whom__icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M3 12a9 9 0 1 0 9-9 9.75 9.75 0 0 0-6.74 2.74L3 8"/><path d="M3 3v5h5"/></svg>
            </div>
            <h3>Changement d'habitudes</h3>
            <p>Vous souhaitez modifier des comportements ou routines qui ne vous servent plus.</p>
          </div>
          <div class="for-whom__card">
            <div class="for-whom__icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 12l2 2 4-4"/><circle cx="12" cy="12" r="10"/></svg>
            </div>
            <h3>Prise de décision</h3>
            <p>Vous faites face à un choix important et cherchez à clarifier vos priorités profondes.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- ============================================================
         CE QUE CE N'EST PAS
         ============================================================ -->
    <section class="not-section">
      <div class="container container-narrow">
        <p class="section-label">Cadre éthique</p>
        <h2 class="section-title">Ce que l'hypno-coaching n'est pas</h2>
        <div class="not-section__box">
          <p>
            <strong>L'hypno-coaching est un accompagnement de bien-être et de développement personnel.</strong>
            Il ne remplace pas un suivi médical, psychologique ou psychiatrique. Il ne constitue ni un diagnostic,
            ni un traitement médical, ni une psychothérapie. Les praticiens en hypnose ne sont pas des professionnels
            de santé et n'interviennent pas dans le cadre de pathologies reconnues. Si vous suivez un traitement
            médical ou un suivi psychologique, poursuivez-le et informez votre professionnel de santé de votre
            démarche.
          </p>
        </div>
      </div>
    </section>

    <!-- ============================================================
         OFFRES / PACKS
         ============================================================ -->
    <section id="offres">
      <div class="container">
        <p class="section-label">Offres hypno-coaching</p>
        <h2 class="section-title">Des programmes structurés, adaptés à vos besoins</h2>
        <p class="section-intro">
          Chaque pack combine des séances d'hypnose éricksonienne et de coaching personnalisé en visioconférence.
          Tarifs de lancement pour les 90 premiers jours.
        </p>

        <div class="packs__grid">

          <!-- Pack 1 : Calme & équilibre -->
          <article class="pack">
            <div class="pack__name">Calme & équilibre</div>
            <p class="pack__tagline">Stress, pression, équilibre pro / perso</p>
            <div class="pack__price">225 €</div>
            <div class="pack__price-detail">3 séances · 75 € / séance · 1h par séance</div>
            <ul class="pack__features">
              <li>Identification des sources de tension</li>
              <li>Apprentissage de l'auto-hypnose</li>
              <li>Techniques de régulation émotionnelle</li>
              <li>Plan d'intégration au quotidien</li>
              <li>Exercices personnalisés entre séances</li>
            </ul>
            <a href="#contact" class="btn btn--ghost pack__btn">Choisir ce pack</a>
          </article>

          <!-- Pack 2 : Confiance & ressources -->
          <article class="pack">
            <div class="pack__name">Confiance & ressources</div>
            <p class="pack__tagline">Confiance, posture, prise de décision</p>
            <div class="pack__price">280 €</div>
            <div class="pack__price-detail">4 séances · 70 € / séance · 1h par séance</div>
            <ul class="pack__features">
              <li>Exploration des ressources intérieures</li>
              <li>Renforcement de la posture et de l'ancrage</li>
              <li>Travail sur les croyances limitantes</li>
              <li>Mise en situation guidée en état modifié</li>
              <li>Stratégies de dépassement de soi</li>
            </ul>
            <a href="#contact" class="btn btn--ghost pack__btn">Choisir ce pack</a>
          </article>

          <!-- Pack 3 : Préparation mentale -->
          <article class="pack pack--featured">
            <span class="pack__badge">Le plus demandé</span>
            <div class="pack__name">Préparation mentale</div>
            <p class="pack__tagline">Performance, pression, objectif important</p>
            <div class="pack__price">300 €</div>
            <div class="pack__price-detail">4 séances · 75 € / séance · 1h par séance</div>
            <ul class="pack__features">
              <li>Définition de l'objectif et de la stratégie</li>
              <li>Visualisation et répétition mentale</li>
              <li>Gestion de la pression et du trac</li>
              <li>Ancrage de l'état de performance</li>
              <li>Séance de renforcement pré-événement</li>
            </ul>
            <a href="#contact" class="btn btn--primary pack__btn">Choisir ce pack</a>
          </article>

          <!-- Pack 4 : Changement d'habitudes -->
          <article class="pack">
            <div class="pack__name">Changement d'habitudes</div>
            <p class="pack__tagline">Comportements, routines, impulsions</p>
            <div class="pack__price">350 €</div>
            <div class="pack__price-detail">5 séances · 70 € / séance · 1h par séance</div>
            <ul class="pack__features">
              <li>Cartographie du comportement à modifier</li>
              <li>Travail sur les déclencheurs et les contextes</li>
              <li>Installation de nouvelles routines</li>
              <li>Séances de renforcement sur 3 semaines</li>
              <li>Stratégies de prévention des rechutes</li>
            </ul>
            <a href="#contact" class="btn btn--ghost pack__btn">Choisir ce pack</a>
          </article>

        </div>

        <!-- Séance unitaire -->
        <div class="single-session">
          <div class="single-session__info">
            <h3>Séance à l'unité</h3>
            <p>Pour découvrir l'approche ou traiter un sujet ponctuel. 1h en visio.</p>
          </div>
          <div class="single-session__price">80 €</div>
          <a href="#contact" class="btn btn--ghost">Réserver une séance</a>
        </div>

        <p class="packs__note">
          Appel découverte gratuit de 30 min · Paiement en ligne sécurisé · Facilités de paiement possibles
        </p>
      </div>
    </section>

    <!-- ============================================================
         DÉROULÉ
         ============================================================ -->
    <section id="deroule">
      <div class="container">
        <p class="section-label">Comment ça marche</p>
        <h2 class="section-title">Un parcours simple et structuré</h2>
        <p class="section-intro">
          De la première prise de contact à l'intégration durable des changements, chaque étape est pensée pour vous accompagner efficacement.
        </p>
        <div class="process__steps">
          <div class="process__step">
            <h3>Appel découverte</h3>
            <p>30 minutes gratuites en visio. Vous présentez votre situation, je vous propose le parcours adapté. Aucun engagement.</p>
          </div>
          <div class="process__step">
            <h3>Première séance</h3>
            <p>1h en visioconférence. Nous explorons votre objectif et démarrons le travail hypnotique et coaching.</p>
          </div>
          <div class="process__step">
            <h3>Séances de suivi</h3>
            <p>Approfondissement et intégration. Des exercices personnalisés entre les séances pour ancrer les changements.</p>
          </div>
          <div class="process__step">
            <h3>Intégration</h3>
            <p>Bilan de parcours, stratégies d'autonomie et outils d'auto-hypnose pour continuer votre progression en solo.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- ============================================================
         À PROPOS
         ============================================================ -->
    <section id="apropos" class="about">
      <div class="container">
        <div class="about__grid">
          <div class="about__visual">
            <svg viewBox="0 0 200 200" fill="none" stroke="currentColor" aria-hidden="true" style="color: var(--color-accent)">
              <circle cx="100" cy="100" r="90" stroke-width="1" opacity="0.2"/>
              <circle cx="100" cy="100" r="70" stroke-width="1" opacity="0.3"/>
              <circle cx="100" cy="100" r="50" stroke-width="1" opacity="0.4"/>
              <circle cx="100" cy="100" r="30" stroke-width="1" opacity="0.6"/>
              <path d="M50 100 Q100 50, 150 100 Q100 150, 50 100" stroke-width="1.5" opacity="0.8"/>
              <circle cx="100" cy="100" r="8" fill="currentColor" opacity="0.9"/>
            </svg>
          </div>
          <div class="about__text">
            <p class="section-label">À propos</p>
            <h2>Karl Kandot</h2>
            <p>
              Formateur en soft skills et coach professionnel, j'accompagne les individus et les équipes
              depuis plusieurs années dans le développement de leurs compétences relationnelles et de leur performance.
            </p>
            <p>
              Praticien certifié en hypnose éricksonienne, j'ai développé l'hypno-coaching pour offrir une approche
              qui combine la profondeur de l'hypnose avec la structuration du coaching. Cette synergie permet
              d'accéder aux ressources inconscientes tout en restant orienté vers l'action et les résultats concrets.
            </p>
            <div class="about__credentials">
              <span class="about__credential">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                Praticien certifié en hypnose éricksonienne
              </span>
              <span class="about__credential">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                Coach professionnel & formateur
              </span>
              <span class="about__credential">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                Séances en visio partout en France
              </span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- ============================================================
         FAQ
         ============================================================ -->
    <section id="faq">
      <div class="container">
        <p class="section-label">Questions fréquentes</p>
        <h2 class="section-title">Vous vous demandez peut-être…</h2>
        <div class="faq__list">
          <details class="faq__item">
            <summary class="faq__summary">
              L'hypnose en visio est-elle aussi efficace qu'en cabinet ?
              <svg class="faq__icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
            </summary>
            <div class="faq__answer">
              Oui. De nombreuses études et retours d'expérience confirment l'efficacité de l'hypnose en visioconférence.
              Le cadre de votre choix (chez vous, dans un espace calme) favorise même parfois un lâcher-prise plus rapide.
              La séance se déroule exactement comme en cabinet, via une plateforme sécurisée avec lien privé.
            </div>
          </details>
          <details class="faq__item">
            <summary class="faq__summary">
              Vais-je perdre le contrôle ou m'endormir ?
              <svg class="faq__icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
            </summary>
            <div class="faq__answer">
              Non. L'hypnose éricksonienne est un état de conscience modifiée où vous restez pleinement conscient et maître
              de vos choix. Vous entendez tout, vous gardez le contrôle, et vous sortez de l'état hypnotique en pleine clarté.
              C'est un état naturel que nous expérimentons tous spontanément (ex: conduit sur un itinéraire connu sans y penser).
            </div>
          </details>
          <details class="faq__item">
            <summary class="faq__summary">
              Combien de séances faut-il prévoir ?
              <svg class="faq__icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
            </summary>
            <div class="faq__answer">
              Cela dépend de votre objectif. Pour un sujet ponctuel, 1 à 2 séances peuvent suffire. Pour un travail
              plus approfondi (gestion du stress, préparation mentale, changement d'habitudes), les packs de 3 à 5 séances
              offrent un accompagnement structuré et durable. L'appel découverte gratuit permet d'évaluer ensemble le parcours adapté.
            </div>
          </details>
          <details class="faq__item">
            <summary class="faq__summary">
              L'hypno-coaching est-il remboursé ?
              <svg class="faq__icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
            </summary>
            <div class="faq__answer">
              L'hypno-coaching n'est pas pris en charge par la Sécurité Sociale. Cependant, certaines mutuelles
              proposent un forfait de remboursement partiel pour les séances d'hypnose (forfait bien-être ou médecines douces).
              Renseignez-vous auprès de votre mutuelle pour connaître vos droits.
            </div>
          </details>
          <details class="faq__item">
            <summary class="faq__summary">
              Les séances sont-elles confidentielles ?
              <svg class="faq__icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
            </summary>
            <div class="faq__answer">
              Absolument. Le secret professionnel s'applique à toutes les séances. Aucune séance n'est enregistrée.
              La plateforme de visioconférence utilise un lien privé. Vos données personnelles sont traitées conformément
              au RGPD. Consultez nos CGV pour plus de détails.
            </div>
          </details>
        </div>
      </div>
    </section>

    <!-- ============================================================
         FORMULAIRE DE RÉSERVATION
         ============================================================ -->
    <section class="booking" id="contact">
      <div class="container">
        <div class="booking__inner">
          <div class="booking__header">
            <p class="section-label">Appel découverte gratuit</p>
            <h2>Réservez vos 30 minutes</h2>
            <p>Présentez votre situation, recevez une recommandation de parcours adapté. Aucun engagement, aucune obligation.</p>
          </div>

          <div class="form-card" id="formCard">
            <div class="form-error" id="formError">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/></svg>
              <span id="formErrorText">Une erreur est survenue. Veuillez réessayer ou me contacter directement par email.</span>
            </div>

            <form id="bookingForm" novalidate>
              <div class="form-row">
                <div class="form-group">
                  <label for="firstName">Prénom <span class="req">*</span></label>
                  <input type="text" id="firstName" name="firstName" class="form-input" placeholder="Votre prénom" required />
                </div>
                <div class="form-group">
                  <label for="lastName">Nom <span class="req">*</span></label>
                  <input type="text" id="lastName" name="lastName" class="form-input" placeholder="Votre nom" required />
                </div>
              </div>

              <div class="form-row">
                <div class="form-group">
                  <label for="email">Email <span class="req">*</span></label>
                  <input type="email" id="email" name="email" class="form-input" placeholder="vous@exemple.fr" required />
                </div>
                <div class="form-group">
                  <label for="phone">Téléphone <span class="opt">(optionnel)</span></label>
                  <input type="tel" id="phone" name="phone" class="form-input" placeholder="06 12 34 56 78" />
                </div>
              </div>

              <div class="form-group">
                <label for="pack">Parcours souhaité <span class="req">*</span></label>
                <select id="pack" name="pack" class="form-select" required>
                  <option value="" disabled selected>Choisissez un parcours…</option>
                  <option value="appel-decouverte">Appel découverte (gratuit, 30 min)</option>
                  <option value="calme-equilibre">Pack Calme & équilibre (3 séances)</option>
                  <option value="confiance-ressources">Pack Confiance & ressources (4 séances)</option>
                  <option value="preparation-mentale">Pack Préparation mentale (4 séances)</option>
                  <option value="changement-habitudes">Pack Changement d'habitudes (5 séances)</option>
                  <option value="seance-unite">Séance à l'unité (1h)</option>
                  <option value="indecis">Je ne sais pas encore</option>
                </select>
              </div>

              <div class="form-row">
                <div class="form-group">
                  <label for="day">Jour préféré <span class="req">*</span></label>
                  <select id="day" name="day" class="form-select" required>
                    <option value="" disabled selected>Choisissez…</option>
                    <option value="lundi">Lundi</option>
                    <option value="mardi">Mardi</option>
                    <option value="mercredi">Mercredi</option>
                    <option value="jeudi">Jeudi</option>
                    <option value="vendredi">Vendredi</option>
                    <option value="samedi">Samedi</option>
                    <option value="flexible">Je suis flexible</option>
                  </select>
                </div>
                <div class="form-group">
                  <label for="time">Créneau préféré <span class="req">*</span></label>
                  <select id="time" name="time" class="form-select" required>
                    <option value="" disabled selected>Choisissez…</option>
                    <option value="matin">Matin (9h - 12h)</option>
                    <option value="dejeuner">Pause déjeuner (12h - 14h)</option>
                    <option value="apres-midi">Après-midi (14h - 17h)</option>
                    <option value="soir">En soirée (17h - 20h)</option>
                    <option value="flexible">Je suis flexible</option>
                  </select>
                </div>
              </div>

              <div class="form-group">
                <label for="message">Votre situation <span class="opt">(optionnel)</span></label>
                <textarea id="message" name="message" class="form-textarea" placeholder="Quelques mots sur ce qui vous amène…"></textarea>
              </div>

              <div class="form-checkbox">
                <input type="checkbox" id="consent" name="consent" required />
                <label for="consent">
                  J'accepte que mes données personnelles soient utilisées uniquement pour traiter ma demande de réservation, conformément au RGPD. Voir les <a href="cgv.html">CGV</a> pour plus d'informations.
                </label>
              </div>

              <button type="submit" class="btn btn--primary form-submit" id="submitBtn">
                Envoyer ma demande
              </button>
            </form>
          </div>

          <div class="form-card form-success" id="formSuccess">
            <div class="form-success__icon">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
            </div>
            <h3>Demande envoyée !</h3>
            <p>Merci. Je vous réponds sous 24 à 48h pour confirmer votre créneau.</p>
            <div class="form-success__detail" id="successDetail"></div>
            <a href="#offres" class="btn btn--ghost">Retour aux offres</a>
          </div>

        </div>
      </div>
    </section>

    <!-- ============================================================
         MENTION LÉGALE
         ============================================================ -->
    <section style="padding-block: var(--space-8);">
      <div class="container">
        <div class="legal-notice">
          <strong>Mention importante :</strong> L'hypno-coaching est un accompagnement de bien-être et de développement personnel.
          Il ne remplace pas un suivi médical, psychologique ou psychiatrique. Les praticiens en hypnose ne sont pas des
          professionnels de santé. En cas de pathologie, consultez un professionnel de santé qualifié.
        </div>
      </div>
    </section>

  </main>

  <!-- ============================================================
       FOOTER
       ============================================================ -->
  <footer class="footer">
    <div class="container">
      <div class="footer__inner">
        <div>
          <div class="footer__brand">Karl Kandot</div>
          <p class="footer__info">
            Formateur en soft skills & Coach professionnel<br>
            Praticien certifié en hypnose éricksonienne<br>
            Séances en visio partout en France
          </p>
        </div>
        <div class="footer__links">
          <a href="#offres">Offres</a>
          <a href="#deroule">Déroulé</a>
          <a href="#apropos">À propos</a>
          <a href="#faq">FAQ</a>
          <a href="cgv.html">CGV</a>
          <a href="mailto:karlkandot@gmail.com">Contact</a>
        </div>
      </div>
      <div class="footer__legal">
        © 2026 Karl Kandot — Tous droits réservés. Praticien certifié en hypnose éricksonienne.
        L'hypno-coaching est un accompagnement de bien-être et ne constitue pas un acte médical.
        Voir les <a href="cgv.html">conditions générales de vente</a>.
      </div>
    </div>
  </footer>

  <!-- ============================================================
       SCRIPTS
       ============================================================ -->
  <script>
    // Theme toggle — fonctionnel avec mémorisation du choix (localStorage)
    (function() {
      var t = document.querySelector('[data-theme-toggle]');
      var r = document.documentElement;

      function iconFor(theme) {
        return theme === 'dark'
          ? '<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="5"/><path d="M12 1v2M12 21v2M4.22 4.22l1.42 1.42M18.36 18.36l1.42 1.42M1 12h2M21 12h2M4.22 19.78l1.42-1.42M18.36 5.64l1.42-1.42"/></svg>'
          : '<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"/></svg>';
      }

      function applyTheme(theme) {
        r.setAttribute('data-theme', theme);
        if (t) {
          t.innerHTML = iconFor(theme);
          t.setAttribute('aria-label', 'Basculer vers le mode ' + (theme === 'dark' ? 'clair' : 'sombre'));
        }
      }

      // Ordre de priorité : choix mémorisé > préférence système > clair par défaut
      var stored = null;
      try { stored = localStorage.getItem('theme'); } catch (e) {}
      var d = stored || (matchMedia('(prefers-color-scheme:dark)').matches ? 'dark' : 'light');
      applyTheme(d);

      if (t) {
        t.addEventListener('click', function() {
          d = d === 'dark' ? 'light' : 'dark';
          applyTheme(d);
          try { localStorage.setItem('theme', d); } catch (e) {}
        });
      }
    })();

    // Mobile menu toggle
    (function() {
      var toggle = document.querySelector('.nav__toggle');
      var nav = document.querySelector('.nav');
      if (toggle && nav) {
        toggle.addEventListener('click', function() {
          if (nav.style.display === 'flex') {
            nav.style.display = '';
          } else {
            nav.style.display = 'flex';
            nav.style.position = 'absolute';
            nav.style.top = '100%';
            nav.style.left = '0';
            nav.style.right = '0';
            nav.style.flexDirection = 'column';
            nav.style.background = 'var(--color-bg)';
            nav.style.padding = 'var(--space-4) var(--space-6)';
            nav.style.borderBottom = '1px solid var(--color-divider)';
          }
        });
      }
    })();
    // Booking form submission via FormSubmit.co (free, no signup)
    (function() {
      var form = document.getElementById('bookingForm');
      if (!form) return;

      var formCard = document.getElementById('formCard');
      var formSuccess = document.getElementById('formSuccess');
      var formError = document.getElementById('formError');
      var formErrorText = document.getElementById('formErrorText');
      var submitBtn = document.getElementById('submitBtn');
      var successDetail = document.getElementById('successDetail');

      var packLabels = {
        'appel-decouverte': 'Appel découverte (gratuit, 30 min)',
        'calme-equilibre': 'Pack Calme & équilibre (3 séances)',
        'confiance-ressources': 'Pack Confiance & ressources (4 séances)',
        'preparation-mentale': 'Pack Préparation mentale (4 séances)',
        'changement-habitudes': 'Pack Changement d\'habitudes (5 séances)',
        'seance-unite': 'Séance à l\'unité (1h)',
        'indecis': 'Je ne sais pas encore'
      };
      var dayLabels = {
        'lundi': 'Lundi', 'mardi': 'Mardi', 'mercredi': 'Mercredi',
        'jeudi': 'Jeudi', 'vendredi': 'Vendredi', 'samedi': 'Samedi',
        'flexible': 'Flexible'
      };
      var timeLabels = {
        'matin': 'Matin (9h - 12h)', 'dejeuner': 'Pause déjeuner (12h - 14h)',
        'apres-midi': 'Après-midi (14h - 17h)', 'soir': 'En soirée (17h - 20h)',
        'flexible': 'Flexible'
      };

      function showError(msg) {
        formErrorText.textContent = msg || 'Une erreur est survenue. Veuillez réessayer ou me contacter directement par email.';
        formError.classList.add('form-error--visible');
      }

      function hideError() {
        formError.classList.remove('form-error--visible');
      }

      form.addEventListener('submit', function(e) {
        e.preventDefault();
        hideError();

        // Basic validation
        var required = form.querySelectorAll('[required]');
        var valid = true;
        required.forEach(function(field) {
          if (!field.value || (field.type === 'checkbox' && !field.checked)) {
            field.style.borderColor = 'var(--color-accent)';
            valid = false;
          } else {
            field.style.borderColor = '';
          }
        });

        // Email validation
        var emailField = document.getElementById('email');
        var emailRe = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        if (emailField.value && !emailRe.test(emailField.value)) {
          emailField.style.borderColor = 'var(--color-accent)';
          showError('Veuillez saisir une adresse email valide.');
          return;
        }

        if (!valid) {
          showError('Veuillez remplir tous les champs obligatoires (marqués d\'un *).');
          return;
        }

        // Build payload
        var data = {
          firstName: document.getElementById('firstName').value.trim(),
          lastName: document.getElementById('lastName').value.trim(),
          email: emailField.value.trim(),
          phone: document.getElementById('phone').value.trim(),
          pack: document.getElementById('pack').value,
          day: document.getElementById('day').value,
          time: document.getElementById('time').value,
          message: document.getElementById('message').value.trim(),
          _subject: 'Nouvelle demande de réservation — Hypno-coaching',
          _template: 'table'
        };

        // Show loading
        submitBtn.disabled = true;
        submitBtn.innerHTML = '<span class="form-loading"></span> Envoi en cours…';

        // Capture form values for success display
        var formData = {
          firstName: data.firstName,
          lastName: data.lastName,
          email: data.email,
          phone: data.phone,
          pack: data.pack,
          day: data.day,
          time: data.time
        };

        // Submit to FormSubmit.co
        fetch('https://formsubmit.co/ajax/karlkandot@gmail.com', {
          method: 'POST',
          headers: {
            'Content-Type': 'application/json',
            'Accept': 'application/json'
          },
          body: JSON.stringify(data)
        })
        .then(function(res) { return res.json(); })
        .then(function(response) {
          if (response.success === 'true' || response.success === true) {
            // Show success
            formCard.style.display = 'none';
            formSuccess.classList.add('form-success--visible');

            // Build detail summary
            var html = '';
            html += '<strong>Nom :</strong> ' + formData.firstName + ' ' + formData.lastName;
            html += '<br><strong>Parcours :</strong> ' + (packLabels[formData.pack] || formData.pack || '');
            html += '<br><strong>Créneau :</strong> ' + (dayLabels[formData.day] || formData.day || '') + ' — ' + (timeLabels[formData.time] || formData.time || '');
            html += '<br><strong>Email :</strong> ' + formData.email;
            if (formData.phone) html += '<br><strong>Téléphone :</strong> ' + formData.phone;
            successDetail.innerHTML = html;
          } else {
            throw new Error(response.message || 'Échec de l\'envoi');
          }
        })
        .catch(function(err) {
          submitBtn.disabled = false;
          submitBtn.innerHTML = 'Envoyer ma demande';
          showError('L\'envoi a échoué. Vous pouvez aussi me contacter directement à karlkandot@gmail.com.');
        });
      });

      // Clear error border on input
      form.querySelectorAll('input, select, textarea').forEach(function(field) {
        field.addEventListener('input', function() {
          field.style.borderColor = '';
          hideError();
        });
      });
    })();

  </script>

</body>
</html>
