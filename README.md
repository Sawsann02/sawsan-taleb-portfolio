<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sawsan Alhaddad | Information Systems Graduate & Digital Creator</title>
    <meta name="description" content="Personal portfolio of Sawsan Alhaddad, an Information Systems graduate specializing in web development, UI/UX design, digital creativity, and technology.">
    <meta name="keywords" content="Sawsan Alhaddad, Information Systems, Web Developer, UI/UX Designer, Digital Creator, Portfolio">
    <meta name="author" content="Sawsan Alhaddad">
    <meta property="og:title" content="Sawsan Alhaddad | Information Systems Graduate & Digital Creator">
    <meta property="og:description" content="Personal portfolio of Sawsan Alhaddad, an Information Systems graduate specializing in web development, UI/UX design, digital creativity, and technology.">
    <meta property="og:type" content="website">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        /* ===== CSS RESET & VARIABLES ===== */
        *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }
        
       :root {

    /* ===== Backgrounds ===== */
    --bg-primary: #F8F9FA;
    --bg-secondary: #F1F3F5;
    --bg-card: #FFFFFF;

    /* ===== Dark Sections ===== */
    --bg-dark: #172033;
    --bg-dark-secondary: #202B3F;

    /* ===== Text ===== */
    --text-primary: #1F2937;
    --text-secondary: #5F6B7A;
    --text-light: #8A94A3;
    --text-white: #FFFFFF;

    /* ===== Main Accent - Professional Blue ===== */
    --accent: #4F6F92;
    --accent-light: #6F8EAE;
    --accent-soft: #E8EEF5;

    /* ===== Elegant Secondary Colors ===== */
    --accent-rose: #B9A6A2;
    --accent-teal: #6F8F8B;

    /* ===== Small Gold Accent ===== */
    --accent-gold: #B79B68;
    --accent-gold-soft: #F3EEE5;

    /* ===== Borders ===== */
    --border: #DDE2E8;
    --border-light: #EDF0F3;

    /* ===== Shadows ===== */
    --shadow-sm:
        0 2px 8px rgba(23, 32, 51, 0.04);

    --shadow-md:
        0 4px 20px rgba(23, 32, 51, 0.06);

    --shadow-lg:
        0 8px 40px rgba(23, 32, 51, 0.08);

    --shadow-xl:
        0 16px 60px rgba(23, 32, 51, 0.10);

    /* ===== Border Radius ===== */
    --radius-sm: 8px;
    --radius-md: 14px;
    --radius-lg: 20px;
    --radius-xl: 28px;

    /* ===== Animation ===== */
    --transition:
        0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);

    --transition-slow:
        0.6s cubic-bezier(0.25, 0.46, 0.45, 0.94);
}

        html {
            scroll-behavior: smooth;
            scroll-padding-top: 80px;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
            background: var(--bg-primary);
            color: var(--text-primary);
            line-height: 1.7;
            overflow-x: hidden;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }

        /* ===== TYPOGRAPHY ===== */
        h1, h2, h3, h4 {
            font-family: 'Playfair Display', Georgia, serif;
            font-weight: 600;
            line-height: 1.25;
            color: var(--text-primary);
        }

        .section-label {
            font-family: 'Inter', sans-serif;
            font-size: 0.75rem;
            font-weight: 600;
            letter-spacing: 0.2em;
            text-transform: uppercase;
            color: var(--accent);
            margin-bottom: 12px;
            display: inline-block;
        }

        .section-title {
            font-size: clamp(2rem, 4vw, 3rem);
            margin-bottom: 16px;
        }

        .section-subtitle {
            font-family: 'Inter', sans-serif;
            font-size: 1.05rem;
            color: var(--text-secondary);
            max-width: 560px;
            line-height: 1.7;
            font-weight: 300;
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-header .section-subtitle {
            margin: 0 auto;
        }

        /* ===== LAYOUT ===== */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 24px;
        }

        section {
            padding: 100px 0;
        }

        /* ===== NAVIGATION ===== */
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            background: rgba(250, 250, 248, 0.85);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(232, 230, 225, 0.5);
            transition: var(--transition);
        }

        .navbar.scrolled {
            background: rgba(250, 250, 248, 0.95);
            box-shadow: var(--shadow-sm);
        }

        .nav-inner {
            display: flex;
            align-items: center;
            justify-content: space-between;
            height: 72px;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 24px;
        }

        .nav-logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.35rem;
            font-weight: 600;
            color: var(--text-primary);
            text-decoration: none;
            letter-spacing: -0.01em;
        }

        .nav-logo span {
            color: var(--accent);
        }

        .nav-links {
            display: flex;
            align-items: center;
            gap: 8px;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--text-secondary);
            font-size: 0.875rem;
            font-weight: 500;
            padding: 8px 16px;
            border-radius: var(--radius-sm);
            transition: var(--transition);
            position: relative;
        }

        .nav-links a:hover,
        .nav-links a.active {
            color: var(--accent);
            background: var(--accent-soft);
        }

        .nav-cta {
            background: var(--accent);
            color: white !important;
            padding: 10px 24px !important;
            border-radius: 50px !important;
            font-weight: 600 !important;
            font-size: 0.85rem !important;
            letter-spacing: 0.02em;
            transition: var(--transition) !important;
        }

        .nav-cta:hover {
            background: var(--accent-light) !important;
            color: white !important;
            transform: translateY(-1px);
            box-shadow: 0 4px 16px rgba(184, 134, 11, 0.3);
        }

        .hamburger {
            display: none;
            flex-direction: column;
            cursor: pointer;
            gap: 5px;
            padding: 8px;
            z-index: 1001;
        }

        .hamburger span {
            display: block;
            width: 24px;
            height: 2px;
            background: var(--text-primary);
            border-radius: 2px;
            transition: var(--transition);
        }

        .hamburger.active span:nth-child(1) {
            transform: rotate(45deg) translate(5px, 5px);
        }
        .hamburger.active span:nth-child(2) {
            opacity: 0;
        }
        .hamburger.active span:nth-child(3) {
            transform: rotate(-45deg) translate(5px, -5px);
        }

        .mobile-menu {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(250, 250, 248, 0.98);
            backdrop-filter: blur(30px);
            z-index: 999;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 8px;
            opacity: 0;
            pointer-events: none;
            transition: var(--transition-slow);
        }

        .mobile-menu.active {
            opacity: 1;
            pointer-events: all;
        }

        .mobile-menu a {
            text-decoration: none;
            color: var(--text-primary);
            font-size: 1.25rem;
            font-weight: 500;
            padding: 12px 32px;
            border-radius: var(--radius-sm);
            transition: var(--transition);
            transform: translateY(20px);
            opacity: 0;
        }

        .mobile-menu.active a {
            transform: translateY(0);
            opacity: 1;
        }

        .mobile-menu a:nth-child(1) { transition-delay: 0.05s; }
        .mobile-menu a:nth-child(2) { transition-delay: 0.1s; }
        .mobile-menu a:nth-child(3) { transition-delay: 0.15s; }
        .mobile-menu a:nth-child(4) { transition-delay: 0.2s; }
        .mobile-menu a:nth-child(5) { transition-delay: 0.25s; }
        .mobile-menu a:nth-child(6) { transition-delay: 0.3s; }
        .mobile-menu a:nth-child(7) { transition-delay: 0.35s; }
        .mobile-menu a:nth-child(8) { transition-delay: 0.4s; }

        .mobile-menu a:hover {
            color: var(--accent);
            background: var(--accent-soft);
        }

        /* ===== HERO SECTION ===== */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding-top: 72px;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -200px;
            right: -200px;
            width: 600px;
            height: 600px;
            background: radial-gradient(circle, rgba(184,134,11,0.06) 0%, transparent 70%);
            border-radius: 50%;
            pointer-events: none;
        }

        .hero::after {
            content: '';
            position: absolute;
            bottom: -100px;
            left: -100px;
            width: 400px;
            height: 400px;
            background: radial-gradient(circle, rgba(123,167,167,0.05) 0%, transparent 70%);
            border-radius: 50%;
            pointer-events: none;
        }

        .hero-inner {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
            width: 100%;
        }

        .hero-content {
            position: relative;
            z-index: 2;
        }

        .hero-greeting {
            font-family: 'Inter', sans-serif;
            font-size: 0.85rem;
            font-weight: 600;
            letter-spacing: 0.15em;
            text-transform: uppercase;
            color: var(--accent);
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .hero-greeting::before {
            content: '';
            display: inline-block;
            width: 30px;
            height: 1.5px;
            background: var(--accent);
        }

        .hero-name {
            font-family: 'Playfair Display', serif;
            font-size: clamp(2.5rem, 5.5vw, 4.2rem);
            font-weight: 700;
            line-height: 1.1;
            margin-bottom: 12px;
            color: var(--text-primary);
        }

        .hero-name .accent {
            color: var(--accent);
            font-style: italic;
        }

        .hero-title {
            font-family: 'Inter', sans-serif;
            font-size: clamp(0.9rem, 1.5vw, 1.05rem);
            font-weight: 400;
            color: var(--text-secondary);
            margin-bottom: 10px;
            letter-spacing: 0.04em;
        }

        .hero-subtitle {
            font-family: 'Inter', sans-serif;
            font-size: clamp(0.85rem, 1.2vw, 0.95rem);
            color: var(--text-light);
            margin-bottom: 28px;
            letter-spacing: 0.08em;
        }

        .hero-description {
            font-size: 1.05rem;
            line-height: 1.8;
            color: var(--text-secondary);
            margin-bottom: 36px;
            max-width: 480px;
            font-weight: 300;
        }

        .hero-buttons {
            display: flex;
            gap: 16px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 14px 32px;
            border-radius: 50px;
            font-family: 'Inter', sans-serif;
            font-size: 0.9rem;
            font-weight: 600;
            text-decoration: none;
            cursor: pointer;
            border: none;
            transition: var(--transition);
            letter-spacing: 0.02em;
        }

        .btn-primary {
            background: var(--accent);
            color: white;
            box-shadow: 0 4px 16px rgba(184, 134, 11, 0.2);
        }

        .btn-primary:hover {
            background: var(--accent-light);
            transform: translateY(-2px);
            box-shadow: 0 6px 24px rgba(184, 134, 11, 0.3);
        }

        .btn-secondary {
            background: transparent;
            color: var(--text-primary);
            border: 1.5px solid var(--border);
        }

        .btn-secondary:hover {
            border-color: var(--accent);
            color: var(--accent);
            background: var(--accent-soft);
            transform: translateY(-2px);
        }

        .btn-small {
            padding: 10px 22px;
            font-size: 0.82rem;
        }

        /* Hero Visual */
        .hero-visual {
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            z-index: 1;
        }

        .hero-visual-container {
            position: relative;
            width: 100%;
            max-width: 480px;
            aspect-ratio: 1;
        }

        .hero-avatar-ring {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 320px;
            height: 320px;
            border-radius: 50%;
            border: 1.5px solid rgba(184,134,11,0.2);
            animation: pulse-ring 4s ease-in-out infinite;
        }

        .hero-avatar-ring::after {
            content: '';
            position: absolute;
            top: -12px; left: -12px; right: -12px; bottom: -12px;
            border-radius: 50%;
            border: 1px dashed rgba(184,134,11,0.1);
            animation: spin-slow 30s linear infinite;
        }

        @keyframes pulse-ring {
            0%, 100% { transform: translate(-50%, -50%) scale(1); opacity: 1; }
            50% { transform: translate(-50%, -50%) scale(1.03); opacity: 0.7; }
        }

        @keyframes spin-slow {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .hero-avatar {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 240px;
            height: 240px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--accent-soft) 0%, var(--bg-secondary) 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: var(--shadow-lg);
            overflow: hidden;
        }

        .hero-avatar-placeholder {
            font-family: 'Playfair Display', serif;
            font-size: 4.5rem;
            font-weight: 700;
            color: var(--accent);
            opacity: 0.7;
            line-height: 1;
        }

        /* Floating UI Cards around avatar */
        .floating-card {
            position: absolute;
            background: var(--bg-card);
            border-radius: var(--radius-md);
            padding: 12px 18px;
            box-shadow: var(--shadow-md);
            display: flex;
            align-items: center;
            gap: 10px;
            font-family: 'Inter', sans-serif;
            font-size: 0.78rem;
            font-weight: 500;
            color: var(--text-primary);
            border: 1px solid rgba(232,230,225,0.5);
            animation: float 6s ease-in-out infinite;
            white-space: nowrap;
        }

        .floating-card .card-icon {
            width: 32px;
            height: 32px;
            border-radius: var(--radius-sm);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.85rem;
        }

        .fc-1 { top: 8%; right: -5%; animation-delay: 0s; }
        .fc-1 .card-icon { background: rgba(184,134,11,0.12); color: var(--accent); }

        .fc-2 { top: 35%; right: -12%; animation-delay: 1s; }
        .fc-2 .card-icon { background: rgba(123,167,167,0.12); color: var(--accent-teal); }

        .fc-3 { bottom: 18%; right: -2%; animation-delay: 2s; }
        .fc-3 .card-icon { background: rgba(201,168,154,0.15); color: var(--accent-rose); }

        .fc-4 { top: 12%; left: -8%; animation-delay: 0.5s; }
        .fc-4 .card-icon { background: rgba(184,134,11,0.1); color: var(--accent); }

        .fc-5 { bottom: 10%; left: -6%; animation-delay: 1.5s; }
        .fc-5 .card-icon { background: rgba(123,167,167,0.1); color: var(--accent-teal); }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        /* ===== ABOUT SECTION ===== */
        .about {
            background: var(--bg-secondary);
        }

        .about-inner {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 60px;
            align-items: start;
        }

        .about-visual {
            position: relative;
        }

        .about-image-container {
            width: 100%;
            max-width: 380px;
            aspect-ratio: 3/4;
            border-radius: var(--radius-lg);
            background: linear-gradient(145deg, var(--accent-soft), #e8e4dc);
            margin: 0 auto;
            position: relative;
            overflow: hidden;
            box-shadow: var(--shadow-lg);
        }

        .about-image-container::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-family: 'Playfair Display', serif;
            font-size: 8rem;
            font-weight: 700;
            color: rgba(184,134,11,0.12);
        }
        .about-image-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
}

        .about-decoration {
            position: absolute;
            bottom: -20px;
            right: -20px;
            width: 120px;
            height: 120px;
            border-radius: var(--radius-lg);
            border: 2px solid var(--accent);
            opacity: 0.2;
        }

        .about-content h2 {
            font-size: clamp(1.8rem, 3vw, 2.5rem);
            margin-bottom: 20px;
        }

        .about-text {
            font-size: 1rem;
            line-height: 1.85;
            color: var(--text-secondary);
            margin-bottom: 32px;
            font-weight: 300;
        }

        .about-highlights {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 12px;
            margin-bottom: 36px;
        }

        .highlight-tag {
            display: flex;
            align-items: center;
            gap: 8px;
            padding: 12px 16px;
            background: var(--bg-card);
            border-radius: var(--radius-sm);
            font-size: 0.8rem;
            font-weight: 500;
            color: var(--text-primary);
            border: 1px solid var(--border);
            transition: var(--transition);
        }

        .highlight-tag:hover {
            border-color: var(--accent);
            background: var(--accent-soft);
            transform: translateY(-2px);
        }

        .highlight-tag i {
            color: var(--accent);
            font-size: 0.75rem;
        }

        /* ===== SKILLS SECTION ===== */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 24px;
        }

        .skill-category {
            background: var(--bg-card);
            border-radius: var(--radius-lg);
            padding: 32px 28px;
            border: 1px solid var(--border);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .skill-category::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, var(--accent), var(--accent-light));
            opacity: 0;
            transition: var(--transition);
        }

        .skill-category:hover {
            border-color: rgba(184,134,11,0.3);
            box-shadow: var(--shadow-md);
            transform: translateY(-4px);
        }

        .skill-category:hover::before {
            opacity: 1;
        }

        .skill-category-icon {
            width: 44px;
            height: 44px;
            border-radius: var(--radius-md);
            background: var(--accent-soft);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--accent);
            font-size: 1.1rem;
            margin-bottom: 18px;
        }

        .skill-category h3 {
            font-family: 'Inter', sans-serif;
            font-size: 1rem;
            font-weight: 600;
            margin-bottom: 16px;
            color: var(--text-primary);
        }

        .skill-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .skill-tag {
            padding: 6px 14px;
            background: var(--bg-secondary);
            border-radius: 50px;
            font-size: 0.78rem;
            font-weight: 500;
            color: var(--text-secondary);
            border: 1px solid rgba(232,230,225,0.6);
            transition: var(--transition);
        }

        .skill-tag:hover {
            background: var(--accent-soft);
            color: var(--accent);
            border-color: rgba(184,134,11,0.2);
        }

        /* ===== PROJECTS SECTION ===== */
        .projects {
            background: var(--bg-secondary);
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
            gap: 28px;
        }

        .project-card {
            background: var(--bg-card);
            border-radius: var(--radius-lg);
            overflow: hidden;
            border: 1px solid var(--border);
            transition: var(--transition);
            cursor: pointer;
        }

        .project-card:hover {
            transform: translateY(-6px);
            box-shadow: var(--shadow-xl);
            border-color: rgba(184,134,11,0.25);
        }

        .project-image {
            width: 100%;
            aspect-ratio: 16/10;
            background: linear-gradient(135deg, var(--accent-soft) 0%, #e8e4dc 50%, var(--bg-secondary) 100%);
            position: relative;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .project-image-placeholder {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            font-weight: 600;
            color: var(--accent);
            opacity: 0.35;
            transition: var(--transition-slow);
        }

        .project-card:hover .project-image-placeholder {
            opacity: 0.55;
            transform: scale(1.05);
        }

        .project-image-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 40%;
            background: linear-gradient(to top, rgba(255,255,255,0.9), transparent);
            pointer-events: none;
        }

        .project-body {
            padding: 24px 28px 28px;
        }

        .project-title {
            font-family: 'Playfair Display', serif;
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 10px;
            color: var(--text-primary);
        }

        .project-description {
            font-size: 0.88rem;
            line-height: 1.7;
            color: var(--text-secondary);
            margin-bottom: 16px;
            font-weight: 300;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            margin-bottom: 20px;
        }

        .project-tag {
            padding: 4px 12px;
            background: var(--accent-soft);
            border-radius: 50px;
            font-size: 0.72rem;
            font-weight: 600;
            color: var(--accent);
            letter-spacing: 0.02em;
        }

        .project-link {
            display: inline-flex;
            align-items: center;
            gap: 6px;
            font-size: 0.85rem;
            font-weight: 600;
            color: var(--accent);
            text-decoration: none;
            transition: var(--transition);
        }

        .project-link:hover {
            gap: 10px;
            color: var(--accent-light);
        }

        /* Project Modal */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(26,26,46,0.6);
            backdrop-filter: blur(8px);
            z-index: 2000;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
            opacity: 0;
            pointer-events: none;
            transition: var(--transition);
        }

        .modal-overlay.active {
            opacity: 1;
            pointer-events: all;
        }

        .modal {
            background: var(--bg-card);
            border-radius: var(--radius-xl);
            max-width: 720px;
            width: 100%;
            max-height: 90vh;
            overflow-y: auto;
            transform: translateY(30px) scale(0.97);
            transition: var(--transition-slow);
            box-shadow: var(--shadow-xl);
        }

        .modal-overlay.active .modal {
            transform: translateY(0) scale(1);
        }

        .modal-header {
            padding: 32px 36px 0;
            display: flex;
            justify-content: space-between;
            align-items: start;
        }

        .modal-close {
            width: 36px;
            height: 36px;
            border-radius: 50%;
            border: 1px solid var(--border);
            background: var(--bg-secondary);
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1rem;
            color: var(--text-secondary);
            transition: var(--transition);
        }

        .modal-close:hover {
            background: var(--accent-soft);
            color: var(--accent);
            border-color: var(--accent);
        }

        .modal-body {
            padding: 24px 36px 36px;
        }

        .modal-project-title {
            font-family: 'Playfair Display', serif;
            font-size: 1.6rem;
            font-weight: 600;
            color: var(--text-primary);
            margin-bottom: 4px;
        }

        .modal-section {
            margin-bottom: 24px;
        }

        .modal-section-title {
            font-family: 'Inter', sans-serif;
            font-size: 0.75rem;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 0.12em;
            color: var(--accent);
            margin-bottom: 8px;
        }

        .modal-section p {
            font-size: 0.92rem;
            line-height: 1.75;
            color: var(--text-secondary);
            font-weight: 300;
        }

        .modal-tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .modal-tech-tag {
            padding: 6px 14px;
            background: var(--accent-soft);
            border-radius: 50px;
            font-size: 0.75rem;
            font-weight: 600;
            color: var(--accent);
        }

        .modal-image {
            width: 100%;
            aspect-ratio: 16/9;
            border-radius: var(--radius-md);
            background: linear-gradient(135deg, var(--accent-soft), var(--bg-secondary));
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .modal-image span {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            font-weight: 600;
            color: var(--accent);
            opacity: 0.25;
        }

        /* ===== CERTIFICATIONS ===== */
        .cert-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .cert-card {
            background: var(--bg-card);
            border-radius: var(--radius-md);
            padding: 28px 24px;
            border: 1px solid var(--border);
            transition: var(--transition);
            display: flex;
            flex-direction: column;
        }

        .cert-card:hover {
            border-color: rgba(184,134,11,0.3);
            box-shadow: var(--shadow-md);
            transform: translateY(-3px);
        }

        .cert-icon {
            width: 40px;
            height: 40px;
            border-radius: var(--radius-sm);
            background: var(--accent-soft);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--accent);
            font-size: 0.95rem;
            margin-bottom: 16px;
        }

        .cert-name {
            font-family: 'Inter', sans-serif;
            font-size: 0.95rem;
            font-weight: 600;
            color: var(--text-primary);
            margin-bottom: 6px;
            line-height: 1.4;
        }

        .cert-provider {
            font-size: 0.8rem;
            color: var(--text-light);
            margin-bottom: 4px;
        }

        .cert-year {
            font-size: 0.75rem;
            color: var(--text-light);
            margin-bottom: 16px;
        }

        .cert-link {
            display: inline-flex;
            align-items: center;
            gap: 6px;
            font-size: 0.78rem;
            font-weight: 600;
            color: var(--accent);
            text-decoration: none;
            transition: var(--transition);
            margin-top: auto;
        }

        .cert-link:hover {
            gap: 10px;
        }

        /* ===== SERVICES ===== */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
            gap: 24px;
        }

        .service-card {
            background: var(--bg-card);
            border-radius: var(--radius-lg);
            padding: 36px 28px;
            border: 1px solid var(--border);
            text-align: center;
            transition: var(--transition);
            position: relative;
        }

        .service-card::after {
            content: '';
            position: absolute;
            inset: 0;
            border-radius: var(--radius-lg);
            background: linear-gradient(135deg, rgba(184,134,11,0.03), transparent);
            opacity: 0;
            transition: var(--transition);
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-lg);
            border-color: rgba(184,134,11,0.2);
        }

        .service-card:hover::after {
            opacity: 1;
        }

        .service-icon {
            width: 56px;
            height: 56px;
            border-radius: var(--radius-md);
            background: var(--accent-soft);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--accent);
            font-size: 1.25rem;
            margin: 0 auto 18px;
            transition: var(--transition);
        }

        .service-card:hover .service-icon {
            background: var(--accent);
            color: white;
            transform: scale(1.08);
        }

        .service-card h3 {
            font-family: 'Inter', sans-serif;
            font-size: 0.95rem;
            font-weight: 600;
            margin-bottom: 10px;
            color: var(--text-primary);
        }

        .service-card p {
            font-size: 0.82rem;
            line-height: 1.7;
            color: var(--text-secondary);
            font-weight: 300;
        }

        /* ===== TIMELINE ===== */
        .timeline-section {
            background: var(--bg-secondary);
        }

        .timeline {
            position: relative;
            max-width: 700px;
            margin: 0 auto;
            padding-left: 40px;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 15px;
            top: 0;
            bottom: 0;
            width: 2px;
            background: linear-gradient(to bottom, var(--accent), var(--accent-teal));
        }

        .timeline-item {
            position: relative;
            margin-bottom: 48px;
            padding-left: 36px;
        }

        .timeline-item:last-child {
            margin-bottom: 0;
        }

        .timeline-dot {
            position: absolute;
            left: -40px;
            top: 4px;
            width: 14px;
            height: 14px;
            border-radius: 50%;
            background: var(--accent);
            border: 3px solid var(--bg-secondary);
            box-shadow: 0 0 0 3px rgba(184,134,11,0.15);
        }

        .timeline-label {
            font-family: 'Inter', sans-serif;
            font-size: 0.7rem;
            font-weight: 700;
            letter-spacing: 0.15em;
            text-transform: uppercase;
            color: var(--accent);
            margin-bottom: 6px;
        }

        .timeline-title {
            font-family: 'Inter', sans-serif;
            font-size: 1.05rem;
            font-weight: 600;
            color: var(--text-primary);
            margin-bottom: 4px;
        }

        .timeline-subtitle {
            font-size: 0.88rem;
            color: var(--text-secondary);
            font-weight: 400;
        }

        /* ===== WHY WORK WITH ME ===== */
        .why-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 24px;
            margin-bottom: 48px;
        }

        .why-card {
            background: var(--bg-card);
            border-radius: var(--radius-lg);
            padding: 32px 24px;
            text-align: center;
            border: 1px solid var(--border);
            transition: var(--transition);
        }

        .why-card:hover {
            border-color: rgba(184,134,11,0.25);
            box-shadow: var(--shadow-md);
            transform: translateY(-4px);
        }

        .why-icon {
            width: 48px;
            height: 48px;
            border-radius: 50%;
            background: var(--accent-soft);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--accent);
            font-size: 1.1rem;
            margin: 0 auto 14px;
        }

        .why-card h3 {
            font-family: 'Inter', sans-serif;
            font-size: 0.92rem;
            font-weight: 600;
            margin-bottom: 8px;
            color: var(--text-primary);
        }

        .why-card p {
            font-size: 0.82rem;
            line-height: 1.6;
            color: var(--text-secondary);
            font-weight: 300;
        }

        .why-statement {
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: clamp(1.1rem, 2vw, 1.35rem);
            font-style: italic;
            color: var(--text-secondary);
            max-width: 600px;
            margin: 0 auto;
            line-height: 1.6;
        }

        .why-statement::before,
        .why-statement::after {
            content: '"';
            color: var(--accent);
            font-size: 1.5em;
            opacity: 0.5;
        }

        /* ===== CONTACT ===== */
        .contact {
            background: var(--bg-dark);
            color: var(--text-white);
            position: relative;
            overflow: hidden;
        }

        .contact::before {
            content: '';
            position: absolute;
            top: -200px;
            right: -150px;
            width: 500px;
            height: 500px;
            background: radial-gradient(circle, rgba(184,134,11,0.08) 0%, transparent 70%);
            border-radius: 50%;
        }

        .contact .section-label { color: var(--accent-light); }
        .contact .section-title { color: var(--text-white); }
        .contact .section-subtitle { color: rgba(250,250,248,0.6); }

        .contact-inner {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 60px;
            align-items: start;
        }

        .contact-info h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.4rem;
            margin-bottom: 14px;
            color: var(--text-white);
        }

        .contact-info p {
            font-size: 0.92rem;
            line-height: 1.7;
            color: rgba(250,250,248,0.6);
            margin-bottom: 32px;
            font-weight: 300;
        }

        .social-links {
            display: flex;
            gap: 12px;
        }

        .social-link {
            width: 46px;
            height: 46px;
            border-radius: 50%;
            border: 1px solid rgba(250,250,248,0.15);
            display: flex;
            align-items: center;
            justify-content: center;
            color: rgba(250,250,248,0.7);
            text-decoration: none;
            font-size: 1rem;
            transition: var(--transition);
        }

        .social-link:hover {
            background: var(--accent);
            border-color: var(--accent);
            color: white;
            transform: translateY(-3px);
        }

        .contact-form {
            display: flex;
            flex-direction: column;
            gap: 18px;
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 18px;
        }

        .form-group {
            display: flex;
            flex-direction: column;
            gap: 6px;
        }

        .form-group label {
            font-size: 0.75rem;
            font-weight: 600;
            letter-spacing: 0.08em;
            text-transform: uppercase;
            color: rgba(250,250,248,0.5);
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 14px 18px;
            border-radius: var(--radius-sm);
            border: 1px solid rgba(250,250,248,0.12);
            background: rgba(250,250,248,0.06);
            color: var(--text-white);
            font-family: 'Inter', sans-serif;
            font-size: 0.9rem;
            transition: var(--transition);
            outline: none;
        }

        .form-group input::placeholder,
        .form-group textarea::placeholder {
            color: rgba(250,250,248,0.25);
        }

        .form-group input:focus,
        .form-group textarea:focus {
            border-color: var(--accent);
            background: rgba(184,134,11,0.05);
            box-shadow: 0 0 0 3px rgba(184,134,11,0.1);
        }

        .form-group textarea {
            min-height: 130px;
            resize: vertical;
        }

        .btn-submit {
            background: var(--accent);
            color: white;
            padding: 16px 40px;
            border: none;
            border-radius: 50px;
            font-family: 'Inter', sans-serif;
            font-size: 0.9rem;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            letter-spacing: 0.02em;
            align-self: flex-start;
        }

        .btn-submit:hover {
            background: var(--accent-light);
            transform: translateY(-2px);
            box-shadow: 0 6px 24px rgba(184,134,11,0.3);
        }

        .btn-submit:disabled {
            opacity: 0.6;
            cursor: not-allowed;
            transform: none;
        }

        #form-message {
            font-size: 0.85rem;
            font-weight: 500;
            min-height: 1.2em;
        }

        /* ===== FOOTER ===== */
        .footer {
            background: #12122A;
            color: rgba(250,250,248,0.5);
            padding: 48px 0;
        }

        .footer-inner {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 24px;
        }

        .footer-brand {
            text-align: center;
        }

        .footer-brand h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.25rem;
            color: var(--text-white);
            margin-bottom: 4px;
        }

        .footer-brand p {
            font-size: 0.78rem;
            letter-spacing: 0.04em;
            color: rgba(250,250,248,0.4);
        }

        .footer-nav {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
            justify-content: center;
        }

        .footer-nav a {
            text-decoration: none;
            color: rgba(250,250,248,0.5);
            font-size: 0.82rem;
            font-weight: 500;
            transition: var(--transition);
        }

        .footer-nav a:hover {
            color: var(--accent-light);
        }

        .footer-social {
            display: flex;
            gap: 12px;
        }

        .footer-social a {
            width: 36px;
            height: 36px;
            border-radius: 50%;
            border: 1px solid rgba(250,250,248,0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            color: rgba(250,250,248,0.4);
            text-decoration: none;
            font-size: 0.85rem;
            transition: var(--transition);
        }

        .footer-social a:hover {
            background: var(--accent);
            border-color: var(--accent);
            color: white;
        }

        .footer-divider {
            width: 100%;
            max-width: 300px;
            height: 1px;
            background: rgba(250,250,248,0.06);
        }

        .footer-copy {
            font-size: 0.75rem;
            color: rgba(250,250,248,0.3);
            text-align: center;
        }

        /* ===== ANIMATIONS ===== */
        .reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.7s ease, transform 0.7s ease;
        }

        .reveal.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .reveal-delay-1 { transition-delay: 0.1s; }
        .reveal-delay-2 { transition-delay: 0.2s; }
        .reveal-delay-3 { transition-delay: 0.3s; }
        .reveal-delay-4 { transition-delay: 0.4s; }
        .reveal-delay-5 { transition-delay: 0.5s; }

        /* ===== SCROLLBAR ===== */
        ::-webkit-scrollbar {
            width: 6px;
        }
        ::-webkit-scrollbar-track {
            background: var(--bg-primary);
        }
        ::-webkit-scrollbar-thumb {
            background: var(--border);
            border-radius: 3px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: var(--accent);
        }

        /* ===== RESPONSIVE ===== */
        @media (max-width: 1024px) {
            .hero-inner {
                grid-template-columns: 1fr;
                text-align: center;
                gap: 40px;
            }
            .hero-content { order: 2; }
            .hero-visual { order: 1; }
            .hero-description { margin: 0 auto 36px; }
            .hero-buttons { justify-content: center; }
            .hero-visual-container { max-width: 350px; margin: 0 auto; }
            .about-inner {
                grid-template-columns: 1fr;
                gap: 40px;
            }
            .about-visual { text-align: center; }
            .about-image-container { max-width: 280px; }
            .contact-inner {
                grid-template-columns: 1fr;
                gap: 40px;
            }
        }

        @media (max-width: 768px) {
            section { padding: 72px 0; }
            .nav-links { display: none; }
            .hamburger { display: flex; }
            .mobile-menu { display: flex; }
            .hero-avatar-ring { width: 220px; height: 220px; }
            .hero-avatar { width: 170px; height: 170px; }
            .hero-avatar-placeholder { font-size: 3.5rem; }
            .floating-card { display: none; }
            .floating-card.fc-1, .floating-card.fc-4 { display: flex; }
            .fc-1 { top: 5%; right: 0; }
            .fc-4 { top: 5%; left: 0; }
            .about-highlights {
                grid-template-columns: repeat(2, 1fr);
            }
            .projects-grid {
                grid-template-columns: 1fr;
            }
            .form-row {
                grid-template-columns: 1fr;
            }
            .hero-visual-container { max-width: 280px; }
        }

        @media (max-width: 480px) {
            .container { padding: 0 16px; }
            section { padding: 56px 0; }
            .hero-name { font-size: 2.2rem; }
            .hero-buttons { flex-direction: column; align-items: center; }
            .btn { width: 100%; justify-content: center; }
            .skills-grid {
                grid-template-columns: 1fr;
            }
            .services-grid {
                grid-template-columns: 1fr;
            }
            .why-grid {
                grid-template-columns: 1fr;
            }
            .cert-grid {
                grid-template-columns: 1fr;
            }
            .about-highlights {
                grid-template-columns: 1fr;
            }
            .modal-header { padding: 24px 20px 0; }
            .modal-body { padding: 16px 20px 24px; }
            .footer-nav { gap: 14px; }
        }

        /* ===== BACK TO TOP ===== */
        .back-to-top {
            position: fixed;
            bottom: 28px;
            right: 28px;
            width: 44px;
            height: 44px;
            border-radius: 50%;
            background: var(--accent);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1rem;
            cursor: pointer;
            border: none;
            box-shadow: 0 4px 16px rgba(184,134,11,0.25);
            opacity: 0;
            transform: translateY(20px);
            transition: var(--transition);
            z-index: 900;
        }

        .back-to-top.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .back-to-top:hover {
            background: var(--accent-light);
            transform: translateY(-3px);
        }


        /* ===== ACCESSIBILITY IMPROVEMENTS ===== */
        .skip-link {
            position: fixed;
            top: 12px;
            left: 12px;
            z-index: 3000;
            padding: 10px 16px;
            border-radius: var(--radius-sm);
            background: var(--bg-dark);
            color: var(--text-white);
            text-decoration: none;
            transform: translateY(-160%);
            transition: var(--transition);
        }

        .skip-link:focus {
            transform: translateY(0);
        }

        .hamburger {
            background: transparent;
            border: 0;
        }

        .project-card:focus-visible,
        .hamburger:focus-visible,
        .modal-close:focus-visible,
        .project-link:focus-visible,
        .btn:focus-visible,
        .btn-submit:focus-visible,
        .back-to-top:focus-visible {
            outline: 3px solid var(--accent-light);
            outline-offset: 3px;
        }

        .project-link-button {
            background: transparent;
            border: 0;
            padding: 0;
            font: inherit;
            cursor: pointer;
        }

        @media (prefers-reduced-motion: reduce) {
            html { scroll-behavior: auto; }
            *, *::before, *::after {
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
                transition-duration: 0.01ms !important;
                scroll-behavior: auto !important;
            }
        }
    </style>
