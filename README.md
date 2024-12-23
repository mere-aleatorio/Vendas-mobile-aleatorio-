<html><head><base href="/">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VinizModz&#x1f451;</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&amp;display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
  }

  body {
    background: linear-gradient(45deg, rgba(15, 15, 26, 0.95), rgba(26, 26, 45, 0.95)),
                url('https://cdn.discordapp.com/attachments/1273680926412640378/1311865445913202728/Viniz-lite.png?ex=67617ba7&is=67602a27&hm=50371d7468a2b54bd45b0977aef2a86ca2cc564e8d8e1a22e58894576bd89d86&');
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
    color: #fff;
    min-height: 100vh;
    position: relative;
    padding-bottom: 80px;
    animation: backgroundPulse 15s ease-in-out infinite;
  }

  @keyframes backgroundPulse {
    0% { background-color: rgba(15, 15, 26, 0.85); }
    50% { background-color: rgba(26, 26, 45, 0.9); }
    100% { background-color: rgba(15, 15, 26, 0.85); }
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 30px;
    display: flex;
    justify-content: center;
    align-items: stretch;
    gap: 30px;
    flex-wrap: wrap;
  }

  header {
    text-align: center;
    padding: 60px 0;
    background: rgba(0,0,0,0.4);
    margin-bottom: 40px;
    border-bottom: 3px solid rgba(0,255,136,0.4);
    box-shadow: 0 5px 25px rgba(0,255,136,0.15);
  }

  header h1 {
    font-size: 4.5em;
    margin-bottom: 25px;
    color: #00ff88;
    text-shadow: 0 0 15px rgba(0,255,136,0.6);
    letter-spacing: 3px;
  }

  header p {
    font-size: 1.4em;
    color: #cccccc;
    max-width: 600px;
    margin: 0 auto;
    line-height: 1.6;
  }

  .discord-button, .rules-button {
    display: inline-block;
    background: #5865F2;
    color: white;
    padding: 18px 35px;
    border-radius: 35px;
    text-decoration: none;
    margin: 15px 20px;
    transition: all 0.3s ease;
    font-weight: bold;
  }

  .rules-button {
    background: #ff6b6b;
  }

  .discord-button:hover {
    background: #4752C4;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(88,101,242,0.4);
  }

  .rules-button:hover {
    background: #ff5252;
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(255,107,107,0.4);
  }

  .product-card {
    background: rgba(255,255,255,0.07);
    border-radius: 25px;
    padding: 40px;
    text-align: center;
    transition: all 0.5s ease;
    flex: 0 0 400px;
    margin: 20px;
    backdrop-filter: blur(15px);
    border: 2px solid rgba(0,255,136,0.15);
    box-shadow: 0 15px 35px rgba(0,0,0,0.4);
  }

  .product-card.offline {
    opacity: 0.7;
    position: relative;
  }

  .product-card.offline::before {
    content: "EM ATUALIZAÇÃO";
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%) rotate(-15deg);
    background: #ff6b6b;
    color: white;
    padding: 10px 20px;
    font-weight: bold;
    border-radius: 5px;
    z-index: 1;
  }

  .product-card.offline .plan-options,
  .product-card.offline .add-to-cart {
    pointer-events: none;
    opacity: 0.5;
  }

  .product-card:hover {
    transform: translateY(-15px) scale(1.02);
    box-shadow: 0 20px 45px rgba(0,255,136,0.25);
  }

  .hs-icon {
    width: 120px;
    height: 120px;
    margin: 0 auto 20px;
    filter: drop-shadow(0 0 10px rgba(0,255,136,0.3));
  }

  .price {
    font-size: 2em;
    color: #00ff88;
    margin: 15px 0;
    text-shadow: 0 0 5px rgba(0,255,136,0.3);
  }

  .plan-options {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin: 25px 0;
  }

  .plan-option {
    background: rgba(0,0,0,0.4);
    padding: 25px 20px;
    border-radius: 18px;
    cursor: pointer;
    transition: all 0.4s;
    border: 2px solid rgba(0,255,136,0.15);
    margin: 12px 0;
    min-height: 100px;
  }

  .plan-option:hover {
    background: rgba(0,255,136,0.15);
    transform: scale(1.05);
    box-shadow: 0 10px 25px rgba(0,255,136,0.25);
  }

  .plan-option.selected {
    background: rgba(0,255,136,0.2);
    border: 2px solid #00ff88;
    box-shadow: 0 0 25px rgba(0,255,136,0.25);
  }

  .plan-option h3 {
    color: #ffffff;
    font-size: 1.5em;
    margin-bottom: 5px;
  }

  .add-to-cart, .payment-button {
    background: linear-gradient(45deg, #00ff88, #00cc6a);
    color: #000;
    border: none;
    padding: 20px 30px;
    border-radius: 35px;
    font-size: 1.3rem;
    cursor: pointer;
    transition: all 0.4s;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 1.5px;
    box-shadow: 0 8px 20px rgba(0,255,136,0.35);
  }

  .add-to-cart:hover, .payment-button:hover {
    transform: scale(1.1);
    box-shadow: 0 15px 30px rgba(0,255,136,0.45);
  }

  .cart-count {
    position: fixed;
    top: 25px;
    right: 25px;
    background: linear-gradient(45deg, #00ff88, #00cc6a);
    color: #000;
    padding: 15px 30px;
    border-radius: 25px;
    font-weight: bold;
    font-size: 1.1rem;
    box-shadow: 0 8px 20px rgba(0,255,136,0.35);
    z-index: 1000;
  }

  .payment-buttons {
    position: fixed;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    gap: 20px;
    z-index: 1000;
  }

  @keyframes pulse {
    0% { transform: scale(1); }
    50% { transform: scale(1.05); }
    100% { transform: scale(1); }
  }

  .added {
    animation: pulse 0.5s ease-in-out;
  }

  .modal {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.8);
    z-index: 2000;
  }

  .modal-content {
    background: linear-gradient(45deg, #1a1a2d, #252542);
    padding: 40px;
    border-radius: 20px;
    max-width: 600px;
    width: 90%;
    border: 3px solid #00ff88;
    box-shadow: 0 15px 35px rgba(0,0,0,0.5);
  }

  .close-modal {
    position: absolute;
    top: 10px;
    right: 15px;
    font-size: 24px;
    cursor: pointer;
    color: #ff6b6b;
  }

  #receiptUpload {
    display: block;
    margin: 20px 0;
    color: #fff;
  }

  .loading {
    display: inline-block;
    width: 20px;
    height: 20px;
    border: 2px solid #00ff88;
    border-radius: 50%;
    border-top-color: transparent;
    animation: spin 1s linear infinite;
  }

  @keyframes spin {
    to {transform: rotate(360deg);}
  }

  .payment-button[style*="background: linear-gradient(45deg, #ff6b6b, #ff5252)"]:hover {
    background: linear-gradient(45deg, #ff5252, #ff3939) !important;
    transform: scale(1.05);
    box-shadow: 0 8px 20px rgba(255,107,107,0.4);
  }

  /* Update mobile-specific button styles */
  .mobile .discord-button, 
  .mobile .rules-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    font-size: 1rem;
    padding: 15px 25px;
    width: 80%;
    max-width: 300px;
    margin: 10px auto;
    border-radius: 30px;
  }

  .mobile .version-btn {
    padding: 12px 20px;
    font-size: 0.9rem;
    border-radius: 25px;
    width: 45%;
    margin: 5px;
  }

  .mobile .add-to-cart {
    width: 100%;
    padding: 16px 20px;
    font-size: 1.1rem;
    border-radius: 30px;
    margin-top: 15px;
  }

  .mobile .payment-button {
    padding: 14px 25px;
    font-size: 1rem;
    border-radius: 25px;
    min-width: 120px;
  }

  .mobile .cart-count {
    padding: 12px 20px;
    font-size: 0.9rem;
    border-radius: 20px;
    right: 10px;
    top: 10px;
  }

  @media screen and (max-width: 480px) {
    .mobile .payment-buttons {
      bottom: 15px;
      width: 100%;
      padding: 0 10px;
    }
    
    .mobile .payment-buttons .payment-button {
      flex: 1;
      min-width: 0;
      padding: 12px 15px;
      font-size: 0.9rem;
    }

    .mobile header {
      padding: 30px 15px;
    }

    .mobile header h1 {
      font-size: 2.5em;
    }

    .mobile header p {
      font-size: 1em;
      padding: 0 15px;
    }
  }

  /* Improve touch targets for mobile */
  .mobile .plan-option {
    padding: 20px 15px;
    margin: 8px 0;
    min-height: 80px;
  }

  .mobile .modal-content {
    width: 95%;
    padding: 25px 15px;
    margin: 10px;
  }

  .mobile .close-modal {
    padding: 15px;
    font-size: 28px;
  }

  /* Additional mobile optimization */
  @media screen and (max-width: 480px) {
    .container {
      padding: 5px;
    }
    
    .product-card {
      flex: 0 0 85%; /* Slightly smaller cards on very small screens */
      padding: 15px;
      margin: 5px;
    }
  }

  /* Desktop/Emulator specific styles */
  body:not(.mobile) .discord-button,
  body:not(.mobile) .rules-button {
    font-size: 1.2rem;
    padding: 18px 35px;
    min-width: 250px;
    border-radius: 35px;
    margin: 15px 20px;
  }

  body:not(.mobile) .version-btn {
    padding: 15px 30px;
    font-size: 1.1rem;
    border-radius: 30px;
    width: auto;
    min-width: 250px;
    margin: 10px;
  }

  body:not(.mobile) .add-to-cart {
    width: 100%;
    padding: 20px 30px;
    font-size: 1.3rem;
    border-radius: 35px;
    margin-top: 20px;
  }

  body:not(.mobile) .payment-button {
    padding: 18px 35px;
    font-size: 1.2rem;
    border-radius: 30px;
    min-width: 180px;
  }

  body:not(.mobile) .cart-count {
    padding: 15px 30px;
    font-size: 1.1rem;
    border-radius: 25px;
  }

  body:not(.mobile) .plan-option {
    padding: 25px 20px;
    margin: 12px 0;
    min-height: 100px;
    cursor: pointer;
    transition: all 0.4s;
  }

  body:not(.mobile) .plan-option h3 {
    font-size: 1.5em;
  }

  body:not(.mobile) .price {
    font-size: 2em;
  }

  /* Adjust container spacing for desktop */
  body:not(.mobile) .container {
    padding: 30px;
    gap: 30px;
  }

  body:not(.mobile) .product-card {
    flex: 0 0 400px;
    padding: 40px;
    margin: 20px;
  }

  /* Make modal buttons bigger on desktop */
  body:not(.mobile) .modal-content button {
    padding: 15px 30px;
    font-size: 1.2rem;
    min-width: 200px;
  }

  /* Improve hover effects for desktop */
  body:not(.mobile) .plan-option:hover {
    transform: scale(1.05);
    box-shadow: 0 10px 25px rgba(0,255,136,0.25);
  }

  body:not(.mobile) .add-to-cart:hover,
  body:not(.mobile) .payment-button:hover {
    transform: scale(1.1);
    box-shadow: 0 15px 30px rgba(0,255,136,0.45);
  }

  /* Adjust header sizes for desktop */
  body:not(.mobile) header h1 {
    font-size: 4.5em;
  }

  body:not(.mobile) header p {
    font-size: 1.4em;
  }

  /* Version selector improvements for desktop */
  body:not(.mobile) .version-selector {
    margin: 30px auto;
    max-width: 800px;
    padding: 20px;
  }

  body:not(.mobile) .version-selector p {
    font-size: 1.2em;
    margin-bottom: 20px;
  }
</style>
</head>
<body>

  <div class="cart-count">Carrinho: <span id="cart-items">0</span></div>
  
  <header>
    <h1>VinizModz&#x1f451;</h1>
    <p>Melhore sua precis&#xe3;o com nossos pacotes exclusivos!</p>
    <a href="https://discord.gg/weZxC2nj" target="_blank" class="discord-button">
      <svg style="width:24px;height:24px;vertical-align:middle;margin-right:8px" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" fill="currentColor">
        <path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057a.082.082 0 0 0 .031.057 19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028c.462-.63.874-1.295 1.226-1.994.021-.041.001-.09-.041-.106a13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.118.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03zM8.02 15.33c-1.183 0-2.157-1.085-2.157-2.419 0-1.333.956-2.419 2.157-2.419 1.21 0 2.176 1.096 2.157 2.42 0 1.333-.956 2.418-2.157 2.418zm7.975 0c-1.183 0-2.157-1.085-2.157-2.419 0-1.333.955-2.419 2.157-2.419 1.21 0 2.176 1.096 2.157 2.42 0 1.333-.946 2.418-2.157 2.418z"/>
      </svg>
      Xit Gr&#xe1;tis
    </a>
    <button class="rules-button" onclick="showRules()">Ver Regras</button>
  </header>

  <div class="version-selector">
    <p>Escolha o modo de visualiza&#xe7;&#xe3;o que melhor se adapta ao seu dispositivo para uma experi&#xea;ncia personalizada</p>
    <button class="version-btn mobile-btn active" onclick="selectVersion(&apos;mobile&apos;)">
      <svg class="version-icon" viewBox="0 0 24 24">
        <path fill="currentColor" d="M17,1.01L7,1C5.9,1,5,1.9,5,3v18c0,1.1,0.9,2,2,2h10c1.1,0,2-0.9,2-2V3C19,1.9,18.1,1.01,17,1.01z M17,19H7V5h10V19z"/>
      </svg>
      Visualiza&#xe7;&#xe3;o Mobile
    </button>
    <button class="version-btn emulator-btn" onclick="selectVersion(&apos;emulator&apos;)">
      <svg class="version-icon" viewBox="0 0 24 24">
        <path fill="currentColor" d="M21,3H3C1.9,3,1,3.9,1,5v14c0,1.1,0.9,2,2,2h18c1.1,0,2-0.9,2-2V5C23,3.9,22.1,3,21,3z M21,19H3V5h18V19z"/>
      </svg>
      Visualiza&#xe7;&#xe3;o Desktop
    </button>
  </div>

  <div class="modal" id="rulesModal">
    <div class="modal-content">
      <span class="close-modal" onclick="closeRules()">&#xd7;</span>
      <h2 style="color: #00ff88; margin-bottom: 20px;">Regras de Uso</h2>
      <ul style="list-style-type: none; line-height: 1.6;">
        <li>1. &#xc9; proibido compartilhar sua conta com outros usu&#xe1;rios</li>
        <li>2. O uso do software &#xe9; de responsabilidade do usu&#xe1;rio</li>
        <li>3. N&#xe3;o h&#xe1; reembolso ap&#xf3;s a compra</li>
        <li>4. Respeite os demais usu&#xe1;rios da comunidade</li>
        <li>5. Reporte qualquer problema diretamente ao admin</li>
      </ul>
    </div>
  </div>

  <div class="modal" id="receiptModal">
    <div class="modal-content">
      <span class="close-modal" onclick="closeReceiptModal()">&#xd7;</span>
      <h2 style="color: #00ff88; margin-bottom: 20px;">Enviar Comprovante</h2>
      <p>Por favor, envie o comprovante do seu pagamento para verifica&#xe7;&#xe3;o.</p>
      <input type="file" accept="image/*" id="receiptUpload" style="margin: 20px 0;">
      <button class="payment-button" onclick="submitReceipt()">Enviar Comprovante</button>
    </div>
  </div>

  <div class="container">
    <div class="product-card">
      <svg class="hs-icon" viewBox="0 0 100 100">
        <circle cx="50" cy="50" r="45" fill="none" stroke="#00ff88" stroke-width="2"/>
        <path d="M35,65 Q50,85 65,65" stroke="#00ff88" fill="none" stroke-width="2"/>
        <circle cx="35" cy="45" r="5" fill="#00ff88"/>
        <circle cx="65" cy="45" r="5" fill="#00ff88"/>
        <rect x="30" y="30" width="40" height="15" rx="7" fill="none" stroke="#00ff88" stroke-width="2"/>
      </svg>
      <h2>Android-HS</h2>
      <div class="plan-options">
        <div class="plan-option" data-price="20" onclick="selectPlan(this)">
          <h3>5 Dias</h3>
          <p class="price">R&#x24; 20,00</p>
        </div>
        <div class="plan-option" data-price="45" onclick="selectPlan(this)">
          <h3>30 Dias</h3>
          <p class="price">R&#x24; 45,00</p>
        </div>
        <div class="plan-option" data-price="70" onclick="selectPlan(this)">
          <h3>Permanente</h3>
          <p class="price">R&#x24; 70,00</p>
        </div>
      </div>
      <button class="add-to-cart" onclick="addToCart()">Adicionar ao Carrinho</button>
    </div>

    <div class="product-card offline">
      <svg class="hs-icon" viewBox="0 0 100 100">
        <circle cx="50" cy="50" r="45" fill="none" stroke="#00ff88" stroke-width="2"/>
        <path d="M35,45 L65,45 L50,75 Z" fill="none" stroke="#00ff88" stroke-width="2"/>
        <circle cx="50" cy="35" r="8" fill="none" stroke="#00ff88" stroke-width="2"/>
        <line x1="50" y1="20" x2="50" y2="30" stroke="#00ff88" stroke-width="2"/>
        <line x1="40" y1="25" x2="60" y2="25" stroke="#00ff88" stroke-width="2"/>
      </svg>
      <h2>Android-Bala-M&#xe1;gica</h2>
      <div class="plan-options">
        <div class="plan-option" data-price="20" onclick="selectPlan(this)">
          <h3>5 Dias</h3>
          <p class="price">R&#x24; 20,00</p>
        </div>
        <div class="plan-option" data-price="45" onclick="selectPlan(this)">
          <h3>30 Dias</h3>
          <p class="price">R&#x24; 45,00</p>
        </div>
        <div class="plan-option" data-price="65" onclick="selectPlan(this)">
          <h3>Permanente</h3>
          <p class="price">R&#x24; 65,00</p>
        </div>
      </div>
      <button class="add-to-cart" onclick="addToCart()">Adicionar ao Carrinho</button>
    </div>
  </div>

  <div class="payment-buttons">
    <button class="payment-button" onclick="viewCart()">Ver Carrinho</button>
    <button class="payment-button" onclick="proceedToPayment()">Pagar</button>
  </div>

<script>let cartItems = 0;
let selectedPrice = 0;
let cartTotal = 0;
let selectedProduct = '';
function selectPlan(element) {
  const productCard = element.closest('.product-card');
  if (!document.body.classList.contains('mobile')) {
    alert('Os painéis para PC/Emulador estão temporariamente indisponíveis devido a uma atualização em andamento. Por favor, tente novamente mais tarde.');
    return;
  }
  if (productCard.classList.contains('offline')) {
    alert('Este produto está temporariamente indisponível devido a uma atualização em andamento. Por favor, tente novamente mais tarde.');
    return;
  }
  document.querySelectorAll('.plan-option').forEach(option => {
    option.classList.remove('selected');
  });
  element.classList.add('selected');
  selectedPrice = parseFloat(element.dataset.price);
  selectedProduct = productCard.querySelector('h2').textContent;
}
function addToCart() {
  const productCard = event.target.closest('.product-card');
  if (!document.body.classList.contains('mobile')) {
    alert('Os painéis para PC/Emulador estão temporariamente indisponíveis devido a uma atualização em andamento. Por favor, tente novamente mais tarde.');
    return;
  }
  if (productCard.classList.contains('offline')) {
    alert('Este produto está temporariamente indisponível devido a uma atualização em andamento. Por favor, tente novamente mais tarde.');
    return;
  }
  if (selectedPrice === 0) {
    alert('Por favor, selecione um plano primeiro!');
    return;
  }
  cartItems++;
  cartTotal += selectedPrice;
  document.getElementById('cart-items').textContent = cartItems;
  const button = event.target;
  button.classList.add('added');
  setTimeout(() => {
    button.classList.remove('added');
  }, 500);
}
function viewCart() {
  if (cartItems === 0) {
    alert('Seu carrinho está vazio!');
  } else {
    closeCartModal();
    const cartModal = document.createElement('div');
    cartModal.id = 'cartModal';
    cartModal.style.cssText = `
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.9);
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 3000;
    `;
    cartModal.addEventListener('click', e => {
      if (e.target === cartModal) {
        closeCartModal();
      }
    });
    const content = document.createElement('div');
    content.style.cssText = `
      background: #1a1a2d;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      border: 2px solid #00ff88;
      max-width: 500px;
      width: 90%;
    `;
    content.innerHTML = `
      <h2 style="color: #00ff88; margin-bottom: 20px;">Seu Carrinho</h2>
      <p style="color: #fff; margin-bottom: 20px;">Total 
