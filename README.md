<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Studio do Sorriso - Odontologia | Campo Grande MS</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Poppins:wght@300;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    
    <style>
        :root {
            --navy-deep: #0B2330;
            --navy-light: #1F4B66;
            --gold: #D19A2B;
            --white: #FFFFFF;
            --gray-light: #F5F7F8;
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--navy-deep);
            color: var(--white);
            line-height: 1.6;
            /* Textura Chevron sutil */
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='60' height='30' viewBox='0 0 60 30'%3E%3Cpath d='M0 30L30 0l30 30v-1L30 29 0 29z' fill='%23ffffff' fill-opacity='0.03'/%3E%3C/svg%3E");
        }

        /* Header */
        header {
            background: rgba(11, 35, 48, 0.95);
            padding: 1rem 5%;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid rgba(209, 154, 43, 0.2);
        }

        .logo {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--gold);
            text-decoration: none;
        }

        .btn-header {
            background: var(--gold);
            color: var(--navy-deep);
            padding: 0.6rem 1.2rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            transition: var(--transition);
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(11, 35, 48, 0.7), rgba(11, 35, 48, 0.7)), url('https://images.unsplash.com/photo-1629909613654-28e377c37b09?auto=format&fit=crop&q=80&w=2070') center/cover;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 0 5%;
            margin-top: 60px;
        }

        .hero-content h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 3rem;
            margin-bottom: 1rem;
            color: var(--white);
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        /* Selo Google */
        .google-badge {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(5px);
            padding: 1rem;
            border-radius: 10px;
            display: inline-block;
            margin-bottom: 2rem;
            border: 1px solid var(--gold);
        }

        .google-badge span { color: var(--gold); font-size: 1.2rem; }

        /* Grid Especialidades */
        .specialties {
            padding: 5rem 5%;
            background: var(--gray-light);
            color: var(--navy-deep);
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-family: 'Montserrat', sans-serif;
            color: var(--navy-deep);
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .card {
            background: var(--white);
            padding: 2.5rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            transition: var(--transition);
            border-bottom: 4px solid transparent;
        }

        .card:hover {
            transform: translateY(-10px);
            border-bottom: 4px solid var(--gold);
        }

        .card i {
            font-size: 2.5rem;
            color: var(--gold);
            margin-bottom: 1.5rem;
        }

        /* Diferenciais Parallax */
        .parallax {
            padding: 6rem 5%;
            background: linear-gradient(rgba(11, 35, 48, 0.85), rgba(11, 35, 48, 0.85)), url('https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?auto=format&fit=crop&q=80&w=2070') fixed center/cover;
            text-align: center;
        }

        /* Banner Coworking */
        .coworking-banner {
            background: var(--gold);
            color: var(--navy-deep);
            padding: 1rem;
            text-align: center;
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        /* Botão WhatsApp */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: #25d366;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 30px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            z-index: 1000;
            transition: var(--transition);
        }

        .whatsapp-float:hover { transform: scale(1.1); }

        /* Footer */
        footer {
            padding: 4rem 5%;
            background: #05121a;
            border-top: 1px solid rgba(209, 154, 43, 0.3);
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 3rem;
        }

        /* Responsividade */
        @media (max-width: 768px) {
            .hero-content h1 { font-size: 2rem; }
            .hero { height: auto; padding: 10rem 5%; }
        }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">STUDIO DO SORRISO</a>
        <a href="https://wa.me/5567984158415" class="btn-header">AGENDE ONLINE</a>
    </header>

    <section class="hero">
        <div class="hero-content">
            <div class="google-badge">
                <span>★★★★★</span>
                <p>+5.067 avaliações no Google</p>
            </div>
            <h1>Referência em Odontologia Digital no melhor endereço de MS</h1>
            <p>Dr. Jorge Pereira (CRO-MS 1889) e equipe completa para cuidar do seu sorriso no Edifício The Place.</p>
            <a href="https://wa.me/5567984158415" class="btn-header" style="padding: 1.2rem 2.5rem; font-size: 1.1rem;">GARANTIR MEU HORÁRIO</a>
        </div>
    </section>
<section class="sobre">
    <div class="sobre-container">
        <img src="link de imagem aqui" alt="Dr. Jorge Pereira em atendimento" class="img-atendimento">
        <div class="sobre-texto">
            <h2>Excelência e Humanização</h2>
            <p>O Dr. Jorge Pereira (CRO-MS 1889) lidera uma equipe focada em tecnologia e bem-estar.</p>
        </div>
    </div>
</section>
    <div class="coworking-banner">
        Novo: Espaço de Coworking para Profissionais da Saúde no The Place
    </div>

    <section class="specialties">
        <h2 class="section-title">Nossas Especialidades</h2>
        <div class="grid">
            <div class="card">
                <i class="fas fa-tooth"></i>
                <h3>Lentes</h3>
                <p>Facetas e lentes de contato dental para transformar seu sorriso com naturalidade.</p>
            </div>
            <div class="card">
                <i class="fas fa-implant"></i>
                <h3>Implantes</h3>
                <p>Reabilitação funcional e estética com tecnologia suíça e segurança total.</p>
            </div>
            <div class="card">
                <i class="fas fa-align-center"></i>
                <h3>Ortodontia</h3>
                <p>Aparelhos estéticos e personalizados que refletem a sua paixão e estilo.</p>
            </div>
            <div class="card">
                <i class="fas fa-microscope"></i>
                <h3>Endodontia</h3>
                <p>Tratamentos de canal precisos com uso de microscopia e odontologia digital.</p>
            </div>
        </div>
    </section>

    <section class="parallax">
        <h2 style="font-family: 'Montserrat'; font-size: 2.5rem; margin-bottom: 1.5rem;">Tecnologia no 17º Andar</h2>
        <p style="max-width: 700px; margin: 0 auto 2rem;">Tratamentos personalizados com a melhor vista de Campo Grande. Equipamentos de última geração para um diagnóstico rápido e indolor.</p>
        <p><strong>"Tratamentos que refletem a sua paixão."</strong></p>
    </section>

    <footer>
        <div class="footer-grid">
            <div>
                <h4 style="color: var(--gold); margin-bottom: 1rem;">CONTATO</h4>
                <p><i class="fas fa-phone"></i> (67) 98415-8415</p>
                <p><i class="fas fa-clock"></i> Aberto até às 18:00</p>
                <p><i class="fas fa- ambulance"></i> Emergência 24 Horas</p>
            </div>
            <div>
                <h4 style="color: var(--gold); margin-bottom: 1rem;">LOCALIZAÇÃO</h4>
                <p>The Place, Torre 2 - Sala 1705</p>
                <p>Av. Afonso Pena, 4785 - Santa Fe</p>
                <p>Campo Grande - MS, 79031-010</p>
            </div>
            <div>
                <h4 style="color: var(--gold); margin-bottom: 1rem;">REDES SOCIAIS</h4>
                <div style="font-size: 1.5rem; display: flex; gap: 15px;">
                    <a href="#" style="color: white;"><i class="fab fa-instagram"></i></a>
                    <a href="#" style="color: white;"><i class="fab fa-facebook"></i></a>
                    <a href="#" style="color: white;"><i class="fab fa-google"></i></a>
                </div>
            </div>
        </div>
        <div style="text-align: center; margin-top: 4rem; font-size: 0.8rem; opacity: 0.6;">
            © 2026 Studio do Sorriso - Odontologia. Todos os direitos reservados. Dr. Jorge Pereira | CRO-MS 1889
        </div>
    </footer>

    <a href="https://wa.me/5567984158415" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

</body>
</html>