</head>
<body>
    <a class="skip-link" href="#main-content">Skip to main content</a>

    <!-- Navigation -->
    <nav class="navbar" id="navbar">
        <div class="nav-inner">
            <a href="#home" class="nav-logo">Sawsan Taleb Alhaddad<span></span></a>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#certifications">Certifications</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
<li><a href="mailto:s.alhaddad1136@gmail.com" class="nav-cta">Let's Work Together</a></li>            </ul>
            <button class="hamburger" id="hamburger" type="button" aria-label="Open navigation menu" aria-expanded="false" aria-controls="mobileMenu">
                <span></span>
                <span></span>
                <span></span>
            </button>
        </div>
    </nav>

    <!-- Mobile Menu -->
    <div class="mobile-menu" id="mobileMenu" aria-label="Mobile navigation">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#certifications">Certifications</a>
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
        <a href="#contact" class="btn btn-primary btn-small">Let's Work Together</a>
    </div>

    <main id="main-content">

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-inner">
                <div class="hero-content">
                    <div class="hero-greeting"> Welcome to my portfolio</div>
                    <h1 class="hero-name">Hi, I'm <span class="accent">Sawsan</span></h1>
                    <p class="hero-title">Information Systems Graduate</p>
                    <p class="hero-subtitle">Web Developer &bull; UI/UX Designer &bull; Digital Creator</p>
                    <p class="hero-description">I combine technology, creativity, and user-centered design to create modern digital experiences and practical web solutions.</p>
                    <div class="hero-buttons">
                        <a href="#projects" class="btn btn-primary">
                            <i class="fas fa-th-large"></i> View My Projects
                        </a>
                        <a href="https://www.linkedin.com/in/sawsan-a-b72647134?utm_source=share_via&utm_content=profile&utm_medium=member_ios" class="btn btn-secondary" target="_blank" rel="noopener noreferrer">
                            <i class="fas fa-envelope"></i> Contact Me
                        </a>
                    </div>
                </div>
                <div class="hero-visual">
                    <div class="hero-visual-container">
                        <div class="hero-avatar-ring"></div>
                        <div class="hero-avatar">
                            <span class="hero-avatar-placeholder">S</span>
                        </div>
                        <!-- Floating UI Cards -->
                        <div class="floating-card fc-1">
                            <div class="card-icon"><i class="fas fa-code"></i></div>
                            <span>Web Development</span>
                        </div>
                        <div class="floating-card fc-2">
                            <div class="card-icon"><i class="fas fa-palette"></i></div>
                            <span>UI/UX Design</span>
                        </div>
                        <div class="floating-card fc-3">
                            <div class="card-icon"><i class="fas fa-cloud"></i></div>
                            <span>Cloud Solutions</span>
                        </div>
                        <div class="floating-card fc-4">
                            <div class="card-icon"><i class="fas fa-database"></i></div>
                            <span>Database Dev</span>
                        </div>
                        <div class="floating-card fc-5">
                            <div class="card-icon"><i class="fas fa-pen-nib"></i></div>
                            <span>Digital Design</span>
                        </div>
                        
                    </div>
                    
                </div>
                
                        
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="about-inner">
                <div class="about-visual reveal">
                   <div class="about-image-container">
    <img src="CVV.jpg" alt="Portrait of Sawsan Alhaddad" loading="lazy" decoding="async">
