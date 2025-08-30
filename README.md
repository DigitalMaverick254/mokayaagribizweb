# mokayaagribizweb
This is my Hakathon Agribusiness website addressing SDG 2 - ZERO HUNGER.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mokaya Agribusiness Solutions</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            @apply bg-gray-50 text-gray-800;
        }
        .hero-bg {
            background-image: url('https://placehold.co/1920x1080/4F46E5/fff?text=Lush+Farm+Field');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }
        .info-section {
            @apply py-16 px-6 sm:px-10 lg:px-20 transition-all duration-500 ease-in-out;
        }
        .info-card {
            @apply bg-white rounded-xl shadow-lg p-8 sm:p-10 transform hover:scale-105 transition-transform duration-300 cursor-pointer;
        }
        .active-card {
            @apply ring-4 ring-green-500/50;
        }
        .content-hidden {
            max-height: 0;
            overflow: hidden;
            opacity: 0;
            padding-top: 0;
            padding-bottom: 0;
        }
        .content-visible {
            max-height: 500px;
            overflow: auto;
            opacity: 1;
        }
    </style>
</head>
<body class="bg-gray-50">

    <!-- Header & Navigation -->
    <header class="bg-white shadow-lg sticky top-0 z-50">
        <nav class="container mx-auto px-4 sm:px-6 lg:px-8 py-4 flex flex-col sm:flex-row justify-between items-center">
            <a href="#" class="text-2xl font-bold text-green-600">AgriSolutions</a>
            <div id="nav-menu" class="hidden sm:flex space-x-4 mt-4 sm:mt-0">
                <a href="#climate" class="text-gray-600 hover:text-green-600 transition-colors duration-300">Climate-Smart</a>
                <a href="#irrigation" class="text-gray-600 hover:text-green-600 transition-colors duration-300">Irrigation</a>
                <a href="#crops" class="text-gray-600 hover:text-green-600 transition-colors duration-300">Drought Crops</a>
                <a href="#fertilizer" class="text-gray-600 hover:text-green-600 transition-colors duration-300">Fertilizer</a>
                <a href="#marketing" class="text-gray-600 hover:text-green-600 transition-colors duration-300">Marketing</a>
            </div>
            <button id="menu-button" class="sm:hidden text-gray-600 hover:text-green-600">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
            </button>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero-bg text-white flex items-center justify-center text-center py-40 sm:py-60">
        <div class="bg-black bg-opacity-40 p-8 sm:p-12 rounded-xl max-w-2xl mx-auto">
            <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight mb-4 leading-tight">Empowering a Greener Future</h1>
            <p class="text-lg sm:text-xl lg:text-2xl font-light mb-8">Modern solutions for sustainable and profitable farming.</p>
            <a href="#climate" class="bg-green-600 hover:bg-green-700 text-white font-semibold py-3 px-8 rounded-full shadow-lg transition-colors duration-300">Explore Solutions</a>
        </div>
    </section>

    <!-- Main Content Sections -->
    <main class="container mx-auto px-4 py-16">

        <!-- Climate-Smart Agriculture Section -->
        <section id="climate" class="info-section">
            <h2 class="text-3xl sm:text-4xl font-bold text-center mb-12 text-green-700">Climate-Smart Agriculture</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="info-card" data-topic="climate-smart">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Regenerative Farming</h3>
                    <p class="text-sm text-gray-600">Focuses on soil health and biodiversity to capture carbon and increase farm resilience.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Regenerative farming is an approach to food and farming systems that regenerates topsoil, increases biodiversity, and improves the water cycle. Practices include no-till farming, cover cropping, and crop rotation to enhance the natural ecosystem.</p>
                    </div>
                </div>
                <!-- Card 2 -->
                <div class="info-card" data-topic="climate-smart">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Agroforestry</h3>
                    <p class="text-sm text-gray-600">Integrating trees and shrubs into crop and animal farming systems for mutual benefits.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Agroforestry can help farmers adapt to climate change by providing shade, reducing soil erosion, and enhancing biodiversity. Trees also provide additional income streams from fruits, nuts, or timber.</p>
                    </div>
                </div>
                <!-- Card 3 -->
                <div class="info-card" data-topic="climate-smart">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Carbon Sequestration</h3>
                    <p class="text-sm text-gray-600">Farming practices that help capture and store atmospheric carbon in the soil.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">By managing soil with practices like adding compost and planting deep-rooted crops, farmers can turn their land into a carbon sink, which is a key part of combating climate change.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Irrigation Section -->
        <section id="irrigation" class="info-section bg-green-50">
            <h2 class="text-3xl sm:text-4xl font-bold text-center mb-12 text-green-700">Efficient Irrigation</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="info-card" data-topic="irrigation">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Drip Systems</h3>
                    <p class="text-sm text-gray-600">Delivering water directly to the plant roots, saving water and increasing efficiency.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Drip irrigation is one of the most efficient ways to water crops. It provides a constant, slow drip of water, which reduces evaporation and allows plants to absorb moisture more effectively, leading to healthier growth and higher yields.</p>
                    </div>
                </div>
                <!-- Card 2 -->
                <div class="info-card" data-topic="irrigation">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Smart Irrigation</h3>
                    <p class="text-sm text-gray-600">Using technology and sensors to automate watering schedules based on real-time data.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Smart irrigation systems use soil moisture sensors and weather data to determine exactly when and how much to water. This prevents overwatering, conserves resources, and reduces the workload for the farmer.</p>
                    </div>
                </div>
                <!-- Card 3 -->
                <div class="info-card" data-topic="irrigation">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Rainwater Harvesting</h3>
                    <p class="text-sm text-gray-600">Collecting and storing rainwater for future use, reducing reliance on conventional sources.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Rainwater harvesting is a simple yet powerful technique. Storing water in tanks or ponds during the rainy season provides a valuable resource during dry periods, making farms more resilient to drought.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Drought-Resistant Crops Section -->
        <section id="crops" class="info-section">
            <h2 class="text-3xl sm:text-4xl font-bold text-center mb-12 text-green-700">Drought-Resistant Crops</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="info-card" data-topic="drought-crops">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Sorghum & Millet</h3>
                    <p class="text-sm text-gray-600">Grain crops that have evolved to thrive in hot, dry climates with minimal water.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Sorghum and millet are "super crops" for dry regions. They have extensive root systems that can find water deep in the soil and a waxy coating on their leaves to reduce water loss. </p>
                    </div>
                </div>
                <!-- Card 2 -->
                <div class="info-card" data-topic="drought-crops">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Cassava & Sweet Potato</h3>
                    <p class="text-sm text-gray-600">Root crops that can produce a harvest even under severe drought conditions.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">These tuber crops store water and nutrients in their roots, making them incredibly hardy. They are a reliable food source in areas where other crops fail due to a lack of rain.</p>
                    </div>
                </div>
                <!-- Card 3 -->
                <div class="info-card" data-topic="drought-crops">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Native Beans & Legumes</h3>
                    <p class="text-sm text-gray-600">Certain bean and legume varieties are adapted to arid environments.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Specific varieties of beans, like Tepary beans and cowpeas, have a high tolerance for drought. They also fix nitrogen in the soil, which benefits the crops planted after them.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Fertilizer Use Section -->
        <section id="fertilizer" class="info-section bg-green-50">
            <h2 class="text-3xl sm:text-4xl font-bold text-center mb-12 text-green-700">Optimizing Fertilizer Use</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="info-card" data-topic="fertilizer">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Soil Testing</h3>
                    <p class="text-sm text-gray-600">Know what your soil needs before you apply any fertilizer.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">A soil test is the most important step in a nutrient management plan. It tells you the exact nutrient levels in your soil and helps you choose the right fertilizer, saving money and preventing environmental pollution.</p>
                    </div>
                </div>
                <!-- Card 2 -->
                <div class="info-card" data-topic="fertilizer">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Organic vs. Synthetic</h3>
                    <p class="text-sm text-gray-600">Understanding the pros and cons of different fertilizer types.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Synthetic fertilizers provide quick, targeted nutrients, but organic options like compost and manure improve soil structure and long-term health. Combining both can create a balanced and sustainable approach.</p>
                    </div>
                </div>
                <!-- Card 3 -->
                <div class="info-card" data-topic="fertilizer">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Application Methods</h3>
                    <p class="text-sm text-gray-600">Applying fertilizer at the right time and in the right way.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Applying fertilizer during the right growth stage of the crop is essential. We will provide information on techniques like banding, side-dressing, and foliar feeding to maximize nutrient uptake and minimize runoff.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Marketing Section -->
        <section id="marketing" class="info-section">
            <h2 class="text-3xl sm:text-4xl font-bold text-center mb-12 text-green-700">Agribusiness Marketing</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="info-card" data-topic="marketing">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Digital Presence</h3>
                    <p class="text-sm text-gray-600">Using websites, social media, and email to connect with consumers.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">A strong digital presence is your farm's new storefront. Use engaging visuals on social media and a clean website to tell your farm's story and showcase your products to a wider audience.</p>
                    </div>
                </div>
                <!-- Card 2 -->
                <div class="info-card" data-topic="marketing">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Direct-to-Consumer Sales</h3>
                    <p class="text-sm text-gray-600">Bypassing middlemen to increase your profit margins.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Selling directly to consumers at farmers' markets, through farm shares, or on an e-commerce platform helps you build direct relationships with your customers and earn more for your hard work.</p>
                    </div>
                </div>
                <!-- Card 3 -->
                <div class="info-card" data-topic="marketing">
                    <h3 class="text-xl font-bold mb-4 text-green-600">Brand Storytelling</h3>
                    <p class="text-sm text-gray-600">Using your farm's history and values to build a loyal customer base.</p>
                    <div class="mt-4 content-hidden transition-all duration-500">
                        <p class="text-gray-700">Consumers want to know where their food comes from. Share your farm's unique story—from your family history to your commitment to sustainable practices—to create an emotional connection and brand loyalty.</p>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white text-center py-8">
        <p class="text-sm">© 2025 Christopher Alvin Mokaya AgriSolutions. All rights reserved.</p>
    </footer>

    <!-- JavaScript for Interactivity -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const infoCards = document.querySelectorAll('.info-card');
            const menuButton = document.getElementById('menu-button');
            const navMenu = document.getElementById('nav-menu');

            // Card click functionality
            infoCards.forEach(card => {
                card.addEventListener('click', () => {
                    const content = card.querySelector('.content-hidden');
                    const isActive = card.classList.contains('active-card');

                    // Close all other cards
                    infoCards.forEach(otherCard => {
                        if (otherCard !== card) {
                            otherCard.classList.remove('active-card');
                            otherCard.querySelector('.content-hidden').classList.remove('content-visible');
                        }
                    });

                    // Toggle the clicked card
                    if (!isActive) {
                        card.classList.add('active-card');
                        content.classList.add('content-visible');
                    } else {
                        card.classList.remove('active-card');
                        content.classList.remove('content-visible');
                    }
                });
            });

            // Mobile menu toggle
            menuButton.addEventListener('click', () => {
                navMenu.classList.toggle('hidden');
                navMenu.classList.toggle('flex-col');
            });
        });
    </script>
</body>
</html>


