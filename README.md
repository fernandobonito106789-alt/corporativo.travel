# corporativo.travel
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Corporativo Travel</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://cdn.jsdelivr.net/npm/swiper@9/swiper-bundle.min.css" rel="stylesheet" />
  <script src="https://cdn.jsdelivr.net/npm/swiper@9/swiper-bundle.min.js"></script>
  <style>
    .fade-in-up {
      opacity: 0;
      transform: translateY(20px);
      animation: fadeInUp 1s forwards;
    }
    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
</head>
<body class="font-sans bg-gray-50 text-gray-800">
  <!-- Header -->
  <header class="bg-blue-900 text-white p-6 shadow-lg fade-in-up">
    <div class="container mx-auto flex justify-between items-center">
      <h1 class="text-3xl font-bold">Corporativo Travel</h1>
      <nav>
        <ul class="flex space-x-6">
          <li><a href="#servicios" class="hover:text-yellow-300 transition">Servicios</a></li>
          <li><a href="#contacto" class="hover:text-yellow-300 transition">Contacto</a></li>
          <li><a href="#aviso" class="hover:text-yellow-300 transition">Aviso de Privacidad</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Slider -->
  <section class="mt-6 fade-in-up">
    <div class="swiper mySwiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide"><img src="https://source.unsplash.com/1600x600/?beach,travel" class="w-full rounded-lg shadow-lg" alt="Viaje 1"></div>
        <div class="swiper-slide"><img src="https://source.unsplash.com/1600x600/?mountains,travel" class="w-full rounded-lg shadow-lg" alt="Viaje 2"></div>
        <div class="swiper-slide"><img src="https://source.unsplash.com/1600x600/?city,travel" class="w-full rounded-lg shadow-lg" alt="Viaje 3"></div>
      </div>
      <!-- Botones navegación -->
      <div class="swiper-button-next"></div>
      <div class="swiper-button-prev"></div>
      <!-- Paginación -->
      <div class="swiper-pagination"></div>
    </div>
  </section>

  <!-- Servicios -->
  <section id="servicios" class="py-16 container mx-auto fade-in-up">
    <h2 class="text-4xl font-bold text-center mb-12">Nuestros Servicios</h2>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      <div class="bg-white rounded-2xl shadow-lg p-6 hover:shadow-2xl transform hover:-translate-y-2 transition">
        <h3 class="text-2xl font-semibold mb-4">Vuelos</h3>
        <p>Reserva tus vuelos nacionales e internacionales con las mejores tarifas.</p>
      </div>
      <div class="bg-white rounded-2xl shadow-lg p-6 hover:shadow-2xl transform hover:-translate-y-2 transition">
        <h3 class="text-2xl font-semibold mb-4">Hoteles</h3>
        <p>Alojamiento de lujo y económico en los mejores destinos turísticos.</p>
      </div>
      <div class="bg-white rounded-2xl shadow-lg p-6 hover:shadow-2xl transform hover:-translate-y-2 transition">
        <h3 class="text-2xl font-semibold mb-4">Paquetes</h3>
        <p>Combina vuelos, hoteles y tours en paquetes diseñados para ti.</p>
      </div>
    </div>
  </section>

  <!-- Contacto -->
  <section id="contacto" class="bg-gray-100 py-16 fade-in-up">
    <div class="container mx-auto text-center">
      <h2 class="text-4xl font-bold mb-6">Contáctanos</h2>
      <p class="mb-4">📞 Teléfono: <strong>7471100298</strong></p>
      <p class="mb-6">📧 Correo: <a href="mailto:corporativo.travelsn@gmail.com" class="text-blue-700">corporativo.travelsn@gmail.com</a></p>
      <a href="mailto:corporativo.travelsn@gmail.com" class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 rounded-lg shadow-lg transition duration-300">Enviar Correo</a>
    </div>
  </section>

  <!-- Aviso de Privacidad -->
  <section id="aviso" class="container mx-auto py-16 fade-in-up">
    <h2 class="text-3xl font-bold mb-4">Aviso de Privacidad</h2>
    <p class="leading-relaxed text-justify">
      En Corporativo Travel, respetamos y protegemos sus datos personales. La información proporcionada será utilizada únicamente para fines relacionados con nuestros servicios de viajes. No compartiremos su información con terceros sin su consentimiento expreso.
    </p>
  </section>

  <!-- Footer -->
  <footer class="bg-blue-900 text-white text-center p-6 mt-12 fade-in-up">
    <p>&copy; 2025 Corporativo Travel. Todos los derechos reservados.</p>
  </footer>

  <!-- Botón flotante de WhatsApp -->
  <a href="https://wa.me/527471100298" target="_blank" 
     class="fixed bottom-20 right-5 bg-green-500 hover:bg-green-600 text-white px-4 py-3 rounded-full shadow-lg transition duration-300 flex items-center space-x-2">
     <span>💬</span>
     <span>WhatsApp</span>
  </a>

  <!-- Botón flotante de llamada -->
  <a href="tel:+527471100298" 
     class="fixed bottom-5 right-5 bg-blue-600 hover:bg-blue-700 text-white px-4 py-3 rounded-full shadow-lg transition duration-300 flex items-center space-x-2">
     <span>📞</span>
     <span>Llamar</span>
  </a>

  <!-- Swiper Script -->
  <script>
    var swiper = new Swiper(".mySwiper", {
      loop: true,
      autoplay: { delay: 4000 },
      pagination: { el: ".swiper-pagination", clickable: true },
      navigation: { nextEl: ".swiper-button-next", prevEl: ".swiper-button-prev" },
    });
  </script>
</body>
</html>