</div>
                    <div class="about-decoration"></div>
                </div>
                <div class="about-content">
                    <span class="section-label reveal">About Me</span>
                    <h2 class="reveal reveal-delay-1">Passionate about turning<br>ideas into digital reality</h2>
                    <p class="about-text reveal reveal-delay-2">Sawsan Alhaddad is an information systems graduate from the University of Bahrain with a passion for combining technology, design, and creativity. Her interests include web development, UI/UX design, database management, cloud and IT solutions, and digital content creation. She enjoys transforming ideas into modern, user-friendly, and visually engaging digital experiences. With a creative mindset and a strong interest in technology, she is eager to apply her skills to real-world projects, continue learning, and create meaningful digital solutions.</p>
                    <div class="about-highlights reveal reveal-delay-3">
                        <div class="highlight-tag"><i class="fas fa-check"></i> Information Systems</div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> Web Development</div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> UI/UX Design</div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> Digital Creativity</div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> Database Development</div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> Cloud & IT Solutions</div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> Video Editing</div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> AR & Snapchat Lens Desig </div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> Photo Editing </div>
                        <div class="highlight-tag"><i class="fas fa-check"></i> Social Media Content </div>




                    </div>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:AP:037e28e3-916e-42e1-b997-8821a8e35f16" class="btn btn-primary reveal reveal-delay-4" target="_blank" rel="noopener noreferrer">
                        <i class="fas fa-download"></i> Download CV
                    </a>
                   
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <div class="container">
            <div class="section-header">
                <span class="section-label reveal">Skills & Expertise</span>
                <h2 class="section-title reveal reveal-delay-1">My Technical Toolkit</h2>
                <p class="section-subtitle reveal reveal-delay-2">A blend of development, design, and information systems skills that enable me to build complete digital solutions.</p>
            </div>
            <div class="skills-grid">
                <div class="skill-category reveal">
                    <div class="skill-category-icon"><i class="fas fa-code"></i></div>
                    <h3>Web Development</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">HTML</span>
                        <span class="skill-tag">CSS</span>
                        <span class="skill-tag">JavaScript</span>
                        <span class="skill-tag">PHP</span>
                        <span class="skill-tag">MySQL</span>
                    </div>
                </div>
                <div class="skill-category reveal reveal-delay-1">
                    <div class="skill-category-icon"><i class="fas fa-pen-ruler"></i></div>
                    <h3>UI/UX Design</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">User Interface</span>
                        <span class="skill-tag">User Experience</span>
                        <span class="skill-tag">Wireframing</span>
                        <span class="skill-tag">Prototyping</span>
                        <span class="skill-tag">Usability</span>
                        <span class="skill-tag">Responsive Design</span>
                    </div>
                </div>
                <div class="skill-category reveal reveal-delay-2">
                    <div class="skill-category-icon"><i class="fas fa-sitemap"></i></div>
                    <h3>Information Systems</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Systems Analysis</span>
                        <span class="skill-tag">Database Management</span>
                        <span class="skill-tag">IT Governance</span>
                        <span class="skill-tag">Enterprise Systems</span>
                        <span class="skill-tag">IT Audit</span>
                    </div>
                </div>
                <div class="skill-category reveal reveal-delay-3">
                    <div class="skill-category-icon"><i class="fas fa-cloud"></i></div>
                    <h3>Cloud & Technology</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">AWS</span>
                        <span class="skill-tag">Cloud Computing</span>
                        <span class="skill-tag">Cybersecurity</span>
                        <span class="skill-tag">Digital Solutions</span>
                    </div>
                </div>
                <div class="skill-category reveal reveal-delay-4">
                    <div class="skill-category-icon"><i class="fas fa-paint-brush"></i></div>
                    <h3>Design Tools</h3>
                    <div class="skill-tags">
                        <span class="skill-tag">Canva</span>
                        <span class="skill-tag">Adobe Creative Tools</span>
                        <span class="skill-tag">Figma</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section class="projects" id="projects">
        <div class="container">
            <div class="section-header">
                <span class="section-label reveal">Featured Work</span>
                <h2 class="section-title reveal reveal-delay-1">Projects That Define Me</h2>
                <p class="section-subtitle reveal reveal-delay-2">Each project reflects my passion for creating meaningful digital experiences through thoughtful design and solid development.</p>
            </div>
            <div class="projects-grid">
                <!-- Project 1: JVAL Jewelry -->
                <div class="project-card reveal" role="button" tabindex="0" data-project-index="0" aria-label="View details for JVAL Jewelry Website">
                    <div class="project-image">
                        <span class="project-image-placeholder">JVAL</span>
                        <div class="project-image-overlay"></div>
                    </div>
                    <div class="project-body">
                        <h3 class="project-title">JVAL Jewelry Website</h3>
                        <p class="project-description">A creative jewelry e-commerce website concept developed with modern web technologies and 3D technology to create an engaging product experience.</p>
                        <div class="project-tags">
                            <span class="project-tag">Web Development</span>
                            <span class="project-tag">3D Technology</span>
                            <span class="project-tag">UI/UX</span>
                        </div>
                        <a href="https://jvaljewelry.framer.website/" class="project-link" target="_blank" rel="noopener noreferrer">Visit Website <i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>

                <!-- Project 4: UCAS UI/UX -->
                <div class="project-card reveal reveal-delay-3" role="button" tabindex="0" data-project-index="3" aria-label="View details for UCAS UI/UX Project">
                    <div class="project-image" style="background: linear-gradient(135deg, #e8dfd4 0%, #e8e4dc 50%, var(--bg-secondary) 100%);">
                        <span class="project-image-placeholder">UCAS</span>
                        <div class="project-image-overlay"></div>
                    </div>
                    <div class="project-body">
                        <h3 class="project-title">UCAS UI/UX Project</h3>
                        <p class="project-description">A user interface and user experience project focused on improving university application-related services.</p>
                        <div class="project-tags">
                            <span class="project-tag">User Research</span>
                            <span class="project-tag">Wireframing</span>
                            <span class="project-tag">Usability</span>
                            <span class="project-tag">UI Design</span>
                            <span class="project-tag">Prototyping</span>
                        </div>
                        <a href="https://www.figma.com/proto/Gyiaw4MS1mcx6X6dLdHXfe/%D8%A7%D9%84%D8%A8%D8%B1%D9%88%D8%AC%D9%83%D8%AA?node-id=142-5623&t=TEnIj76cbSxE65xq-1" class="project-link" target="_blank" rel="noopener noreferrer">View Prototype <i class="fas fa-external-link-alt"></i></a>
                    </div>
                </div>

                <!-- Project 5: Digital Design Collection -->
                <div class="project-card reveal reveal-delay-4" role="button" tabindex="0" data-project-index="4" aria-label="View details for Digital Design Collection">
                    <div class="project-image" style="background: linear-gradient(135deg, #f5ecd7 0%, #e8e4dc 50%, var(--bg-secondary) 100%);">
                        <span class="project-image-placeholder">DESIGN</span>
                        <div class="project-image-overlay"></div>
                    </div>
                    <div class="project-body">
                        <h3 class="project-title">Digital Design Collection</h3>
                        <p class="project-description">A creative collection of digital designs including invitations, graduation designs, social media graphics, and visual content created with a modern and elegant style.</p>
                        <div class="project-tags">
                            <span class="project-tag">Graphic Design</span>
                            <span class="project-tag">Canva</span>
                            <span class="project-tag">Digital Design</span>
                            <span class="project-tag">Social Media</span>
                            <span class="project-tag">Visual Content</span>
                        </div>
                        <button type="button" class="project-link project-link-button" data-open-project="4">View Details <i class="fas fa-arrow-right"></i></button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Project Modal -->
    <div class="modal-overlay" id="projectModal" aria-hidden="true">
        <div class="modal" role="dialog" aria-modal="true" aria-labelledby="modalTitle">
            <div class="modal-header">
                <div>
                    <h2 class="modal-project-title" id="modalTitle"></h2>
                </div>
                <button class="modal-close" id="modalClose" type="button" aria-label="Close project details"><i class="fas fa-times"></i></button>
            </div>
            <div class="modal-body" id="modalBody">
                <!-- Content injected by JS -->
            </div>
        </div>
    </div>

    <!-- Certifications Section -->
     
    <section id="certifications">
        <div class="container">
            <div class="section-header">
            
                <span class="section-label reveal">Credentials</span>
                <h2 class="section-title reveal reveal-delay-1">Certifications & Training</h2>
                <p class="section-subtitle reveal reveal-delay-2">Continuously learning and growing through professional certifications and specialized training programs.</p>
            </div>
            <div class="cert-grid">
                <div class="cert-card reveal">
                    <div class="cert-icon"><i class="fas fa-certificate"></i></div>
                    <h3 class="cert-name">Becoming an SAP Professional</h3>
                    <p class="cert-provider">SAP Learning</p>
                    <p class="cert-year">Professional Certification</p>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:AP:b1b8b9e1-a4d8-4f2e-ba58-659dc88bb738" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate <i class="fas fa-external-link-alt"></i></a>
                </div>
                <div class="cert-card reveal reveal-delay-1">
                    <div class="cert-icon"><i class="fas fa-building"></i></div>
                    <h3 class="cert-name">Planning, Auditing, and Maintaining Enterprise Systems</h3>
                    <p class="cert-provider">Enterprise Systems</p>
                    <p class="cert-year">Professional Certification</p>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:AP:c22bbc90-d7de-419f-aa94-366799aa6862" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate <i class="fas fa-external-link-alt"></i></a>
                </div>
                <div class="cert-card reveal reveal-delay-2">
                    <div class="cert-icon"><i class="fas fa-layer-group"></i></div>
                    <h3 class="cert-name">TOGAF 10 Foundation</h3>
                    <p class="cert-provider">The Open Group</p>
                    <p class="cert-year">Professional Certification</p>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:ap:216250c4-6a2f-4003-b60b-9254855023d4" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate <i class="fas fa-external-link-alt"></i></a>
                </div>
                <div class="cert-card reveal reveal-delay-3">
                    <div class="cert-icon"><i class="fas fa-cubes"></i></div>
                    <h3 class="cert-name">Services-Oriented Architecture</h3>
                    <p class="cert-provider">SOA Training</p>
                    <p class="cert-year">Professional Certification</p>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:AP:96e124d3-bd69-4346-b10e-f9322a861286" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate <i class="fas fa-external-link-alt"></i></a>
                </div>
                <div class="cert-card reveal reveal-delay-4">
                    <div class="cert-icon"><i class="fas fa-chart-gantt"></i></div>
                    <h3 class="cert-name">How to Create a Gantt Chart in Wrike</h3>
                    <p class="cert-provider">Wrike</p>
                    <p class="cert-year">Professional Training</p>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:AP:b86dc7e6-8552-45f9-94b4-53364a739023" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate <i class="fas fa-external-link-alt"></i></a>
                </div>
                <div class="cert-card reveal reveal-delay-5">
                    <div class="cert-icon"><i class="fas fa-rocket"></i></div>
                    <h3 class="cert-name">Get Started with Wrike</h3>
                    <p class="cert-provider">Wrike</p>
                    <p class="cert-year">Professional Training</p>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:AP:c3113f15-f8bd-4921-bef3-b1818970294a" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate <i class="fas fa-external-link-alt"></i></a>
                </div>
                <div class="cert-card reveal">
                    <div class="cert-icon"><i class="fas fa-database"></i></div>
                    <h3 class="cert-name">Using MySQL Database with PHP</h3>
                    <p class="cert-provider">Web Development</p>
                    <p class="cert-year">Professional Certification</p>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:AP:e6843129-1408-46a6-b36f-acd95bfb92bd" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate <i class="fas fa-external-link-alt"></i></a>
                </div>
                <div class="cert-card reveal reveal-delay-1">
                    <div class="cert-icon"><i class="fas fa-globe"></i></div>
                    <h3 class="cert-name">Building a Dynamic Web App Using PHP & MySQL</h3>
                    <p class="cert-provider">Web Development</p>
                    <p class="cert-year">Professional Certification</p>
                    <a href="https://acrobat.adobe.com/id/urn:aaid:sc:AP:59ae51b7-5911-482d-a606-6315a8b558c0" class="cert-link" target="_blank" rel="noopener noreferrer">View Certificate <i class="fas fa-external-link-alt"></i></a>
                </div>

            </div>
            
        </div>
        
    </section>


    <!-- Services Section -->
    <section class="services-section" id="services">
        <div class="container">
            <div class="section-header">
                <span class="section-label reveal">What I Offer</span>
                <h2 class="section-title reveal reveal-delay-1">What I Can Do</h2>
                <p class="section-subtitle reveal reveal-delay-2">Turning your vision into reality with a combination of technical skill and creative design thinking.</p>
            </div>
            <div class="services-grid">
                <div class="service-card reveal">
                    <div class="service-icon"><i class="fas fa-code"></i></div>
                    <h3>Web Development</h3>
                    <p>Modern responsive websites using HTML, CSS, JavaScript, PHP and MySQL.</p>
                </div>
                <div class="service-card reveal reveal-delay-1">
                    <div class="service-icon"><i class="fas fa-pen-ruler"></i></div>
                    <h3>UI/UX Design</h3>
                    <p>Clean and user-friendly interfaces focused on usability and user experience.</p>
                </div>
                <div class="service-card reveal reveal-delay-2">
                    <div class="service-icon"><i class="fas fa-pen-nib"></i></div>
                    <h3>Digital Design</h3>
                    <p>Creative digital products including templates, cards, planners and social media designs.</p>
                </div>
                <div class="service-card reveal reveal-delay-3">
                    <div class="service-icon"><i class="fas fa-desktop"></i></div>
                    <h3>Website Design</h3>
                    <p>Modern landing pages and portfolio/business websites.</p>
                </div>
                <div class="service-card reveal reveal-delay-4">
                    <div class="service-icon"><i class="fas fa-database"></i></div>
                    <h3>Database Solutions</h3>
                    <p>Basic database-driven web applications using PHP and MySQL.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience / Education Timeline -->
    <section class="timeline-section" id="experience">
        <div class="container">
            <div class="section-header">
                <span class="section-label reveal">My Journey</span>
                <h2 class="section-title reveal reveal-delay-1">Experience & Education</h2>
            </div>
            <div class="timeline">
                <div class="timeline-item reveal">
                    <div class="timeline-dot"></div>
                    <div class="timeline-label">Education</div>
                    <h3 class="timeline-title">University of Bahrain</h3>
                    <p class="timeline-subtitle">Bachelor's Degree in Information Systems | Started: 2020-Finished: 2026</p>
                </div>
                <div class="timeline-item reveal reveal-delay-1">
                    <div class="timeline-dot"></div>
                    <div class="timeline-label">Professional Training</div>
                    <h3 class="timeline-title">University of Bahrain - Vocational Training</h3>
                   <p class="timeline-subtitle">
                   Hydro Company | 3 June 2025 – 31 July 2025</p>              
                  </div>
                
            </div>
        </div>
    </section>

    <!-- Why Work With Me -->
    <section id="why-me">
        <div class="container">
            <div class="section-header">
                <span class="section-label reveal">My Approach</span>
                <h2 class="section-title reveal reveal-delay-1">Why Work With Me</h2>
            </div>
            <div class="why-grid">
                <div class="why-card reveal">
                    <div class="why-icon"><i class="fas fa-lightbulb"></i></div>
                    <h3>Creative Thinking</h3>
                    <p>Bringing fresh, innovative ideas to every project with a creative problem-solving mindset.</p>
                </div>
                <div class="why-card reveal reveal-delay-1">
                    <div class="why-icon"><i class="fas fa-microchip"></i></div>
                    <h3>Technical Knowledge</h3>
                    <p>Solid foundation in information systems, web technologies, and cloud computing.</p>
                </div>
                <div class="why-card reveal reveal-delay-2">
                    <div class="why-icon"><i class="fas fa-user-check"></i></div>
                    <h3>User-Centered Design</h3>
                    <p>Designing with the user in mind — every decision is guided by empathy and usability.</p>
                </div>
                <div class="why-card reveal reveal-delay-3">
                    <div class="why-icon"><i class="fas fa-search"></i></div>
                    <h3>Attention to Detail</h3>
                    <p>Precision in every pixel and interaction, ensuring a polished and professional result.</p>
                </div>
            </div>
            <p class="why-statement reveal reveal-delay-4">I believe great digital products combine functionality, simplicity, and creativity.</p>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-header">
                <span class="section-label reveal">Get In Touch</span>
                <h2 class="section-title reveal reveal-delay-1">Let's Create Something Great Together</h2>
                <p class="section-subtitle reveal reveal-delay-2">Have a project, idea, or opportunity? I'd love to hear about it.</p>
            </div>
            <div class="contact-inner">
                <div class="contact-info reveal">
                    <h3>Let's connect</h3>
                    <p>Whether you have a project in mind, a question, or just want to say hello . I'm always open to discussing new opportunities and creative ideas.</p>
                </div>
              <form id="contact-form" class="contact-form">

    <!-- Web3Forms Access Key -->
    <input type="hidden"
           name="access_key"
           value="b77ea6ba-86a0-4a2a-b5fb-0e1c45286ac4">

    <!-- Email Subject -->
    <input type="hidden"
           name="subject"
           value="New Message From Sawsan Portfolio">

    <!-- Bot Protection -->
    <input type="checkbox"
           name="botcheck"
           style="display: none;">

    <div class="form-row">

        <div class="form-group">
            <label for="name">Name</label>

            <input
                type="text"
                id="name"
                name="name"
                placeholder="Your Name"
                required
            >
        </div>


        <div class="form-group">
            <label for="email">Email</label>

            <input
                type="email"
                id="email"
                name="email"
                placeholder="Your Email"
                required
            >
        </div>

    </div>


    <div class="form-group">
        <label for="message">Message</label>

        <textarea
            id="message"
            name="message"
            rows="6"
            placeholder="Write your message..."
            required
        ></textarea>
    </div>


    <button
        type="submit"
        id="send-button"
        class="btn-submit"
    >
        Send Message
    </button>


    <!-- Success / Error Message -->
    <p id="form-message" role="status" aria-live="polite"></p>

