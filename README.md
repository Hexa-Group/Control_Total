<DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8">
  <title>Control Hogar</title>
  

</head>
<body>
<!-- partial:index.partial.html -->
<!DOCTYPE html>
<html lang="es">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Control Hogar - Hexa Group | Sistema Inteligente de Seguridad</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Poppins:wght@300;400;600&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #0a0a2e 0%, #16213e 30%, #1e3a8a 70%, #3b82f6 100%);
      color: white;
      overflow-x: hidden;
    }

    .hero {
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      background: radial-gradient(circle at 30% 50%, rgba(59, 130, 246, 0.15) 0%, transparent 50%);
    }

    .hero-content {
      text-align: center;
      z-index: 10;
      max-width: 900px;
      padding: 20px;
    }

    .logo-container {
      margin-bottom: 30px;
      position: relative;
    }

    .company-logo {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      background: white;
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 0 auto 20px;
      box-shadow: 0 0 30px rgba(59, 130, 246, 0.5);
      animation: logoGlow 3s ease-in-out infinite alternate;
    }

    .company-logo img {
      width: 100px;
      height: 100px;
      object-fit: contain;
    }

    @keyframes logoGlow {
      from {
        box-shadow: 0 0 30px rgba(59, 130, 246, 0.5);
      }

      to {
        box-shadow: 0 0 50px rgba(59, 130, 246, 0.8);
      }
    }

    .hero h1 {
      font-size: 4.5rem;
      font-weight: 900;
      margin-bottom: 10px;
      background: linear-gradient(45deg, #3b82f6, #60a5fa, #93c5fd);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-transform: uppercase;
      letter-spacing: 3px;
      animation: titleGlow 2s ease-in-out infinite alternate;
    }

    .hero .subtitle {
      font-size: 1.8rem;
      color: #60a5fa;
      font-weight: 700;
      margin-bottom: 20px;
      text-transform: uppercase;
      letter-spacing: 2px;
    }

    @keyframes titleGlow {
      from {
        filter: drop-shadow(0 0 20px rgba(59, 130, 246, 0.5));
      }

      to {
        filter: drop-shadow(0 0 40px rgba(59, 130, 246, 0.8));
      }
    }

    .hero p {
      font-size: 1.4rem;
      margin-bottom: 40px;
      opacity: 0.9;
      font-weight: 400;
    }

    .cta-buttons {
      display: flex;
      gap: 20px;
      justify-content: center;
      flex-wrap: wrap;
    }

    .cta-button {
      background: linear-gradient(45deg, #1e40af, #3b82f6);
      padding: 18px 35px;
      font-size: 1.1rem;
      font-weight: 700;
      border: none;
      border-radius: 50px;
      color: white;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 10px 30px rgba(59, 130, 246, 0.4);
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 10px;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .cta-button:hover {
      transform: translateY(-5px);
      box-shadow: 0 20px 40px rgba(59, 130, 246, 0.6);
      background: linear-gradient(45deg, #3b82f6, #60a5fa);
    }

    .whatsapp-btn {
      background: linear-gradient(45deg, #059669, #10b981) !important;
      box-shadow: 0 10px 30px rgba(16, 185, 129, 0.4) !important;
    }

    .whatsapp-btn:hover {
      box-shadow: 0 20px 40px rgba(16, 185, 129, 0.6) !important;
      background: linear-gradient(45deg, #10b981, #34d399) !important;
    }

    .floating-elements {
      position: absolute;
      width: 100%;
      height: 100%;
      pointer-events: none;
    }

    .floating-icon {
      position: absolute;
      font-size: 3rem;
      opacity: 0.1;
      animation: float 6s ease-in-out infinite;
      color: #3b82f6;
    }

    @keyframes float {

      0%,
      100% {
        transform: translateY(0px) rotate(0deg);
      }

      50% {
        transform: translateY(-20px) rotate(10deg);
      }
    }

    .demo-section {
      padding: 100px 20px;
      max-width: 1400px;
      margin: 0 auto;
    }

    .section-title {
      text-align: center;
      font-size: 3rem;
      font-weight: 900;
      margin-bottom: 60px;
      background: linear-gradient(45deg, #3b82f6, #60a5fa);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-transform: uppercase;
      letter-spacing: 2px;
    }

    .demo-container {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 60px;
      align-items: center;
    }

    .phone-mockup {
      background: linear-gradient(145deg, #1e3a8a, #3b82f6);
      border-radius: 40px;
      padding: 30px;
      box-shadow: 0 30px 60px rgba(59, 130, 246, 0.3);
      transform: perspective(1000px) rotateY(-15deg);
      transition: all 0.3s ease;
      border: 2px solid #60a5fa;
    }

    .phone-mockup:hover {
      transform: perspective(1000px) rotateY(0deg) scale(1.05);
      box-shadow: 0 40px 80px rgba(59, 130, 246, 0.4);
    }

    .phone-screen {
      background: linear-gradient(145deg, #0f172a, #1e293b);
      border-radius: 25px;
      padding: 30px;
      min-height: 600px;
      border: 1px solid #3b82f6;
    }

    .app-header {
      text-align: center;
      margin-bottom: 30px;
      padding: 15px;
      background: rgba(59, 130, 246, 0.2);
      border-radius: 15px;
      border: 1px solid #3b82f6;
    }

    .app-header h3 {
      color: #60a5fa;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .control-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
      margin-bottom: 30px;
    }

    .control-item {
      background: rgba(59, 130, 246, 0.1);
      border-radius: 15px;
      padding: 20px;
      text-align: center;
      transition: all 0.3s ease;
      cursor: pointer;
      border: 1px solid rgba(59, 130, 246, 0.3);
    }

    .control-item:hover {
      background: rgba(59, 130, 246, 0.2);
      transform: translateY(-5px);
      border-color: #3b82f6;
    }

    .control-item.active {
      background: rgba(59, 130, 246, 0.3);
      border-color: #60a5fa;
      box-shadow: 0 0 20px rgba(59, 130, 246, 0.5);
    }

    .control-icon {
      font-size: 2rem;
      margin-bottom: 10px;
    }

    .security-modes {
      background: rgba(59, 130, 246, 0.1);
      border-radius: 15px;
      padding: 20px;
      margin-bottom: 20px;
      border: 1px solid rgba(59, 130, 246, 0.3);
    }

    .security-modes h4 {
      color: #60a5fa;
      font-weight: 700;
    }

    .mode-buttons {
      display: flex;
      gap: 10px;
      margin-top: 15px;
    }

    .mode-btn {
      flex: 1;
      padding: 10px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: all 0.3s ease;
      font-weight: 600;
      font-size: 0.9rem;
    }

    .mode-silent {
      background: rgba(100, 100, 100, 0.3);
      color: white;
    }

    .mode-light {
      background: rgba(255, 193, 7, 0.3);
      color: #ffc107;
    }

    .mode-sound {
      background: rgba(220, 53, 69, 0.3);
      color: #dc3545;
    }

    .mode-btn.active {
      transform: scale(1.1);
      box-shadow: 0 5px 15px rgba(59, 130, 246, 0.4);
    }

    .features-list {
      list-style: none;
    }

    .features-list li {
      padding: 15px 0;
      border-bottom: 1px solid rgba(59, 130, 246, 0.2);
      display: flex;
      align-items: center;
      font-size: 1.1rem;
      font-weight: 500;
    }

    .features-list li::before {
      content: "✓";
      color: #60a5fa;
      font-weight: bold;
      font-size: 1.5rem;
      margin-right: 15px;
    }

    .pricing-section {
      background: rgba(15, 23, 42, 0.7);
      padding: 100px 20px;
      margin: 100px 0;
      border-top: 2px solid #3b82f6;
      border-bottom: 2px solid #3b82f6;
    }

    .pricing-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 40px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .pricing-card {
      background: linear-gradient(145deg, #1e3a8a, #3b82f6);
      border-radius: 25px;
      padding: 40px;
      text-align: center;
      position: relative;
      transition: all 0.3s ease;
      border: 2px solid rgba(59, 130, 246, 0.3);
    }

    .pricing-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 30px 60px rgba(59, 130, 246, 0.4);
      border-color: #60a5fa;
    }

    .pricing-card.featured {
      border-color: #60a5fa;
      transform: scale(1.05);
      box-shadow: 0 20px 40px rgba(59, 130, 246, 0.3);
    }

    .pricing-card h3 {
      font-size: 1.8rem;
      font-weight: 700;
      margin-bottom: 10px;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .price {
      font-size: 3.5rem;
      font-weight: 900;
      color: #60a5fa;
      margin: 20px 0;
    }

    .price-usd {
      font-size: 1.2rem;
      color: #93c5fd;
      font-weight: 400;
    }

    .customizer {
      background: rgba(59, 130, 246, 0.1);
      border-radius: 20px;
      padding: 40px;
      margin: 60px 0;
      border: 2px solid rgba(59, 130, 246, 0.3);
    }

    .customizer h3 {
      text-align: center;
      margin-bottom: 30px;
      font-size: 2rem;
      font-weight: 700;
      color: #60a5fa;
      text-transform: uppercase;
      letter-spacing: 1px;
    }

    .slider-container {
      margin: 30px 0;
    }

    .slider-container label {
      display: block;
      margin-bottom: 10px;
      font-weight: 600;
      color: #93c5fd;
    }

    .slider {
      width: 100%;
      height: 8px;
      border-radius: 5px;
      background: rgba(59, 130, 246, 0.3);
      outline: none;
      -webkit-appearance: none;
    }

    .slider::-webkit-slider-thumb {
      -webkit-appearance: none;
      width: 25px;
      height: 25px;
      border-radius: 50%;
      background: #3b82f6;
      cursor: pointer;
      box-shadow: 0 0 10px rgba(59, 130, 246, 0.5);
    }

    .total-price {
      text-align: center;
      font-size: 2.8rem;
      color: #60a5fa;
      font-weight: 900;
      margin-top: 30px;
    }

    .stats-section {
      padding: 80px 20px;
      background: rgba(0, 0, 0, 0.3);
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 40px;
      max-width: 1000px;
      margin: 0 auto;
      text-align: center;
    }

    .stat-item {
      padding: 30px;
      background: rgba(59, 130, 246, 0.1);
      border-radius: 20px;
      border: 1px solid rgba(59, 130, 246, 0.3);
      transition: all 0.3s ease;
    }

    .stat-item:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 30px rgba(59, 130, 246, 0.2);
    }

    .stat-number {
      font-size: 3rem;
      font-weight: 900;
      color: #60a5fa;
      display: block;
    }

    .stat-label {
      font-size: 1.2rem;
      opacity: 0.9;
      margin-top: 10px;
      font-weight: 600;
    }

    .commercial-section {
      background: linear-gradient(135deg, #1e3a8a, #3b82f6);
      padding: 80px 20px;
      margin: 60px 0;
      text-align: center;
    }

    .commercial-section h2 {
      font-size: 3rem;
      font-weight: 900;
      margin-bottom: 30px;
      text-transform: uppercase;
      letter-spacing: 2px;
    }

    .commercial-features {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
      max-width: 1000px;
      margin: 40px auto;
    }

    .commercial-feature {
      background: rgba(255, 255, 255, 0.1);
      padding: 30px;
      border-radius: 15px;
      border: 1px solid rgba(255, 255, 255, 0.2);
    }

    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2.8rem;
      }

      .hero .subtitle {
        font-size: 1.4rem;
      }

      .demo-container {
        grid-template-columns: 1fr;
      }

      .phone-mockup {
        transform: none;
      }

      .control-grid {
        grid-template-columns: 1fr;
      }

      .cta-buttons {
        flex-direction: column;
        align-items: center;
      }

      .pricing-grid {
        grid-template-columns: 1fr;
      }
    }

    .contact-section {
      background: rgba(15, 23, 42, 0.9);
      padding: 80px 20px;
      text-align: center;
      border-top: 2px solid #3b82f6;
    }

    .contact-info {
      max-width: 800px;
      margin: 0 auto;
    }

    .contact-info h2 {
      font-size: 2.5rem;
      font-weight: 700;
      margin-bottom: 30px;
      color: #60a5fa;
      text-transform: uppercase;
    }

    .contact-details {
      display: flex;
      justify-content: center;
      gap: 40px;
      flex-wrap: wrap;
      margin-top: 40px;
    }

    .contact-item {
      display: flex;
      align-items: center;
      gap: 15px;
      font-size: 1.2rem;
      font-weight: 600;
    }

    .whatsapp-float {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: linear-gradient(45deg, #059669, #10b981);
      border-radius: 50%;
      width: 60px;
      height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 4px 20px rgba(16, 185, 129, 0.4);
      z-index: 1000;
      animation: pulse 2s infinite;
      cursor: pointer;
      text-decoration: none;
    }

    @keyframes pulse {
      0% {
        transform: scale(1);
      }

      50% {
        transform: scale(1.1);
      }

      100% {
        transform: scale(1);
      }
    }
  </style>
</head>

<body>
  <section class="hero">
    <div class="floating-elements">
      <div class="floating-icon" style="top: 20%; left: 10%; animation-delay: 0s;">🏠</div>
      <div class="floating-icon" style="top: 40%; right: 15%; animation-delay: 1s;">🔒</div>
      <div class="floating-icon" style="bottom: 30%; left: 20%; animation-delay: 2s;">💡</div>
      <div class="floating-icon" style="top: 60%; right: 25%; animation-delay: 1.5s;">📱</div>
      <div class="floating-icon" style="bottom: 20%; right: 10%; animation-delay: 0.5s;">🎥</div>
    </div>

    <div class="hero-content">
      <div class="logo-container">
        <div class="company-logo">
          <svg width="100" height="100" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
            <!-- Casa -->
            <path d="M40 120 L100 60 L160 120 L160 180 L40 180 Z" fill="none" stroke="#1e40af" stroke-width="4" />
            <path d="M40 120 L100 60 L160 120" fill="none" stroke="#1e40af" stroke-width="4" />
            <!-- Texto HEXA -->
            <text x="100" y="140" text-anchor="middle" fill="#1e40af" font-family="Arial Black" font-size="16" font-weight="900">HEXA</text>
            <text x="100" y="158" text-anchor="middle" fill="#1e40af" font-family="Arial Black" font-size="16" font-weight="900">GROUP</text>
            <text x="100" y="174" text-anchor="middle" fill="#3b82f6" font-family="Arial" font-size="10" font-weight="600">CONTROL TOTAL</text>
          </svg>
        </div>
      </div>

      <h1>CONTROL HOGAR</h1>
      <div class="subtitle">Hexa Group</div>
      <p>Tu casa inteligente y segura desde cualquier lugar del mundo</p>

      <div class="cta-buttons">
        <a href="#demo" class="cta-button">
          🎮 Ver Demo Interactivo
        </a>
        <a href="https://wa.me/5493812107020?text=Hola!%20Me%20interesa%20el%20sistema%20Control%20Hogar.%20Quiero%20más%20información." class="cta-button whatsapp-btn" target="_blank">
          📱 WhatsApp
        </a>
      </div>
    </div>
  </section>

  <section class="stats-section">
    <div class="stats-grid">
      <div class="stat-item">
        <span class="stat-number">78%</span>
        <span class="stat-label">Reducción en robos</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">45%</span>
        <span class="stat-label">Ahorro energético</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">24/7</span>
        <span class="stat-label">Monitoreo completo</span>
      </div>
      <div class="stat-item">
        <span class="stat-number">∞</span>
        <span class="stat-label">Distancia de control</span>
      </div>
    </div>
  </section>

  <section class="demo-section" id="demo">
    <h2 class="section-title">Controla Todo Desde Tu Celular</h2>

    <div class="demo-container">
      <div class="phone-mockup">
        <div class="phone-screen">
          <div class="app-header">
            <h3>🏠 Control Hogar</h3>
            <p>Estado: <span id="status">🟢 Seguro</span></p>
          </div>

          <div class="control-grid">
            <div class="control-item" onclick="toggleDevice(this, 'Luces')">
              <div class="control-icon">💡</div>
              <div>Luces</div>
              <small>Living, Cocina, Dormitorio</small>
            </div>

            <div class="control-item" onclick="toggleDevice(this, 'Pava Eléctrica')">
              <div class="control-icon">🫖</div>
              <div>Pava Eléctrica</div>
              <small>Cocina</small>
            </div>

            <div class="control-item" onclick="toggleDevice(this, 'Cafetera')">
              <div class="control-icon">☕</div>
              <div>Cafetera</div>
              <small>Cocina</small>
            </div>

            <div class="control-item" onclick="toggleDevice(this, 'Ventilador')">
              <div class="control-icon">🌀</div>
              <div>Ventilador</div>
              <small>Dormitorio</small>
            </div>
          </div>

          <div class="security-modes">
            <h4>🛡️ Modos de Seguridad</h4>
            <div class="mode-buttons">
              <button class="mode-btn mode-silent" onclick="setSecurityMode(this, 'Silencioso')">🔇 Silencioso</button>
              <button class="mode-btn mode-light active" onclick="setSecurityMode(this, 'Luminoso')">💡 Luminoso</button>
              <button class="mode-btn mode-sound" onclick="setSecurityMode(this, 'Sonoro')">🔊 Sonoro</button>
            </div>
          </div>

          <div class="control-item" onclick="showCameras()">
            <div class="control-icon">📹</div>
            <div>Cámaras 360°</div>
            <small>Ver en vivo</small>
          </div>
        </div>
      </div>

      <div>
        <ul class="features-list">
          <li>Control remoto desde cualquier parte del mundo</li>
          <li>Programación inteligente de horarios ON/OFF</li>
          <li>Sensores de movimiento, 360° techo y apertura</li>
          <li>3 modos: alarma silenciosa, luminosa y sonora</li>
          <li>Integración con cámaras de seguridad 360° Wi-Fi</li>
          <li>Kit personalizable hasta 12 luces controlables</li>
          <li>Sirena de alta potencia configurable</li>
          <li>App móvil intuitiva Control Hogar</li>
          <li>Instalación profesional incluida</li>
          <li>Soporte técnico 24/7 Hexa Group</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="commercial-section">
    <h2>CONTROL TOTAL - PARA COMERCIOS</h2>
    <p style="font-size: 1.3rem; margin-bottom: 40px;">Protección empresarial de nivel superior</p>

    <div class="commercial-features">
      <div class="commercial-feature">
        <h3>🏢 Multi-Sucursales</h3>
        <p>Control centralizado de múltiples ubicaciones desde una sola app</p>
      </div>
      <div class="commercial-feature">
        <h3>👥 Usuarios Múltiples</h3>
        <p>Acceso por niveles: administradores, gerentes y empleados</p>
      </div>
      <div class="commercial-feature">
        <h3>📊 Reportes Avanzados</h3>
        <p>Estadísticas detalladas de uso y eventos de seguridad</p>
      </div>
      <div class="commercial-feature">
        <h3>🚨 Alertas Inmediatas</h3>
        <p>Notificaciones instantáneas a múltiples contactos</p>
      </div>
    </div>
  </section>

  <section class="pricing-section">
    <h2 class="section-title">Planes y Precios</h2>

    <div class="pricing-grid">
      <div class="pricing-card">
        <h3>Kit Básico</h3>
        <div class="price">$299<span class="price-usd">USD</span></div>
        <ul style="text-align: left; list-style: none; padding: 0;">
          <li>✓ 1 Sensores de movimiento Gral</li>
          <li>✓ 1 Sirena configurable</li>
          <li>✓ Control de 4 luces</li>
          <li>✓ 1 Enchufes inteligentes programable</li>
          <li>✓ App Control Hogar incluida</li>
          <li>✓ Instalación profesional</li>
        </ul>
        <a href="https://wa.me/5493812107020?text=Hola!%20Me%20interesa%20el%20Kit%20Básico%20de%20Control%20Hogar%20($299%20USD).%20Quiero%20más%20información." class="cta-button" style="margin-top: 20px;" target="_blank">Elegir Plan</a>
      </div>

      <div class="pricing-card featured">
        <div style="position: absolute; top: -15px; left: 50%; transform: translateX(-50%); background: #60a5fa; color: #0f172a; padding: 5px 20px; border-radius: 20px; font-weight: bold;">MÁS POPULAR</div>
        <h3>Kit Completo</h3>
        <div class="price">$599<span class="price-usd">USD</span></div>
        <ul style="text-align: left; list-style: none; padding: 0;">
          <li>✓ 2 Sensores de movimiento</li>
          <li>✓ 2 Sensores de apertura</li>
          <li>✓ 1 Sirenas configurables</li>
          <li>✓ Control de 8 luces</li>
          <li>✓ 2 Enchufes inteligentes</li>
          <li>✓ 2 Cámaras 360° Wi-Fi</li>
          <li>✓ App Control Hogar premium</li>
          <li>✓ Programación horarios ON/OFF</li>
        </ul>
        <a href="https://wa.me/5493812107020?text=Hola!%20Me%20interesa%20el%20Kit%20Completo%20de%20Control%20Hogar%20($599%20USD).%20Quiero%20más%20información." class="cta-button" style="margin-top: 20px;" target="_blank">Elegir Plan</a>
      </div>

      <div class="pricing-card">
        <h3>Control Total<br><small>(Comercios)</small></h3>
        <div class="price">$899<span class="price-usd">USD</span></div>
        <ul style="text-align: left; list-style: none; padding: 0;">
          <li>✓ 8 Sensores de movimiento</li>
          <li>✓ 2 Sirenas de alta potencia</li>
          <li>✓ Control de 12 luces</li>
          <li>✓ 4 Enchufes inteligentes</li>
          <li>✓ 4 Cámaras 360° Wi-Fi</li>
          <li>✓ Panel Control Total comercial</li>
          <li>✓ Multi-usuarios y reportes</li>
        </ul>
        <a href="https://wa.me/5493812107020?text=Hola!%20Me%20interesa%20el%20sistema%20Control%20Total%20para%20comercio%20($899%20USD).%20Quiero%20más%20información." class="cta-button" style="margin-top: 20px;" target="_blank">Elegir Plan</a>
      </div>
    </div>

    <div class="customizer">
      <h3>🛠️ Personaliza Tu Kit</h3>

      <div class="slider-container">
        <label>Sensores: <span id="sensors-count">2</span></label>
        <input type="range" min="1" max="12" value="2" class="slider" id="sensors" oninput="updatePrice()">
      </div>

      <div class="slider-container">
        <label>Sirenas: <span id="sirens-count">1</span></label>
        <input type="range" min="1" max="6" value="1" class="slider" id="sirens" oninput="updatePrice()">
      </div>

      <div class="slider-container">
        <label>Luces Controlables: <span id="lights-count">4</span></label>
        <input type="range" min="4" max="12" value="4" class="slider" id="lights" oninput="updatePrice()">
      </div>

      <div class="slider-container">
        <label>Cámaras 360°: <span id="cameras-count">0</span></label>
        <input type="range" min="0" max="8" value="0" class="slider" id="cameras" oninput="updatePrice()">
      </div>

      <div class="total-price">
        Total: $<span id="total-price">299</span> <span class="price-usd">USD</span>
      </div>

      <div style="text-align: center; margin-top: 30px;">
        <a href="#" onclick="sendCustomQuote()" class="cta-button">📋 Solicitar Cotización Personalizada</a>
      </div>
    </div>
  </section>

  <section class="contact-section">
    <div class="contact-info">
      <h2>CONTÁCTANOS AHORA</h2>
      <p style="font-size: 1.2rem; margin-bottom: 30px;">
        Protege y controla tu casa AHORA! Quedáte tranquilo, que está va por cuenta de nosotros!
      </p>

      <div class="contact-details">
        <div class="contact-item">
          <span style="font-size: 1.5rem;">📱</span>
          <span>+54 9 381 654 3778</span>
        </div>
        <div class="contact-item">
          <span style="font-size: 1.5rem;">📍</span>
          <span>Tucumán, Argentina</span>
        </div>
        <div class="contact-item">
          <span style="font-size: 1.5rem;">📧</span>
          <span>@hexa.group.tuc</span>
        </div>
      </div>

      <div style="margin-top: 40px;">
        <a href="https://wa.me/5493812107020?text=Hola%20Hexa%20Group!%20Me%20interesa%20el%20sistema%20Control%20Hogar.%20Quiero%20que%20me%20asesoren%20sobre%20la%20mejor%20opción%20para%20mi%20hogar/comercio." class="cta-button whatsapp-btn" target="_blank" style="font-size: 1.3rem; padding: 20px 40px;">
          💬 Asesoría Gratuita por WhatsApp
        </a>
      </div>
    </div>
  </section>

  <!-- WhatsApp Float Button -->
  <a href="https://wa.me/5493812107020?text=Hola!%20Me%20interesa%20Control%20Hogar%20de%20Hexa%20Group" class="whatsapp-float" target="_blank">
    <span style="font-size: 1.8rem;">💬</span>
  </a>

  <script>
    function toggleDevice(element, deviceName) {
      element.classList.toggle('active');
      const isActive = element.classList.contains('active');
      // Actualizar status
      const activeDevices = document.querySelectorAll('.control-item.active').length;
      const status = document.getElementById('status');
      if (activeDevices > 0) {
        status.innerHTML = `🟡 ${activeDevices} dispositivo${activeDevices > 1 ? 's' : ''} activo${activeDevices > 1 ? 's' : ''}`;
      } else {
        status.innerHTML = '🟢 Seguro';
      }
      // Efecto visual
      if (isActive) {
        element.style.background = 'rgba(59, 130, 246, 0.4)';
        element.style.transform = 'translateY(-5px) scale(1.05)';
        element.style.boxShadow = '0 0 25px rgba(59, 130, 246, 0.6)';
      } else {
        element.style.background = 'rgba(59, 130, 246, 0.1)';
        element.style.transform = 'translateY(0) scale(1)';
        element.style.boxShadow = 'none';
      }
    }

    function setSecurityMode(element, mode) {
      // Remover active de todos los botones
      document.querySelectorAll('.mode-btn').forEach(btn => btn.classList.remove('active'));
      // Activar el botón seleccionado
      element.classList.add('active');
      // Actualizar status
      const status = document.getElementById('status');
      const modeEmojis = {
        'Silencioso': '🔇',
        'Luminoso': '💡',
        'Sonoro': '🔊'
      };
      status.innerHTML = `${modeEmojis[mode]} Modo ${mode} activo`;
      // Efecto visual en toda la pantalla
      const screen = document.querySelector('.phone-screen');
      screen.style.animation = 'pulse 0.5s ease-in-out';
      setTimeout(() => {
        screen.style.animation = '';
      }, 500);
    }

    function showCameras() {
      alert('🎥 Abriendo vista de cámaras 360°...\n\n• Vista completa del perímetro\n• Grabación en tiempo real\n• Detección de movimiento Wi-Fi\n• Visión nocturna HD\n• Zoom digital 10x\n• Integración Control Hogar');
    }

    function updatePrice() {
      const sensors = parseInt(document.getElementById('sensors').value);
      const sirens = parseInt(document.getElementById('sirens').value);
      const lights = parseInt(document.getElementById('lights').value);
      const cameras = parseInt(document.getElementById('cameras').value);
      // Actualizar contadores
      document.getElementById('sensors-count').textContent = sensors;
      document.getElementById('sirens-count').textContent = sirens;
      document.getElementById('lights-count').textContent = lights;
      document.getElementById('cameras-count').textContent = cameras;
      // Calcular precio
      let basePrice = 199; // Precio base del sistema
      let total = basePrice;
      total += sensors * 25; // $25 por sensor adicional
      total += sirens * 35; // $35 por sirena adicional
      total += lights * 15; // $15 por luz adicional
      total += cameras * 120; // $120 por cámara
      document.getElementById('total-price').textContent = total;
    }

    function sendCustomQuote() {
      const sensors = document.getElementById('sensors').value;
      const sirens = document.getElementById('sirens').value;
      const lights = document.getElementById('lights').value;
      const cameras = document.getElementById('cameras').value;
      const total = document.getElementById('total-price').textContent;
      const message = `Hola Hexa Group! Quiero una cotización personalizada para Control Hogar:
            
🔧 CONFIGURACIÓN PERSONALIZADA:
• Sensores: ${sensors}
• Sirenas: ${sirens}  
• Luces controlables: ${lights}
• Cámaras 360°: ${cameras}
• Total estimado: ${total} USD

¿Pueden confirmarme el precio final y disponibilidad?`;
      const encodedMessage = encodeURIComponent(message);
      window.open(`https://wa.me/5493812107020?text=${encodedMessage}`, '_blank');
    }
    // Agregar animación de pulso
    const style = document.createElement('style');
    style.textContent = `
            @keyframes pulse {
                0% { transform: scale(1); }
                50% { transform: scale(1.02); box-shadow: 0 0 30px rgba(59, 130, 246, 0.5); }
                100% { transform: scale(1); }
            }
        `;
    document.head.appendChild(style);
    // Scroll suave para el botón CTA
    document.querySelector('.cta-button').addEventListener('click', function(e) {
      if (this.getAttribute('href') === '#demo') {
        e.preventDefault();
        document.getElementById('demo').scrollIntoView({
          behavior: 'smooth'
        });
      }
    });
    // Animación de entrada para los elementos
    const observerOptions = {
      threshold: 0.1,
      rootMargin: '0px 0px -50px 0px'
    };
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.style.opacity = '1';
          entry.target.style.transform = 'translateY(0)';
        }
      });
    }, observerOptions);
    // Observar elementos para animaciones
    document.querySelectorAll('.pricing-card, .control-item, .features-list li, .stat-item').forEach(el => {
      el.style.opacity = '0';
      el.style.transform = 'translateY(30px)';
      el.style.transition = 'all 0.6s ease';
      observer.observe(el);
    });
    // Efecto de typing en el hero
    window.addEventListener('load', function() {
      const title = document.querySelector('.hero h1');
      title.style.animation = 'titleGlow 2s ease-in-out infinite alternate, typing 3s steps(13) 1s 1 normal both';
    });
  </script>
</body>

</html>
<style>
  h1,
  h2,
  h3 {
    font-family: 'Orbitron', sans-serif !important;
  }
</style>
<!-- partial -->
  
</body>
</html>
