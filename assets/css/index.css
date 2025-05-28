        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-neon: #00ffff;
            --secondary-neon: #ff00ff;
            --accent-neon: #ffff00;
            --bg-dark: #0a0a0f;
            --bg-darker: #050508;
            --glass-bg: rgba(255, 255, 255, 0.05);
            --glass-border: rgba(255, 255, 255, 0.1);
            --text-primary: #ffffff;
            --text-secondary: #b0b0b0;
        }

        body {
            font-family: 'Orbitron', monospace;
            background: var(--bg-dark);
            color: var(--text-primary);
            overflow-x: hidden;
            position: relative;
        }

        /* Animated Background */
        .bg-animation {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                linear-gradient(45deg, transparent 30%, rgba(0, 255, 255, 0.03) 50%, transparent 70%),
                linear-gradient(-45deg, transparent 30%, rgba(255, 0, 255, 0.03) 50%, transparent 70%),
                radial-gradient(circle at 20% 50%, rgba(0, 255, 255, 0.1) 0%, transparent 30%),
                radial-gradient(circle at 80% 20%, rgba(255, 0, 255, 0.1) 0%, transparent 30%),
                linear-gradient(180deg, var(--bg-darker) 0%, var(--bg-dark) 100%);
            animation: backgroundShift 20s ease-in-out infinite;
            z-index: -2;
        }

        @keyframes backgroundShift {
            0%, 100% { transform: rotate(0deg) scale(1); }
            50% { transform: rotate(180deg) scale(1.1); }
        }

        /* Matrix Rain Effect */
        .matrix-rain {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
            overflow: hidden;
        }

        .matrix-column {
            position: absolute;
            top: -100%;
            color: var(--primary-neon);
            font-family: 'Courier New', monospace;
            font-size: 14px;
            opacity: 0.3;
            animation: matrixFall linear infinite;
        }

        @keyframes matrixFall {
            to { transform: translateY(100vh); }
        }

        /* Header */
        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 2rem;
            position: relative;
            z-index: 100;
            background: rgba(10, 10, 15, 0.8);
            backdrop-filter: blur(20px);
            border-bottom: 1px solid var(--glass-border);
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 1rem;
            font-size: 1.5rem;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .logo-icon {
            width: 40px;
            height: 40px;
            background: linear-gradient(45deg, var(--primary-neon), var(--secondary-neon));
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            animation: logoGlow 2s ease-in-out infinite alternate;
            position: relative;
            overflow: hidden;
        }

        .logo-icon::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(255, 255, 255, 0.3), transparent);
            animation: logoSweep 3s linear infinite;
        }

        @keyframes logoGlow {
            from { box-shadow: 0 0 10px var(--primary-neon); }
            to { box-shadow: 0 0 30px var(--primary-neon), 0 0 50px var(--secondary-neon); }
        }

        @keyframes logoSweep {
            0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); }
            100% { transform: translateX(100%) translateY(100%) rotate(45deg); }
        }

        .nav {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav a {
            color: var(--text-secondary);
            text-decoration: none;
            transition: all 0.3s ease;
            position: relative;
            padding: 0.5rem 1rem;
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing: 1px;
        }

        .nav a::before {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            width: 0;
            height: 2px;
            background: linear-gradient(90deg, var(--primary-neon), var(--secondary-neon));
            transition: all 0.3s ease;
            transform: translateX(-50%);
        }

        .nav a:hover {
            color: var(--text-primary);
            text-shadow: 0 0 10px var(--primary-neon);
        }

        .nav a:hover::before {
            width: 100%;
        }

        .contact-btn {
            background: linear-gradient(45deg, var(--primary-neon), var(--secondary-neon));
            padding: 0.8rem 2rem;
            border-radius: 30px;
            color: var(--bg-dark);
            text-decoration: none;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .contact-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.3), transparent);
            transition: left 0.5s ease;
        }

        .contact-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0, 255, 255, 0.5);
        }

        .contact-btn:hover::before {
            left: 100%;
        }

        /* Mobile Menu */
        .mobile-menu-btn {
            display: none;
            flex-direction: column;
            gap: 4px;
            cursor: pointer;
            padding: 0.5rem;
        }

        .mobile-menu-btn span {
            width: 25px;
            height: 3px;
            background: var(--primary-neon);
            border-radius: 2px;
            transition: all 0.3s ease;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 6rem 2rem;
            position: relative;
            min-height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }

        .hero h1 {
            font-size: clamp(2.5rem, 8vw, 5rem);
            font-weight: 900;
            margin-bottom: 2rem;
            text-transform: uppercase;
            letter-spacing: 3px;
            background: linear-gradient(45deg, var(--primary-neon), var(--secondary-neon), var(--accent-neon));
            background-size: 200% 200%;
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradientAnimation 3s ease-in-out infinite;
            position: relative;
        }

        .hero h1::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(45deg, var(--primary-neon), var(--secondary-neon));
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: glitchEffect 4s infinite;
            z-index: -1;
        }

        @keyframes gradientAnimation {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        @keyframes glitchEffect {
            0%, 90%, 100% { transform: translate(0); }
            91% { transform: translate(-2px, 2px); }
            92% { transform: translate(2px, -2px); }
            93% { transform: translate(-2px, 2px); }
        }

        .hero p {
            font-size: clamp(1rem, 3vw, 1.3rem);
            color: var(--text-secondary);
            margin-bottom: 3rem;
            max-width: 700px;
            line-height: 1.6;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .cta-section {
            width: 100%;
            max-width: 600px;
            margin: 2rem 0;
        }

        .animated-prompt-container {
            position: relative;
            margin-bottom: 2rem;
            text-align: center;
        }

        .animated-prompt-text {
            background: var(--glass-bg);
            border: 2px solid var(--glass-border);
            border-radius: 50px;
            padding: 1.5rem 2rem;
            width: 100%;
            max-width: 600px;
            color: var(--text-secondary);
            backdrop-filter: blur(20px);
            font-family: 'Orbitron', monospace;
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin: 0 auto;
            min-height: 60px;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            cursor: default;
        }

        .generate-btn {
            background: linear-gradient(45deg, var(--primary-neon), var(--secondary-neon));
            border: none;
            padding: 1.5rem 3rem;
            border-radius: 50px;
            color: var(--bg-dark);
            font-weight: 900;
            font-family: 'Orbitron', monospace;
            font-size: 1.1rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            cursor: pointer;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            width: 100%;
            max-width: 400px;
        }

        .generate-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.4), transparent);
            transition: left 0.5s ease;
        }

        .generate-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0, 255, 255, 0.4);
        }

        .generate-btn:hover::before {
            left: 100%;
        }

        /* Floating NFT Cards - More Futuristic */
        .nft-card {
            position: absolute;
            width: 100px;
            height: 100px;
            background: var(--glass-bg);
            border: 2px solid var(--glass-border);
            border-radius: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.5rem;
            backdrop-filter: blur(20px);
            cursor: pointer;
            transition: all 0.3s ease;
            animation: float 8s ease-in-out infinite;
            z-index: 1;
        }

        .nft-card::before {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            background: linear-gradient(45deg, var(--primary-neon), var(--secondary-neon), var(--accent-neon));
            border-radius: 22px;
            z-index: -1;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .nft-card:hover {
            transform: scale(1.2) rotate(10deg);
            box-shadow: 0 20px 50px rgba(0, 255, 255, 0.3);
        }

        .nft-card:hover::before {
            opacity: 1;
        }

        .nft-card:nth-child(1) {
            top: 15%;
            left: 5%;
            animation-delay: 0s;
        }

        .nft-card:nth-child(2) {
            top: 25%;
            left: 15%;
            animation-delay: 1s;
        }

        .nft-card:nth-child(3) {
            top: 40%;
            left: 8%;
            animation-delay: 2s;
        }

        .nft-card:nth-child(4) {
            top: 20%;
            right: 10%;
            animation-delay: 0.5s;
        }

        .nft-card:nth-child(5) {
            top: 35%;
            right: 20%;
            animation-delay: 1.5s;
        }

        .nft-card:nth-child(6) {
            top: 50%;
            right: 5%;
            animation-delay: 3s;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            25% { transform: translateY(-30px) rotate(5deg); }
            50% { transform: translateY(-20px) rotate(-3deg); }
            75% { transform: translateY(-25px) rotate(2deg); }
        }

        /* Features Section */
        .features {
            padding: 6rem 2rem;
            max-width: 1400px;
            margin: 0 auto;
            position: relative;
        }

        .features::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                repeating-linear-gradient(
                    90deg,
                    transparent,
                    transparent 98px,
                    rgba(0, 255, 255, 0.03) 100px
                );
            pointer-events: none;
        }

        .section-header {
            text-align: center;
            margin-bottom: 4rem;
        }

        .section-tag {
            color: var(--primary-neon);
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 3px;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .section-title {
            font-size: clamp(2rem, 6vw, 3.5rem);
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 1.5rem;
            background: linear-gradient(45deg, var(--text-primary), var(--primary-neon));
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .section-description {
            color: var(--text-secondary);
            max-width: 700px;
            margin: 0 auto;
            line-height: 1.6;
            font-size: 1.1rem;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 4rem;
        }

        .feature-card {
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            border-radius: 20px;
            padding: 2.5rem;
            backdrop-filter: blur(20px);
            transition: all 0.3s ease;
            cursor: pointer;
            position: relative;
            overflow: hidden;
        }

        .feature-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(0, 255, 255, 0.1), transparent);
            transition: left 0.5s ease;
        }

        .feature-card:hover {
            transform: translateY(-10px);
            border-color: var(--primary-neon);
            box-shadow: 0 20px 50px rgba(0, 255, 255, 0.2);
        }

        .feature-card:hover::before {
            left: 100%;
        }

        .feature-icon {
            width: 80px;
            height: 80px;
            border-radius: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            margin-bottom: 1.5rem;
            position: relative;
            overflow: hidden;
        }

        .feature-card:nth-child(1) .feature-icon {
            background: linear-gradient(45deg, var(--primary-neon), var(--secondary-neon));
        }

        .feature-card:nth-child(2) .feature-icon {
            background: linear-gradient(45deg, var(--secondary-neon), var(--accent-neon));
        }

        .feature-card:nth-child(3) .feature-icon {
            background: linear-gradient(45deg, var(--accent-neon), var(--primary-neon));
        }

        .feature-card:nth-child(4) .feature-icon {
            background: linear-gradient(45deg, var(--primary-neon), var(--accent-neon));
        }

        .feature-card h4 {
            font-size: 1.3rem;
            margin-bottom: 1rem;
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing: 1px;
            color: var(--text-primary);
        }

        .feature-card p {
            color: var(--text-secondary);
            line-height: 1.6;
            font-size: 0.95rem;
        }

        /* FAQ Section */
        .faq {
            padding: 6rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .faq h2 {
            font-size: clamp(2rem, 5vw, 3rem);
            margin-bottom: 3rem;
            text-align: center;
            text-transform: uppercase;
            font-weight: 900;
            letter-spacing: 2px;
            background: linear-gradient(45deg, var(--text-primary), var(--primary-neon));
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .faq-item {
            background: var(--glass-bg);
            border: 1px solid var(--glass-border);
            border-radius: 15px;
            margin-bottom: 1rem;
            overflow: hidden;
            backdrop-filter: blur(20px);
            transition: all 0.3s ease;
        }

        .faq-item:hover {
            border-color: var(--primary-neon);
            box-shadow: 0 10px 30px rgba(0, 255, 255, 0.1);
        }

        .faq-question {
            padding: 1.5rem 2rem;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: all 0.3s ease;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .faq-question:hover {
            color: var(--primary-neon);
        }

        .faq-answer {
            padding: 0 2rem 1.5rem;
            color: var(--text-secondary);
            line-height: 1.6;
            display: none;
            animation: fadeIn 0.3s ease;
        }

        .faq-item.active .faq-answer {
            display: block;
        }

        .faq-toggle {
            font-size: 1.5rem;
            transition: all 0.3s ease;
            color: var(--primary-neon);
        }

        .faq-item.active .faq-toggle {
            transform: rotate(180deg);
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Footer */
        .footer {
            background: linear-gradient(180deg, transparent 0%, var(--bg-darker) 50%);
            padding: 4rem 2rem 2rem;
            border-top: 1px solid var(--glass-border);
            position: relative;
        }

        .footer::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--primary-neon), var(--secondary-neon), transparent);
        }

        .footer-content {
            max-width: 1400px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            margin-bottom: 3rem;
        }

        .footer-section h4 {
            margin-bottom: 1.5rem;
            color: var(--text-primary);
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1px;
            font-size: 1.1rem;
        }

        .footer-section a {
            color: var(--text-secondary);
            text-decoration: none;
            display: block;
            margin-bottom: 0.8rem;
            transition: all 0.3s ease;
            text-transform: uppercase;
            font-size: 0.9rem;
            letter-spacing: 1px;
        }

        .footer-section a:hover {
            color: var(--primary-neon);
            text-shadow: 0 0 10px var(--primary-neon);
            transform: translateX(10px);
        }

        .footer-bottom {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid var(--glass-border);
            color: var(--text-secondary);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .newsletter {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .newsletter input {
            flex: 1;
            padding: 1rem;
            border: 1px solid var(--glass-border);
            border-radius: 10px;
            background: var(--glass-bg);
            color: var(--text-primary);
            backdrop-filter: blur(20px);
            font-family: 'Orbitron', monospace;
        }

        .newsletter input:focus {
            outline: none;
            border-color: var(--primary-neon);
            box-shadow: 0 0 20px rgba(0, 255, 255, 0.3);
        }

        .newsletter button {
            background: linear-gradient(45deg, var(--primary-neon), var(--secondary-neon));
            border: none;
            padding: 1rem 1.5rem;
            border-radius: 10px;
            color: var(--bg-dark);
            cursor: pointer;
            font-family: 'Orbitron', monospace;
            font-weight: 700;
            text-transform: uppercase;
            transition: all 0.3s ease;
        }

        .newsletter button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0, 255, 255, 0.3);
        }

        @media (max-width: 1024px) {
            .features-grid {
                grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            }
            
            .nft-card {
                width: 80px;
                height: 80px;
                font-size: 2rem;
            }
        }

        @media (max-width: 768px) {
            .header {
                padding: 1rem;
            }
            
            .nav {
                display: none;
            }
            
            .mobile-menu-btn {
                display: flex;
            }
            
            .hero {
                padding: 4rem 1rem;
            }
            
            .hero h1 {
                font-size: 2.5rem;
                letter-spacing: 1px;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .features, .faq {
                padding: 4rem 1rem;
            }
            
            .features-grid {
                grid-template-columns: 1fr;
                gap: 1.5rem;
            }
            
            .feature-card {
                padding: 2rem;
            }
            
            .nft-card {
                width: 60px;
                height: 60px;
                font-size: 1.5rem;
            }
            
            .footer-content {
                grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
                gap: 2rem;
            }
            
            .newsletter {
                flex-direction: column;
            }
            
            .contact-btn {
                padding: 0.6rem 1.5rem;
                font-size: 0.9rem;
            }
            
            .animated-prompt-text {
                padding: 1rem;
                font-size: 0.9rem;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .cta-section {
                max-width: 100%;
            }
            
            .generate-btn {
                padding: 1rem 2rem;
                font-size: 1rem;
            }
            
            .faq-question {
                padding: 1rem;
                font-size: 0.9rem;
            }
            
            .faq-answer {
                padding: 0 1rem 1rem;
                font-size: 0.9rem;
            }
        }

        /* Accessibility */
        @media (prefers-reduced-motion: reduce) {
            *, *::before, *::after {
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
                transition-duration: 0.01ms !important;
            }
        }
   