</form>
            </div>
        </div>
    </section>

    </main>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-inner">
                <div class="footer-brand">
                    <h3>Sawsan Taleb Alhaddad</h3>
                    <p>Information Systems Graduate | Web Developer | UI/UX Designer | Digital Creator</p>
                </div>
                <nav class="footer-nav" aria-label="Footer navigation">
                    <a href="#home">Home</a>
                    <a href="#about">About</a>
                    <a href="#skills">Skills</a>
                    <a href="#projects">Projects</a>
                    <a href="#certifications">Certifications</a>
                    <a href="#services">Services</a>
                    <a href="#contact">Contact</a>
                </nav>
                <div class="footer-social">
                    <a href="https://www.linkedin.com/in/sawsan-a-b72647134?utm_source=share_via&utm_content=profile&utm_medium=member_ios" aria-label="LinkedIn" title="LinkedIn" target="_blank" rel="noopener noreferrer"><i class="fab fa-linkedin-in"></i></a>
                    <a href="mailto:s.alhaddad1136@gmail.com" aria-label="Email" title="Email"><i class="fas fa-envelope"></i></a>
                </div>
                <div class="footer-divider"></div>
                <p class="footer-copy">&copy; 2026 Sawsan Alhaddad. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Back to Top -->
    <button class="back-to-top" id="backToTop" aria-label="Back to top">
        <i class="fas fa-chevron-up"></i>
    </button>

    <script>
        // ===== Project Data =====
        const projects = [
            {
                title: "JVAL Jewelry Website",
                overview: "A creative jewelry e-commerce website concept that brings luxury products to life through modern web technologies and immersive 3D experiences.",
                problem: "Traditional jewelry websites often lack the immersive experience that customers need to appreciate the craftsmanship and detail of each piece. Static images fail to convey the beauty and quality of fine jewelry.",
                solution: "Developed a modern e-commerce concept using 3D product visualization, smooth animations, and an elegant UI that reflects the luxury nature of the brand while maintaining excellent usability.",
                role: "Web Developer & UI/UX Designer",
                tools: ["HTML", "CSS", "JavaScript", "3D Technology", "UI/UX Design Tools"],
                process: "Started with market research and competitive analysis, then moved to wireframing and prototyping the user journey. Designed the visual identity to match the luxury brand feel, and implemented interactive 3D product views for an engaging shopping experience.",
                result: "A fully concept e-commerce website that demonstrates how modern web technologies can elevate the online jewelry shopping experience, making products feel tangible and desirable.",
                imageText: "JVAL"
            },
            {
                title: "Cloud Based Citizen Services Platform",
                overview: "A cloud-based platform concept designed to integrate Bahrain government services into a unified, modern web and mobile experience for citizens.",
                problem: "Citizens often need to access multiple government services through disconnected systems, leading to poor user experience, duplicated efforts, and inefficient service delivery.",
                solution: "Designed a cloud-native platform architecture on AWS that centralizes government services, provides a seamless user experience across web and mobile, and ensures scalability and security through proper cloud infrastructure.",
                role: "Cloud Architect & Platform Designer",
                tools: ["AWS EC2", "RDS", "S3", "VPC", "CloudFront", "API Gateway", "UI/UX Design"],
                process: "Analyzed existing government service channels, mapped citizen journey pain points, then designed a cloud architecture that addresses scalability, security, and performance requirements. Created responsive UI designs for both web and mobile interfaces.",
                result: "A comprehensive cloud platform concept demonstrating how modern cloud architecture and user-centered design can transform government service delivery into an efficient, citizen-friendly experience.",
                imageText: "CCS"
            },
            {
                title: "Cybersecurity Maturity Model",
                overview: "A research project focused on developing a cybersecurity maturity model to assess and improve cybersecurity resilience for micro-enterprises and nonprofit organizations.",
                problem: "Micro-enterprises and nonprofit organizations often lack the resources, expertise, and structured approaches to build effective cybersecurity defenses, leaving them vulnerable to increasingly sophisticated threats.",
                solution: "Developed a practical maturity model that provides these organizations with a clear roadmap for improving their cybersecurity posture, covering risk management, security awareness, governance, and incident response capabilities.",
                role: "Researcher & Model Developer",
                tools: ["Risk Management Frameworks", "Security Analysis", "Governance Models", "Incident Response Planning"],
                process: "Conducted extensive literature review on existing cybersecurity frameworks, analyzed the specific constraints and needs of micro-enterprises and nonprofits, then synthesized a tailored maturity model with actionable assessment criteria and improvement pathways.",
                result: "A research-backed cybersecurity maturity model that gives resource-constrained organizations a practical, step-by-step approach to strengthening their security posture and building resilience against cyber threats.",
                imageText: "CSM"
            },
            {
                title: "UCAS UI/UX Project",
                overview: "A comprehensive UI/UX project focused on improving the user experience of university application-related services, making the process more intuitive and less stressful for applicants.",
                problem: "University application systems are often complex, confusing, and stressful for students to navigate, leading to errors, missed deadlines, and a poor overall experience during a critical life moment.",
                solution: "Redesigned the application experience through extensive user research, simplified information architecture, clear visual hierarchy, and intuitive interaction patterns that guide applicants through the process with confidence.",
                role: "UI/UX Designer & Researcher",
                tools: ["User Research", "Wireframing", "Figma", "Prototyping", "Usability Testing"],
                process: "Conducted user interviews and surveys with university applicants, created user personas and journey maps, designed low-fidelity wireframes, iterated based on feedback, built interactive prototypes, and validated through usability testing sessions.",
                result: "A redesigned application experience that significantly reduces cognitive load, guides users through complex processes, and transforms a stressful experience into a clear, confident journey toward their academic goals.",
                imageText: "UCAS"
            },
            {
                title: "Digital Design Collection",
                overview: "A curated showcase of digital products and creative designs including planners, CV templates, graduation cards, wedding designs, and social media content that demonstrate creative versatility.",
                problem: "Many individuals and small businesses need professionally designed digital products but lack the design skills or budget for custom work, relying on generic templates that don't stand out.",
                solution: "Created a collection of thoughtfully designed, customizable digital products that combine aesthetic appeal with practical functionality, each tailored to specific use cases and personal styles.",
                role: "Digital Designer & Creative Director",
                tools: ["Canva", "Adobe Creative Tools", "Figma", "Digital Illustration"],
                process: "Identified common design needs across different occasions and professional contexts, developed consistent visual systems for each product category, and refined designs based on practical usability and aesthetic appeal.",
                result: "A diverse portfolio of digital designs that showcase creative range and attention to detail, from elegant wedding stationery to professional CV templates, each crafted to help people present their best selves.",
                imageText: "DDC"
            }
        ];

        // ===== Modal Functions =====
        const projectModal = document.getElementById('projectModal');
        const modalClose = document.getElementById('modalClose');
        let lastFocusedElement = null;

        function openModal(index) {
            const project = projects[index];
            if (!project) return;

            const title = document.getElementById('modalTitle');
            const body = document.getElementById('modalBody');
            lastFocusedElement = document.activeElement;

            title.textContent = project.title;
            body.innerHTML = `
                <div class="modal-image"><span>${project.imageText}</span></div>
                <div class="modal-section">
                    <div class="modal-section-title">Project Overview</div>
                    <p>${project.overview}</p>
                </div>
                <div class="modal-section">
                    <div class="modal-section-title">The Problem</div>
                    <p>${project.problem}</p>
                </div>
                <div class="modal-section">
                    <div class="modal-section-title">The Solution</div>
                    <p>${project.solution}</p>
                </div>
                <div class="modal-section">
                    <div class="modal-section-title">My Role</div>
                    <p>${project.role}</p>
                </div>
                <div class="modal-section">
                    <div class="modal-section-title">Tools & Technologies</div>
                    <div class="modal-tech-tags">
                        ${project.tools.map(t => `<span class="modal-tech-tag">${t}</span>`).join('')}
                    </div>
                </div>
                <div class="modal-section">
                    <div class="modal-section-title">Design Process</div>
                    <p>${project.process}</p>
                </div>
                <div class="modal-section">
                    <div class="modal-section-title">Final Result</div>
                    <p>${project.result}</p>
                </div>
            `;

            projectModal.classList.add('active');
            projectModal.setAttribute('aria-hidden', 'false');
            document.body.style.overflow = 'hidden';
            requestAnimationFrame(() => modalClose.focus());
        }

        function closeModal() {
            if (!projectModal.classList.contains('active')) return;
            projectModal.classList.remove('active');
            projectModal.setAttribute('aria-hidden', 'true');
            document.body.style.overflow = '';
            if (lastFocusedElement) lastFocusedElement.focus();
        }

        // Open project cards with mouse or keyboard.
        document.querySelectorAll('.project-card[data-project-index]').forEach(card => {
            card.addEventListener('click', (event) => {
                if (event.target.closest('a, button')) return;
                openModal(Number(card.dataset.projectIndex));
            });

            card.addEventListener('keydown', (event) => {
                if ((event.key === 'Enter' || event.key === ' ') && !event.target.closest('a, button')) {
                    event.preventDefault();
                    openModal(Number(card.dataset.projectIndex));
                }
            });
        });

        document.querySelectorAll('[data-open-project]').forEach(button => {
            button.addEventListener('click', () => openModal(Number(button.dataset.openProject)));
        });

        modalClose.addEventListener('click', closeModal);
        projectModal.addEventListener('click', (event) => {
            if (event.target === projectModal) closeModal();
        });

        document.addEventListener('keydown', (event) => {
            if (event.key === 'Escape') closeModal();
        });

        // ===== Contact Form Handler (Web3Forms) =====

