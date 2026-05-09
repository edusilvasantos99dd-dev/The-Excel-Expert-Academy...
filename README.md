<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
<meta name="description" content="Excel Expert Academy - Curso de Excel profissional, planos acessíveis, certificado, mentoria ao vivo e suporte 24h.">
<title>Excel Expert Academy | Curso de Excel Profissional</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;400;500;600;700;800&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
<style>
* { margin: 0; padding: 0; box-sizing: border-box; }
body {
    font-family: 'Inter', -apple-system, sans-serif;
    background: #0a0c12;
    color: #edf2ff;
    line-height: 1.5;
    scroll-behavior: smooth;
}
/* Fundo com grid e brilho */
body::before {
    content: "";
    position: fixed;
    inset: 0;
    background-image: 
        repeating-linear-gradient(0deg, rgba(46,204,113,0.03) 1px, transparent 1px, transparent 40px),
        repeating-linear-gradient(90deg, rgba(46,204,113,0.03) 1px, transparent 1px, transparent 40px);
    pointer-events: none;
    z-index: 0;
}
body::after {
    content: "";
    position: fixed;
    inset: 0;
    background: radial-gradient(circle at 30% 50%, rgba(46,204,113,0.07), transparent 70%);
    pointer-events: none;
    z-index: 0;
    animation: pulseGlow 8s infinite alternate;
}
@keyframes pulseGlow {
    0% { opacity: 0.3; }
    100% { opacity: 0.8; }
}
.sticky-header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background: rgba(10,12,18,0.85);
    backdrop-filter: blur(16px);
    z-index: 100;
    padding: 0.8rem 2rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid rgba(46,204,113,0.2);
}
.logo {
    font-size: 1.4rem;
    font-weight: 700;
    background: linear-gradient(135deg, #fff, #2ecc71);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
}
.nav-links a {
    color: #cbd5e6;
    text-decoration: none;
    margin-left: 2rem;
    font-weight: 500;
    transition: 0.2s;
}
.nav-links a:hover { color: #2ecc71; }
.hero {
    min-height: 90vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 100px 24px 60px;
    background: radial-gradient(circle at 70% 20%, rgba(46,204,113,0.1), rgba(10,12,18,0.96)),
                linear-gradient(125deg, #0c1122, #03050b);
    position: relative;
    z-index: 1;
}
.hero h1 {
    font-size: 3.8rem;
    background: linear-gradient(135deg, #FFFFFF, #2ecc71, #1abc9c);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
    margin-bottom: 1rem;
    font-weight: 800;
}
.hero .tagline {
    font-size: 1.3rem;
    margin: 1rem auto;
    color: #cbd5e6;
    max-width: 750px;
}
.counter-section {
    display: flex;
    justify-content: center;
    gap: 3rem;
    margin: 2rem 0;
    flex-wrap: wrap;
}
.counter-number {
    font-size: 2.5rem;
    font-weight: 800;
    color: #2ecc71;
}
.counter-label {
    font-size: 0.9rem;
    color: #8ba3b9;
}
.section {
    padding: 80px 24px;
    max-width: 1400px;
    margin: 0 auto;
    position: relative;
    z-index: 2;
}
.plan-card {
    background: rgba(18,25,45,0.8);
    backdrop-filter: blur(12px);
    border-radius: 2rem;
    padding: 2rem 1.8rem;
    transition: transform 0.3s, box-shadow 0.3s;
    border: 1px solid rgba(46,204,113,0.35);
}
.plan-card:hover {
    transform: translateY(-10px);
    border-color: #2ecc71;
    box-shadow: 0 25px 45px -12px rgba(46,204,113,0.3);
}
.plan-price {
    font-size: 2.8rem;
    font-weight: 800;
    color: #2ecc71;
    margin: 1rem 0;
}
.btn-primary {
    background: linear-gradient(105deg, #1e6b3c, #2ecc71);
    border: none;
    font-weight: 600;
    padding: 0.9rem 2rem;
    border-radius: 60px;
    font-size: 1rem;
    color: white;
    cursor: pointer;
    transition: all 0.2s;
    box-shadow: 0 6px 14px rgba(46,204,113,0.3);
}
.btn-primary:hover { transform: scale(1.02); }
.btn-outline {
    background: transparent;
    border: 1.5px solid #2ecc71;
    color: #2ecc71;
    padding: 0.7rem 1.5rem;
    border-radius: 60px;
    font-weight: 600;
    cursor: pointer;
}
.form-container {
    background: rgba(15,23,42,0.75);
    backdrop-filter: blur(20px);
    border-radius: 2rem;
    padding: 2rem;
    border: 1px solid rgba(46,204,113,0.4);
    max-width: 950px;
    margin: 0 auto;
}
.input-field {
    width: 100%;
    padding: 14px 18px;
    border-radius: 60px;
    border: 1px solid #2d3a4e;
    background: #0f172a;
    color: white;
    font-size: 0.95rem;
    transition: 0.2s;
}
.input-field:focus {
    outline: none;
    border-color: #2ecc71;
    box-shadow: 0 0 0 3px rgba(46,204,113,0.2);
}
.payment-methods {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
    justify-content: center;
    margin: 2rem 0;
}
.pay-card {
    background: #0f172a;
    border-radius: 3rem;
    padding: 12px 28px;
    font-weight: 600;
    cursor: pointer;
    border: 1px solid #2ecc71;
    transition: all 0.2s;
}
.pay-card:hover, .pay-card.active {
    background: #2ecc71;
    color: #070b17;
    transform: scale(1.03);
}
.pix-area-transition {
    transition: all 0.4s cubic-bezier(0.2,0.9,0.4,1.1);
    opacity: 0;
    transform: translateY(15px) scale(0.98);
    display: none;
}
.pix-area-transition.show {
    opacity: 1;
    transform: translateY(0) scale(1);
    display: block;
}
.qr-container {
    text-align: center;
    background: white;
    border-radius: 28px;
    padding: 1.5rem;
    margin: 1rem 0;
    color: #0f172a;
}
.chave-pix {
    background: #eef2ff;
    padding: 14px;
    border-radius: 24px;
    margin: 15px 0;
}
.testimonials {
    background: rgba(15,23,42,0.5);
    backdrop-filter: blur(10px);
    border-radius: 2rem;
    padding: 2rem;
    margin: 2rem auto;
}
.testimonial-card {
    background: rgba(10,12,18,0.7);
    border-radius: 1.5rem;
    padding: 1.5rem;
    border: 1px solid rgba(46,204,113,0.2);
    transition: 0.3s;
}
.testimonial-card:hover { border-color: #2ecc71; transform: translateY(-4px); }
.security-badges {
    display: flex;
    justify-content: center;
    gap: 2rem;
    margin: 2rem 0;
    flex-wrap: wrap;
}
.badge {
    background: rgba(0,0,0,0.5);
    backdrop-filter: blur(4px);
    padding: 0.5rem 1.2rem;
    border-radius: 40px;
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    border: 1px solid rgba(46,204,113,0.3);
}
.wpp-minimal {
    position: fixed;
    bottom: 28px;
    left: 28px;
    background: #25D366;
    width: 52px;
    height: 52px;
    border-radius: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    z-index: 99;
    text-decoration: none;
    color: white;
    font-size: 28px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    transition: 0.2s;
}
.wpp-minimal:hover { transform: scale(1.05); background: #20b859; }
.ia-fab {
    position: fixed;
    bottom: 28px;
    right: 28px;
    z-index: 1000;
}
.ia-btn {
    background: linear-gradient(135deg, #1e6b3c, #2ecc71);
    width: 52px;
    height: 52px;
    border-radius: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    border: none;
    font-size: 26px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    transition: 0.2s;
}
.ia-btn:hover { transform: scale(1.05); }
.ia-chat-window {
    position: fixed;
    bottom: 95px;
    right: 28px;
    width: 360px;
    background: #101826;
    border-radius: 28px;
    backdrop-filter: blur(12px);
    border: 1px solid #2ecc71;
    display: none;
    flex-direction: column;
    overflow: hidden;
    z-index: 1001;
}
.ia-chat-window.open { display: flex; }
.ia-header {
    background: #1e2a3a;
    padding: 16px;
    font-weight: 600;
    display: flex;
    justify-content: space-between;
    cursor: pointer;
    border-bottom: 1px solid #2ecc71;
}
.ia-messages {
    height: 320px;
    overflow-y: auto;
    padding: 12px;
    display: flex;
    flex-direction: column;
    gap: 8px;
    background: #0c1220;
}
.ia-input-area {
    display: flex;
    padding: 12px;
    background: #0a0f1c;
    gap: 8px;
}
.message-user {
    background: #2ecc71;
    color: #000;
    align-self: flex-end;
    padding: 8px 14px;
    border-radius: 20px;
    max-width: 85%;
}
.message-bot {
    background: #1e2a3a;
    align-self: flex-start;
    padding: 8px 14px;
    border-radius: 20px;
    max-width: 85%;
}
.suggestion-btn {
    background: #1e2a3a;
    border: 1px solid #2ecc71;
    border-radius: 30px;
    padding: 4px 14px;
    font-size: 0.75rem;
    cursor: pointer;
    margin: 3px;
}
.modal-dashboard {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.96);
    backdrop-filter: blur(12px);
    z-index: 2000;
    display: flex;
    align-items: center;
    justify-content: center;
}
.dashboard-content {
    background: linear-gradient(135deg, #0b1120, #121b2d);
    max-width: 700px;
    width: 90%;
    border-radius: 2rem;
    padding: 2rem;
    border: 2px solid #2ecc71;
    position: relative;
    animation: fadeUp 0.3s;
}
@keyframes fadeUp {
    from { opacity: 0; transform: translateY(20px);}
    to { opacity: 1; transform: translateY(0);}
}
.toast {
    position: fixed;
    bottom: 30px;
    left: 50%;
    transform: translateX(-50%);
    background: #1a2a36;
    color: white;
    padding: 12px 28px;
    border-radius: 60px;
    z-index: 3000;
    border-left: 5px solid #2ecc71;
    animation: fadeSlide 0.3s;
    font-weight: 500;
}
@keyframes fadeSlide {
    from { opacity: 0; transform: translateX(-50%) translateY(20px);}
    to { opacity: 1; transform: translateX(-50%) translateY(0);}
}
.loading-overlay {
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.94);
    z-index: 5000;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}
.spinner {
    width: 48px;
    height: 48px;
    border: 4px solid #2ecc7133;
    border-top-color: #2ecc71;
    border-radius: 50%;
    animation: spin 0.6s linear infinite;
}
@keyframes spin { to { transform: rotate(360deg); } }
.reveal {
    opacity: 0;
    transform: translateY(30px);
    transition: 0.6s ease;
}
.reveal.active {
    opacity: 1;
    transform: translateY(0);
}
#backToTop {
    position: fixed;
    bottom: 100px;
    right: 28px;
    background: #2ecc71;
    color: #0a0c12;
    width: 44px;
    height: 44px;
    border-radius: 30px;
    display: none;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    z-index: 99;
    border: none;
    transition: 0.2s;
}
#backToTop:hover { transform: scale(1.05); }
.plans-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
}
.popular {
    position: relative;
}
.popular-badge {
    position: absolute;
    top: -12px;
    right: 20px;
    background: #e74c3c;
    padding: 4px 14px;
    border-radius: 40px;
    font-size: 0.8rem;
    font-weight: bold;
}
@media (max-width: 768px) {
    .hero h1 { font-size: 2.4rem; }
    .hero .tagline { font-size: 1rem; }
    .sticky-header { padding: 0.5rem 1rem; }
    .nav-links a { margin-left: 1rem; font-size: 0.9rem; }
    .plan-card { width: 100%; max-width: 360px; }
    .ia-chat-window { width: 300px; right: 10px; bottom: 85px; }
}
</style>
</head>
<body>

<header class="sticky-header">
    <div class="logo">📊 Excel Expert Academy</div>
    <div class="nav-links">
        <a href="#plans-section">Planos</a>
        <a href="#checkout-section">Matrícula</a>
    </div>
</header>

<section class="hero">
    <div>
        <h1 class="reveal">📊 Excel Expert Academy</h1>
        <p class="tagline reveal">Transforme dados em decisões. Acelere sua carreira. Domine o Excel como um líder.</p>
        <div class="counter-section reveal">
            <div class="counter-item"><div class="counter-number" id="alunosCount">0</div><div class="counter-label">Alunos</div></div>
            <div class="counter-item"><div class="counter-number" id="certificadosCount">0</div><div class="counter-label">Certificados</div></div>
            <div class="counter-item"><div class="counter-number" id="aulasCount">0</div><div class="counter-label">Aulas</div></div>
        </div>
        <button class="btn-primary reveal" id="verPlanosBtn" style="margin-top:2rem;">🚀 VER PLANOS</button>
    </div>
</section>

<div class="section" id="plans-section">
    <h2 style="text-align:center; font-size:2rem; margin-bottom:2rem;">🎯 Escolha o seu plano</h2>
    <div class="plans-container">
        <div class="plan-card reveal">
            <div class="plan-name" style="font-size:1.6rem; font-weight:700;">📘 Básico</div>
            <div class="plan-price">R$ 49,90</div>
            <ul style="list-style:none; margin:1rem 0; text-align:left;"><li>✓ Fundamentos + Fórmulas essenciais</li><li>✓ Certificado básico</li><li>✓ Material em PDF</li><li>✓ Suporte por e-mail</li></ul>
            <button class="btn-primary" style="width:100%;" onclick="selectPlan('Básico', 49.90)">ESCOLHER PLANO</button>
        </div>
        <div class="plan-card popular reveal">
            <div class="popular-badge">🔥 MAIS VENDIDO</div>
            <div class="plan-name" style="font-size:1.6rem;">🚀 Profissional</div>
            <div class="plan-price">R$ 110,80</div>
            <ul style="list-style:none; margin:1rem 0; text-align:left;"><li>✓ Tudo do Básico</li><li>✓ Tabelas Dinâmicas + Dashboards</li><li>✓ Power Query</li><li>✓ Certificado Profissional</li></ul>
            <button class="btn-primary" style="width:100%;" onclick="selectPlan('Profissional', 110.80)">ESCOLHER PLANO</button>
        </div>
        <div class="plan-card reveal">
            <div class="plan-name">🏆 Premium</div>
            <div class="plan-price">R$ 260,40</div>
            <ul style="list-style:none; margin:1rem 0; text-align:left;"><li>✓ Tudo do Profissional</li><li>✓ VBA + Macros (Automação)</li><li>✓ Power BI + Mentoria ao vivo</li><li>✓ Grupo VIP + Certificado Premium</li></ul>
            <button class="btn-primary" style="width:100%;" onclick="selectPlan('Premium', 260.40)">ESCOLHER PLANO</button>
        </div>
    </div>
</div>

<div class="section testimonials reveal">
    <h2 style="text-align:center; margin-bottom:2rem;">💬 O que nossos alunos dizem</h2>
    <div style="display:flex; flex-wrap:wrap; gap:1.5rem; justify-content:center;">
        <div class="testimonial-card" style="max-width:300px;"><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><p style="margin:1rem 0;">"Saí do zero ao avançado em 3 meses. Hoje sou analista de dados!"</p><strong>— Ana C.</strong></div>
        <div class="testimonial-card" style="max-width:300px;"><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><p>"Material excelente e suporte rápido. Recomendo a todos!"</p><strong>— Ricardo M.</strong></div>
        <div class="testimonial-card" style="max-width:300px;"><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><i class="fas fa-star" style="color:#f1c40f;"></i><p>"A mentoria ao vivo me ajudou a conseguir uma promoção!"</p><strong>— Juliana S.</strong></div>
    </div>
</div>

<div class="security-badges reveal">
    <div class="badge"><i class="fas fa-lock"></i> Pagamento 100% seguro</div>
    <div class="badge"><i class="fas fa-certificate"></i> Certificado reconhecido</div>
    <div class="badge"><i class="fas fa-money-bill-wave"></i> Garantia de 7 dias</div>
    <div class="badge"><i class="fas fa-headset"></i> Suporte 24h</div>
</div>

<div class="section" id="checkout-section">
    <h2 class="reveal" id="checkoutTitle" style="text-align:center;">💳 Finalize sua Matrícula</h2>
    <div class="form-container">
        <div style="display:flex; gap:12px; justify-content:center; margin-bottom:30px;">
            <button id="btnTabPagamento" class="btn-primary" style="background:#217346;">🛒 Pagamento</button>
            <button id="btnTabLogin" class="btn-outline">📚 Já sou aluno</button>
        </div>
        <div id="painelCompra">
            <div style="background:#1e3a2f; padding:12px; border-radius:60px; text-align:center; margin-bottom:20px;" id="selectedPlanDisplay">⚡ Nenhum plano selecionado</div>
            <div style="display:grid; gap:1rem;">
                <input type="text" id="nomeCompleto" class="input-field" placeholder="Nome completo *">
                <input type="email" id="emailCompra" class="input-field" placeholder="E-mail *">
                <input type="text" id="cpf" class="input-field" placeholder="CPF *" maxlength="14">
                <input type="date" id="dataNascimento" class="input-field">
                <input type="tel" id="telefone" class="input-field" placeholder="WhatsApp com DDD *">
                <input type="password" id="senhaCadastro" class="input-field" placeholder="Crie uma senha * (mínimo 6 caracteres)">
            </div>
            <h3 style="margin: 1.5rem 0 0.5rem;">💳 Forma de Pagamento</h3>
            <div class="payment-methods">
                <div class="pay-card" onclick="showPaymentMethod('pix')">📱 PIX</div>
                <div class="pay-card" onclick="showPaymentMethod('card')">💳 Cartão de Crédito</div>
                <div class="pay-card" onclick="showPaymentMethod('boleto')">📄 Boleto</div>
            </div>
            <div id="pixArea" class="pix-area-transition"></div>
            <div id="cardArea" style="display:none;">
                <div style="border:1px solid #2ecc71; border-radius:24px; padding:1.5rem; margin-top:1rem;">
                    <input type="text" id="cardNumber" class="input-field" placeholder="Número do Cartão" maxlength="19">
                    <input type="text" id="cardName" class="input-field" placeholder="Nome no Cartão">
                    <div style="display:flex; gap:12px; margin-top:12px;">
                        <input type="text" id="cardValidade" class="input-field" placeholder="MM/AA" maxlength="5">
                        <input type="text" id="cardCvv" class="input-field" placeholder="CVV" maxlength="4">
                    </div>
                    <select id="cardParcelas" class="input-field" style="margin-top:12px;"></select>
                    <button class="btn-primary" style="width:100%; margin-top:20px;" onclick="processarPagamentoCartao()">💳 Pagar com Cartão</button>
                </div>
            </div>
            <div id="boletoArea" style="display:none;">
                <div class="qr-container" style="background:#0f172a; color:white;">
                    <p>📄 Boleto Bancário</p>
                    <div style="background:#0a0f1c; padding:1rem; border-radius:20px;">
                        <p style="word-break:break-all;">34191.79001 01043.210047 21020.390008 1 92780000026040</p>
                        <button class="btn-primary" onclick="gerarBoleto()">📄 Gerar Boleto</button>
                    </div>
                </div>
            </div>
        </div>
        <div id="painelLogin" style="display:none;">
            <h3>🔐 Acesso com verificação</h3>
            <input type="email" id="loginEmail" class="input-field" placeholder="E-mail cadastrado">
            <input type="password" id="loginSenha" class="input-field" placeholder="Senha" style="margin-top:12px;">
            <input type="text" id="loginCpf" class="input-field" placeholder="CPF para verificação" maxlength="14">
            <button class="btn-primary" style="width:100%; margin-top:20px;" onclick="fazerLoginComCpf()">Entrar</button>
            <a onclick="showForgotPassword()" style="display:block; text-align:center; margin-top:1rem; cursor:pointer; color:#2ecc71;">🔑 Esqueci minha senha</a>
        </div>
    </div>
</div>

<div class="ia-fab"><div class="ia-btn" id="iaFabBtn">🤖</div><div class="ia-chat-window" id="iaChatWindow"><div class="ia-header"><span>🤖 Assistente Excel Expert</span><span style="cursor:pointer;" id="closeChatBtn">✕</span></div><div class="ia-messages" id="iaMessages"><div class="message-bot">Olá! Sou seu assistente. Posso ajudar com planos, preços e pagamentos.</div><div><button class="suggestion-btn" onclick="sendSuggestion('Quanto custa?')">💰 Preços</button><button class="suggestion-btn" onclick="sendSuggestion('Diferença de planos')">📊 Diferença</button><button class="suggestion-btn" onclick="sendSuggestion('Aceita PIX?')">💳 Pagamento</button></div></div><div class="ia-input-area"><input type="text" id="iaQuestion" placeholder="Digite sua dúvida..." class="input-field" style="flex:1; margin:0;"><button class="btn-primary" style="padding:0 20px;" onclick="askIA()">Enviar</button></div></div></div>

<a href="https://wa.me/5517997729758" target="_blank" class="wpp-minimal">💬</a>
<button id="backToTop"><i class="fas fa-arrow-up"></i></button>
<footer style="text-align:center; padding:2rem; background:#03050a;"><p>© 2025 Excel Expert Academy - Todos os direitos reservados | <a href="#" style="color:#2ecc71;">Termos de uso</a> | <a href="#" style="color:#2ecc71;">Privacidade</a></p></footer>

<script>
// ==================== PAYLOADS PIX EXATOS ====================
const PAYLOADS_PIX = {
    basico: "00020101021126330014br.gov.bcb.pix011123756167828520400005303986540549.905802BR5920EDUARDO S DOS SANTOS6013SAO JOSE DO R62070503***6304AA1C",
    profissional: "00020101021126330014br.gov.bcb.pix0111237561678285204000053039865406110.805802BR5920EDUARDO S DOS SANTOS6013SAO JOSE DO R62070503***6304C1F0",
    premium: "00020101021126330014br.gov.bcb.pix0111237561678285204000053039865406260.405802BR5920EDUARDO S DOS SANTOS6013SAO JOSE DO R62070503***6304366C"
};

const LINKS_PDF = {
    basico: "https://drive.google.com/file/d/1MyJ-u9ImBrPEaZRf5x8qYjJT54XhiUhg/view?usp=sharing",
    profissional: "https://drive.google.com/file/d/1fKn4qrDwwbR2msf42lctDFIxO1pm7THH/view?usp=sharing",
    premium: "https://drive.google.com/file/d/1SoqR27z2sMsiQqjPvHQ2Ijx-dN9FdZQh/view?usp=sharing"
};

let selectedPlanName = "", selectedPlanPrice = 0;
let usuariosCadastrados = [];

// ==================== FUNÇÕES AUXILIARES ====================
function loadUsers() {
    const stored = localStorage.getItem("excel_academy_users_final");
    if(stored) usuariosCadastrados = JSON.parse(stored);
    else {
        usuariosCadastrados = [{ id: Date.now(), email: "demo@excel.com", nome: "Aluno Demo", cpf: "12345678901", dataNascimento: "1990-01-01", plano: "Premium", senhaHash: btoa("123456"+"salt"), dataCompra: new Date().toISOString() }];
        saveUsers();
    }
}
function saveUsers() { localStorage.setItem("excel_academy_users_final", JSON.stringify(usuariosCadastrados)); }
function hashPassword(pw) { return btoa(pw + "salt"); }
function verifyPassword(pw, hash) { return hashPassword(pw) === hash; }

function validarCPF(cpf) {
    cpf = cpf.replace(/\D/g,'');
    if(cpf.length!==11) return false;
    if(/^(\d)\1{10}$/.test(cpf)) return false;
    let sum=0, rest;
    for(let i=1;i<=9;i++) sum += parseInt(cpf[i-1])*(11-i);
    rest = (sum*10)%11; if(rest===10||rest===11) rest=0;
    if(rest!==parseInt(cpf[9])) return false;
    sum=0;
    for(let i=1;i<=10;i++) sum += parseInt(cpf[i-1])*(12-i);
    rest = (sum*10)%11; if(rest===10||rest===11) rest=0;
    if(rest!==parseInt(cpf[10])) return false;
    return true;
}
function calcularIdade(dataNasc) {
    const hoje = new Date(), nasc = new Date(dataNasc);
    let idade = hoje.getFullYear() - nasc.getFullYear();
    const m = hoje.getMonth() - nasc.getMonth();
    if(m<0 || (m===0 && hoje.getDate()<nasc.getDate())) idade--;
    return idade;
}
function validarCartao(numero, validade, cvv) {
    const num = numero.replace(/\s/g,'');
    if(num.length < 13 || num.length > 19) return false;
    let sum = 0, alternate = false;
    for(let i=num.length-1; i>=0; i--) {
        let n = parseInt(num.charAt(i));
        if(alternate) { n *= 2; if(n>9) n = (n%10)+1; }
        sum += n;
        alternate = !alternate;
    }
    if(sum%10 !== 0) return false;
    if(!validade.match(/^\d{2}\/\d{2}$/)) return false;
    const [mes, ano] = validade.split('/');
    const now = new Date();
    const currentYear = now.getFullYear() % 100;
    const currentMonth = now.getMonth() + 1;
    const anoNum = parseInt(ano,10);
    const mesNum = parseInt(mes,10);
    if(anoNum < currentYear || (anoNum === currentYear && mesNum < currentMonth)) return false;
    if(cvv.length < 3 || cvv.length > 4) return false;
    return true;
}
function atualizarParcelas() {
    let sel = document.getElementById("cardParcelas");
    if(sel && selectedPlanPrice) {
        sel.innerHTML = '';
        for(let i=1;i<=12;i++) {
            let val = (selectedPlanPrice / i).toFixed(2);
            sel.innerHTML += `<option value="${i}">${i}x de R$ ${val}</option>`;
        }
    }
}
function selectPlan(plan, price) {
    selectedPlanName = plan;
    selectedPlanPrice = price;
    document.getElementById("selectedPlanDisplay").innerHTML = `✅ Plano selecionado: <strong>${plan}</strong> - R$ ${price.toFixed(2)}`;
    document.getElementById("checkoutTitle").innerHTML = `💳 Finalizar Compra - ${plan}`;
    document.getElementById("checkout-section").scrollIntoView({ behavior: "smooth" });
    atualizarParcelas();
    if(document.getElementById("pixArea").classList.contains('show')) gerarConteudoPix();
}
function gerarConteudoPix() {
    if(!selectedPlanName) return;
    let key = selectedPlanName === 'Básico' ? 'basico' : (selectedPlanName === 'Profissional' ? 'profissional' : 'premium');
    const payload = PAYLOADS_PIX[key];
    const qrUrl = `https://api.qrserver.com/v1/create-qr-code/?size=260x260&data=${encodeURIComponent(payload)}`;
    const valorStr = selectedPlanPrice.toFixed(2).replace('.',',');
    const html = `
        <div class="qr-container">
            <p><strong>📱 Pague com PIX - ${selectedPlanName} - R$ ${valorStr}</strong></p>
            <div class="qr-code"><img src="${qrUrl}" width="240" height="240" alt="QR Code PIX" style="max-width:100%; border-radius:16px;"></div>
            <div class="chave-pix"><strong>🔑 Chave (CPF):</strong> 237.561.678-28<br><strong>👤 Beneficiário:</strong> EDUARDO SILVA DOS SANTOS<br>
            <button class="btn-primary" style="margin-top:8px;" onclick="copiarChavePix()">📋 Copiar CPF</button>
            <button class="btn-primary" style="margin-top:8px; margin-left:8px;" id="btnCopiarPayloadDinamico">📋 Copiar Payload (Copia&Cola)</button></div>
            <p style="font-size:0.8rem;">Após o pagamento, clique em "Confirmar Pagamento"</p>
            <button class="btn-primary" onclick="confirmarPagamentoPIX()">✅ Confirmar Pagamento</button>
        </div>
    `;
    document.getElementById("pixArea").innerHTML = html;
    window.payloadAtual = payload;
    const btn = document.getElementById("btnCopiarPayloadDinamico");
    if(btn) btn.onclick = (e) => { e.preventDefault(); copiarPayloadPix(); };
}
function copiarChavePix() {
    navigator.clipboard.writeText("237.561.678-28").then(() => showToast("✅ CPF copiado! Use como chave PIX."))
        .catch(() => { fallbackCopy("237.561.678-28"); showToast("✅ CPF copiado (fallback)."); });
}
function copiarPayloadPix() {
    if(window.payloadAtual) {
        navigator.clipboard.writeText(window.payloadAtual).then(() => showToast("✅ Payload Pix copiado com sucesso! Cole no app do banco."))
            .catch(() => { fallbackCopy(window.payloadAtual); showToast("✅ Payload copiado (fallback). Cole no app do banco."); });
    } else { showToast("⚠️ Payload não disponível. Selecione um plano e escolha PIX novamente.", 'error'); }
}
function fallbackCopy(text) {
    const textarea = document.createElement("textarea");
    textarea.value = text;
    document.body.appendChild(textarea);
    textarea.select();
    document.execCommand("copy");
    document.body.removeChild(textarea);
}
function showPaymentMethod(method) {
    const pixDiv = document.getElementById("pixArea");
    const cardDiv = document.getElementById("cardArea");
    const boletoDiv = document.getElementById("boletoArea");
    pixDiv.classList.remove("show");
    cardDiv.style.display = "none";
    boletoDiv.style.display = "none";
    if(method === 'pix') {
        gerarConteudoPix();
        pixDiv.style.display = "block";
        setTimeout(() => pixDiv.classList.add("show"), 10);
    } else if(method === 'card') cardDiv.style.display = "block";
    else if(method === 'boleto') boletoDiv.style.display = "block";
}
function confirmarPagamentoPIX() { if(selectedPlanName) processarPagamento('pix'); else showToast("Escolha um plano primeiro", 'error'); }
function processarPagamentoCartao() {
    const numero = document.getElementById("cardNumber").value;
    const validade = document.getElementById("cardValidade").value;
    const cvv = document.getElementById("cardCvv").value;
    if(!validarCartao(numero, validade, cvv)) { showToast("Cartão inválido. Verifique número, data ou CVV.", 'error'); return; }
    processarPagamento('card');
}
function gerarBoleto() { processarPagamento('boleto'); }

function processarPagamento(method) {
    if(!selectedPlanName) { showToast("Selecione um plano primeiro", 'error'); return; }
    const nome = document.getElementById("nomeCompleto").value.trim();
    const email = document.getElementById("emailCompra").value.trim();
    const cpf = document.getElementById("cpf").value;
    const dataNasc = document.getElementById("dataNascimento").value;
    const telefone = document.getElementById("telefone").value.trim();
    const senha = document.getElementById("senhaCadastro").value;
    if(!nome || nome.length<3) return showToast("Nome completo inválido (mínimo 3 letras)", 'error');
    if(!email || !email.includes('@') || !email.includes('.')) return showToast("E-mail inválido", 'error');
    if(!validarCPF(cpf)) return showToast("CPF inválido", 'error');
    if(!dataNasc) return showToast("Data de nascimento obrigatória", 'error');
    if(calcularIdade(dataNasc) < 18) return showToast("Você deve ter pelo menos 18 anos", 'error');
    if(!telefone || telefone.replace(/\D/g,'').length < 10) return showToast("WhatsApp inválido (mínimo 10 dígitos)", 'error');
    if(!senha || senha.length < 6) return showToast("Senha deve ter no mínimo 6 caracteres", 'error');
    if(usuariosCadastrados.find(u => u.email === email)) { showToast("Este e-mail já está cadastrado. Faça login.", 'error'); toggleTabLogin(); return; }
    showLoading(true);
    setTimeout(() => {
        let linkPDF = selectedPlanName === 'Básico' ? LINKS_PDF.basico : (selectedPlanName === 'Profissional' ? LINKS_PDF.profissional : LINKS_PDF.premium);
        const novoUsuario = { id: Date.now(), email, nome, cpf: cpf.replace(/\D/g,''), dataNascimento: dataNasc, telefone, plano: selectedPlanName, senhaHash: hashPassword(senha), dataCompra: new Date().toISOString(), pagamento: method };
        usuariosCadastrados.push(novoUsuario);
        saveUsers();
        showLoading(false);
        showSuccessModal(novoUsuario, linkPDF);
        showToast(`✅ Pagamento aprovado! Plano ${selectedPlanName} ativado.`);
        document.getElementById("nomeCompleto").value = "";
        document.getElementById("emailCompra").value = "";
        document.getElementById("cpf").value = "";
        document.getElementById("dataNascimento").value = "";
        document.getElementById("telefone").value = "";
        document.getElementById("senhaCadastro").value = "";
        document.getElementById("cardNumber").value = "";
        document.getElementById("cardName").value = "";
        document.getElementById("cardValidade").value = "";
        document.getElementById("cardCvv").value = "";
    }, 1800);
}
function showSuccessModal(user, pdfLink) {
    const modalDiv = document.createElement('div'); modalDiv.className = 'modal-dashboard';
    modalDiv.innerHTML = `<div class="dashboard-content"><div style="position:absolute;top:16px;right:24px;font-size:28px;cursor:pointer;" onclick="this.closest('.modal-dashboard').remove()">&times;</div><h2 style="color:#2ecc71;">🎉 Parabéns, ${user.nome}!</h2><p>✅ Sua matrícula na <strong>Excel Expert Academy</strong> foi confirmada! Plano: ${user.plano}.</p><p>📧 Enviamos as instruções para <strong>${user.email}</strong>.</p><hr style="margin:20px 0; border-color:#2ecc7133;"><h3>📥 Acesse seu material exclusivo agora:</h3><a href="${pdfLink}" target="_blank" class="btn-primary" style="display:inline-block;margin:20px 0;text-decoration:none;">📥 ACESSAR MATERIAL</a><div style="background:#111c2c;padding:1rem;border-radius:1rem;"><strong>🔐 Suas credenciais de acesso:</strong><br>E-mail: ${user.email}<br>Senha: (a que você criou)<br>CPF: ${user.cpf}</div><button class="btn-primary" style="margin-top:1rem;" onclick="this.closest('.modal-dashboard').remove()">Fechar</button></div>`;
    document.body.appendChild(modalDiv);
}
function fazerLoginComCpf() {
    const email = document.getElementById("loginEmail").value.trim();
    const senha = document.getElementById("loginSenha").value;
    const cpf = document.getElementById("loginCpf").value.replace(/\D/g,'');
    const user = usuariosCadastrados.find(u => u.email === email);
    if(!user || user.cpf !== cpf || !verifyPassword(senha, user.senhaHash)) return showToast("Credenciais inválidas. Verifique e-mail, CPF e senha.", 'error');
    let link = user.plano === 'Básico' ? LINKS_PDF.basico : (user.plano === 'Profissional' ? LINKS_PDF.profissional : LINKS_PDF.premium);
    showSuccessModal(user, link);
}
function showToast(msg, type='success') {
    let d = document.createElement('div'); d.className='toast'; d.innerText = (type==='success'?'✅ ':'⚠️ ')+msg;
    document.body.appendChild(d); setTimeout(()=>d.remove(), 3500);
}
function showLoading(show) {
    let el = document.querySelector('.loading-overlay');
    if(show && !el) { let o=document.createElement('div'); o.className='loading-overlay'; o.innerHTML='<div class="spinner"></div><p>Processando pagamento...</p>'; document.body.appendChild(o); }
    else if(!show && el) el.remove();
}
function toggleTabLogin() { document.getElementById("painelCompra").style.display = "none"; document.getElementById("painelLogin").style.display = "block"; }
document.getElementById("btnTabPagamento").onclick = () => { document.getElementById("painelCompra").style.display = "block"; document.getElementById("painelLogin").style.display = "none"; };
document.getElementById("btnTabLogin").onclick = toggleTabLogin;
document.getElementById("verPlanosBtn").onclick = () => document.getElementById("plans-section").scrollIntoView({behavior:"smooth"});

// Contadores animados
function animateCounter(el, target) {
    let current = 0, step = target/50;
    let timer = setInterval(() => { current += step; if(current>=target) { el.innerText = target.toLocaleString(); clearInterval(timer); } else el.innerText = Math.floor(current).toLocaleString(); }, 30);
}
window.addEventListener('load', () => { loadUsers(); animateCounter(document.getElementById('alunosCount'),15420); animateCounter(document.getElementById('certificadosCount'),12890); animateCounter(document.getElementById('aulasCount'),187); });
window.addEventListener('scroll', () => { let back=document.getElementById('backToTop'); if(window.scrollY>400) back.style.display='flex'; else back.style.display='none'; });
document.getElementById('backToTop').onclick = () => window.scrollTo({top:0,behavior:'smooth'});

// IA Chat
const iaBtn = document.getElementById("iaFabBtn"), iaWindow = document.getElementById("iaChatWindow"), closeChat = document.getElementById("closeChatBtn");
iaBtn.onclick = () => iaWindow.classList.toggle("open");
closeChat.onclick = () => iaWindow.classList.remove("open");
function askIA() { let input=document.getElementById("iaQuestion"), q=input.value.trim(); if(!q) return; addMessage(q,'user'); input.value=''; setTimeout(()=>addMessage(getAIResponse(q),'bot'),400); }
function addMessage(t,sender) { let c=document.getElementById("iaMessages"), d=document.createElement('div'); d.className=sender==='user'?'message-user':'message-bot'; d.innerText=t; c.appendChild(d); c.scrollTop=c.scrollHeight; }
function getAIResponse(q) { let l=q.toLowerCase(); if(l.includes('preço')) return "💰 Planos: Básico R$49,90 | Profissional R$110,80 | Premium R$260,40"; if(l.includes('diferença')) return "📊 Básico: fundamentos | Profissional: +Dashboards+Power Query | Premium: +VBA+Power BI+Mentoria"; if(l.includes('pix')) return "💳 Pagamento via PIX com QR Code oficial (CPF 237.561.678-28)."; return "Posso ajudar com preços, diferenças entre planos ou formas de pagamento!"; }
function sendSuggestion(t) { document.getElementById("iaQuestion").value=t; askIA(); }

// Máscaras
document.getElementById("cpf")?.addEventListener("input", function(e){ let v=e.target.value.replace(/\D/g,''); if(v.length>11) v=v.slice(0,11); e.target.value=v.replace(/(\d{3})(\d)/,'$1.$2').replace(/(\d{3})(\d)/,'$1.$2').replace(/(\d{3})(\d{1,2})$/,'$1-$2'); });
document.getElementById("telefone")?.addEventListener("input", function(e){ let v=e.target.value.replace(/\D/g,''); if(v.length===10) e.target.value=v.replace(/(\d{2})(\d{4})(\d{4})/,'($1) $2-$3'); else if(v.length===11) e.target.value=v.replace(/(\d{2})(\d{5})(\d{4})/,'($1) $2-$3'); });
document.getElementById("cardNumber")?.addEventListener("input", function(e){ let v=e.target.value.replace(/\D/g,''); e.target.value=v.replace(/(\d{4})(?=\d)/g,'$1 '); });
document.getElementById("cardValidade")?.addEventListener("input",function(e){ let v=e.target.value.replace(/\D/g,''); if(v.length>=3) e.target.value=v.slice(0,2)+'/'+v.slice(2,4); });

// Reveal animation
const reveals = document.querySelectorAll('.reveal');
function animateOnScroll() { let t=window.innerHeight*0.85; reveals.forEach(el=>{ if(el.getBoundingClientRect().top<t) el.classList.add('active'); }); }
window.addEventListener('scroll', animateOnScroll);
window.selectPlan = selectPlan; window.showPaymentMethod = showPaymentMethod; window.copiarChavePix = copiarChavePix; window.copiarPayloadPix = copiarPayloadPix;
window.confirmarPagamentoPIX = confirmarPagamentoPIX; window.processarPagamentoCartao = processarPagamentoCartao; window.gerarBoleto = gerarBoleto;
window.fazerLoginComCpf = fazerLoginComCpf; window.showForgotPassword = () => showToast("Recuperação de senha: entre em contato pelo WhatsApp 17 99772-9758", 'error');
window.sendSuggestion = sendSuggestion; window.askIA = askIA;
</script>
</body>
</html>