const form = document.getElementById("contact-form");
const button = document.getElementById("send-button");
const formMessage = document.getElementById("form-message");

form.addEventListener("submit", async function(event) {

    event.preventDefault();

    button.disabled = true;
    button.textContent = "Sending...";
    formMessage.textContent = "";

    const formData = new FormData(form);

    try {

        const response = await fetch(
            "https://api.web3forms.com/submit",
            {
                method: "POST",
                body: formData
            }
        );

        const data = await response.json();

        if (data.success) {

            formMessage.textContent =
                "✓ Message sent successfully!";

            formMessage.style.color = "#7BA7A7";

            form.reset();

        } else {

            formMessage.textContent =
                "Unable to send message. Please try again.";

            formMessage.style.color = "#C9A89A";

        }

    } catch (error) {

        console.error(error);

        formMessage.textContent =
            "Unable to send message. Please try again.";

        formMessage.style.color = "#C9A89A";

    } finally {

        button.disabled = false;
        button.textContent = "Send Message";

    }

});
        

        // ===== Scroll Reveal =====
        const revealElements = document.querySelectorAll('.reveal');
        const revealObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    revealObserver.unobserve(entry.target);
                }
            });
        }, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });

        revealElements.forEach(el => revealObserver.observe(el));

        // ===== Navbar Scroll =====
        const navbar = document.getElementById('navbar');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
            
        });

        // ===== Active Nav Link =====
        const sections = document.querySelectorAll('section[id]');
        window.addEventListener('scroll', () => {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop - 100;
                if (window.scrollY >= sectionTop) {
                    current = section.getAttribute('id');
                }
            });
            document.querySelectorAll('.nav-links a:not(.nav-cta)').forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === '#' + current) {
                    link.classList.add('active');
                }
            });
        });

        // ===== Mobile Menu =====
        const hamburger = document.getElementById('hamburger');
        const mobileMenu = document.getElementById('mobileMenu');

        function setMobileMenu(open) {
            hamburger.classList.toggle('active', open);
            mobileMenu.classList.toggle('active', open);
            hamburger.setAttribute('aria-expanded', String(open));
            hamburger.setAttribute('aria-label', open ? 'Close navigation menu' : 'Open navigation menu');
            document.body.style.overflow = open ? 'hidden' : '';
        }

        hamburger.addEventListener('click', () => {
            setMobileMenu(!mobileMenu.classList.contains('active'));
        });

        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => setMobileMenu(false));
        });

        // ===== Back to Top =====
        const backToTop = document.getElementById('backToTop');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 400) {
                backToTop.classList.add('visible');
            } else {
                backToTop.classList.remove('visible');
            }
        });

        backToTop.addEventListener('click', () => {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        });

        // ===== Smooth scroll for all anchor links =====
        const prefersReducedMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                const href = this.getAttribute('href');
                if (!href || href === '#') return;
                const target = document.querySelector(href);
                if (target) {
                    e.preventDefault();
                    target.scrollIntoView({ behavior: prefersReducedMotion ? 'auto' : 'smooth' });
                }
            });
        });
    </script>
</body>
</html>
