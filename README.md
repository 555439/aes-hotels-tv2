‎<!DOCTYPE html>
‎<html lang="fr">
‎<head>
‎    <meta charset="UTF-8">
‎    <meta name="viewport" content="width=device-width, initial-scale=1.0">
‎    <title>AES Hotel TV - IPTV Haut Débit Économique pour Hôtels, Restaurants et Bars</title>
‎    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
‎    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css">
‎    <style>
‎        .hero-bg {
‎            background: linear-gradient(135deg, #1e3a8a 0%, #3730a3 100%);
‎        }
‎        .card-hover {
‎            transition: all 0.3s ease;
‎        }
‎        .card-hover:hover {
‎            transform: translateY(-5px);
‎            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
‎        }
‎        .pricing-card {
‎            border: 2px solid transparent;
‎            transition: all 0.3s ease;
‎        }
‎        .pricing-card:hover {
‎            border-color: #f59e0b;
‎            transform: scale(1.05);
‎        }
‎        .pricing-card.featured {
‎            border-color: #f59e0b;
‎            background: linear-gradient(135deg, #fffbeb 0%, #fef3c7 100%);
‎        }
‎        .faq-item {
‎            transition: all 0.3s ease;
‎        }
‎        .faq-content {
‎            max-height: 0;
‎            overflow: hidden;
‎            transition: max-height 0.3s ease;
‎        }
‎        .faq-content.open {
‎            max-height: 200px;
‎        }
‎        .btn-primary {
‎            background: linear-gradient(135deg, #f59e0b 0%, #d97706 100%);
‎            transition: all 0.3s ease;
‎        }
‎        .btn-primary:hover {
‎            background: linear-gradient(135deg, #d97706 0%, #b45309 100%);
‎            transform: translateY(-2px);
‎        }
‎        .floating-whatsapp {
‎            position: fixed;
‎            bottom: 20px;
‎            right: 20px;
‎            background: #25d366;
‎            color: white;
‎            padding: 15px;
‎            border-radius: 50%;
‎            font-size: 24px;
‎            box-shadow: 0 4px 12px rgba(37, 211, 102, 0.4);
‎            z-index: 1000;
‎            animation: pulse 2s infinite;
‎        }
‎        @keyframes pulse {
‎            0% { transform: scale(1); }
‎            50% { transform: scale(1.1); }
‎            100% { transform: scale(1); }
‎        }
‎        .section-divider {
‎            background: linear-gradient(90deg, transparent, #e5e7eb, transparent);
‎            height: 1px;
‎            margin: 4rem 0;
‎        }
‎    </style>
‎</head>
‎<body class="bg-gray-50">
‎    <!-- Navigation -->
‎    <nav class="bg-white shadow-lg sticky top-0 z-50">
‎        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
‎            <div class="flex justify-between h-16">
‎                <div class="flex items-center">
‎                    <div class="flex-shrink-0 flex items-center">
‎                        <i class="fas fa-tv text-3xl text-blue-600 mr-3"></i>
‎                        <span class="text-xl font-bold text-gray-900">AES Hotel TV</span>
‎                    </div>
‎                </div>
‎                <div class="hidden md:flex items-center space-x-8">
‎                    <a href="#accueil" class="text-gray-700 hover:text-blue-600 px-3 py-2 rounded-md text-sm font-medium">Accueil</a>
‎                    <a href="#avantages" class="text-gray-700 hover:text-blue-600 px-3 py-2 rounded-md text-sm font-medium">Avantages</a>
‎                    <a href="#forfaits" class="text-gray-700 hover:text-blue-600 px-3 py-2 rounded-md text-sm font-medium">Forfaits</a>
‎                    <a href="#contact" class="text-gray-700 hover:text-blue-600 px-3 py-2 rounded-md text-sm font-medium">Contact</a>
‎                    <a href="https://wa.me/22679949312" class="bg-green-500 text-white px-4 py-2 rounded-lg hover:bg-green-600 transition-colors">
‎                        <i class="fab fa-whatsapp mr-2"></i>WhatsApp
‎                    </a>
‎                </div>
‎                <div class="md:hidden flex items-center">
‎                    <button id="mobile-menu-btn" class="text-gray-700 hover:text-blue-600">
‎                        <i class="fas fa-bars text-xl"></i>
‎                    </button>
‎                </div>
‎            </div>
‎        </div>
‎        <div id="mobile-menu" class="md:hidden hidden bg-white border-t">
‎            <div class="px-2 pt-2 pb-3 space-y-1">
‎                <a href="#accueil" class="block px-3 py-2 text-gray-700 hover:bg-gray-100">Accueil</a>
‎                <a href="#avantages" class="block px-3 py-2 text-gray-700 hover:bg-gray-100">Avantages</a>
‎                <a href="#forfaits" class="block px-3 py-2 text-gray-700 hover:bg-gray-100">Forfaits</a>
‎                <a href="#contact" class="block px-3 py-2 text-gray-700 hover:bg-gray-100">Contact</a>
‎                <a href="https://wa.me/22679949312" class="block px-3 py-2 text-green-600 hover:bg-gray-100">WhatsApp</a>
‎            </div>
‎        </div>
‎    </nav>
‎
‎    <!-- Hero Section -->
‎    <section id="accueil" class="hero-bg text-white py-20">
‎        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
‎            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
‎                <div>
‎                    <h1 class="text-4xl md:text-5xl font-bold mb-6">
‎                        AES Hotel TV – IPTV Haut Débit Économique pour Hôtels, Restaurants et Bars
‎                    </h1>
‎                    <p class="text-xl mb-8 text-blue-100">
‎                        Économisez jusqu'à 70% sur vos abonnements TV grâce à notre solution IPTV stable, fiable et abordable !
‎                    </p>
‎                    <div class="flex flex-col sm:flex-row gap-4">
‎                        <a href="#forfaits" class="btn-primary text-white px-8 py-3 rounded-lg font-semibold inline-flex items-center justify-center">
‎                            <i class="fas fa-shopping-cart mr-2"></i>
‎                            Choisissez Votre Forfait
‎                        </a>
‎                        <a href="https://wa.me/22679949312" class="bg-green-500 text-white px-8 py-3 rounded-lg font-semibold hover:bg-green-600 transition-colors inline-flex items-center justify-center">
‎                            <i class="fab fa-whatsapp mr-2"></i>
‎                            Discutez avec Nous
‎                        </a>
‎                    </div>
‎                </div>
‎                <div class="lg:text-right">
‎                    <img src="https://noniussolutions.com/wp-content/uploads/2025/03/Solutions_TV_Header_google-label.jpg" alt="IPTV Hotel Solution" class="rounded-lg shadow-2xl w-full max-w-lg mx-auto">
‎                </div>
‎            </div>
‎        </div>
‎    </section>
‎
‎    <!-- Avantages Section -->
‎    <section id="avantages" class="py-20 bg-white">
‎        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
‎            <div class="text-center mb-16">
‎                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
‎                    Pourquoi Choisir AES Hotel TV ?
‎                </h2>
‎                <p class="text-xl text-gray-600">
‎                    Découvrez nos avantages concurrentiels pour votre établissement
‎                </p>
‎            </div>
‎            
‎            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
‎                <div class="text-center p-6 bg-gray-50 rounded-lg card-hover">
‎                    <div class="bg-blue-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
‎                        <i class="fas fa-hd-video text-2xl text-blue-600"></i>
‎                    </div>
‎                    <h3 class="text-xl font-semibold text-gray-900 mb-2">Stabilité et Qualité HD/FHD</h3>
‎                    <p class="text-gray-600">Diffusion stable en haute définition pour une expérience client exceptionnelle</p>
‎                </div>
‎                
‎                <div class="text-center p-6 bg-gray-50 rounded-lg card-hover">
‎                    <div class="bg-green-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
‎                        <i class="fas fa-dollar-sign text-2xl text-green-600"></i>
‎                    </div>
‎                    <h3 class="text-xl font-semibold text-gray-900 mb-2">Économique vs. Satellite</h3>
‎                    <p class="text-gray-600">Réduisez vos coûts TV jusqu'à 70% par rapport aux solutions satellite traditionnelles</p>
‎                </div>
‎                
‎                <div class="text-center p-6 bg-gray-50 rounded-lg card-hover">
‎                    <div class="bg-purple-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
‎                        <i class="fas fa-headset text-2xl text-purple-600"></i>
‎                    </div>
‎                    <h3 class="text-xl font-semibold text-gray-900 mb-2">Support Technique 24/7</h3>
‎                    <p class="text-gray-600">Assistance technique disponible 24h/24 et 7j/7 pour garantir votre tranquillité</p>
‎                </div>
‎                
‎                <div class="text-center p-6 bg-gray-50 rounded-lg card-hover">
‎                    <div class="bg-orange-100 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
‎                        <i class="fas fa-mobile-alt text-2xl text-orange-600"></i>
‎                    </div>
‎                    <h3 class="text-xl font-semibold text-gray-900 mb-2">Compatibilité Smart TV</h3>
‎                    <p class="text-gray-600">Compatible avec WebOS, Android TV et Box Android pour toutes vos installations</p>
‎                </div>
‎            </div>
‎        </div>
‎    </section>
‎
‎    <!-- Images Gallery Section -->
‎    <section class="py-20 bg-gray-50">
‎        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
‎            <div class="text-center mb-16">
‎                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
‎                    Nos Solutions en Images
‎                </h2>
‎                <p class="text-xl text-gray-600">
‎                    Découvrez comment nos solutions IPTV transforment l'expérience de vos clients
‎                </p>
‎            </div>
‎            
‎            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
‎                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
‎                    <img src="https://hibox.tv/shared/images/smartroom/hospitality-tv-smartroom-ui.jpg" alt="Interface IPTV Hôtel" class="w-full h-48 object-cover">
‎                    <div class="p-6">
‎                        <h3 class="text-xl font-semibold text-gray-900 mb-2">Interface Hôtel Moderne</h3>
‎                        <p class="text-gray-600">Interface intuitive et élégante spécialement conçue pour l'hôtellerie</p>
‎                    </div>
‎                </div>
‎                
‎                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
‎                    <img src="https://timelineproav.com/wp-content/uploads/2023/08/Sport-Bar-cop-2-2.jpg" alt="Bar Restaurant TV" class="w-full h-48 object-cover">
‎                    <div class="p-6">
‎                        <h3 class="text-xl font-semibold text-gray-900 mb-2">Solutions Bar & Restaurant</h3>
‎                        <p class="text-gray-600">Parfait pour les bars et restaurants avec diffusion multi-écrans</p>
‎                    </div>
‎                </div>
‎                
‎                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
‎                    <img src="https://www.tanixtvbox.com/wp-content/uploads/2025/05/Set-up-Android-TV-Box-1024x666.webp" alt="Android TV Box Setup" class="w-full h-48 object-cover">
‎                    <div class="p-6">
‎                        <h3 class="text-xl font-semibold text-gray-900 mb-2">Box Android Incluse</h3>
‎                        <p class="text-gray-600">Installation simple avec notre box Android pour TV non-smart</p>
‎                    </div>
‎                </div>
‎                
‎                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
‎                    <img src="https://www.netup.tv/assets/img/iptv/imgBlockTV.png" alt="Hotel TV IPTV" class="w-full h-48 object-cover">
‎                    <div class="p-6">
‎                        <h3 class="text-xl font-semibold text-gray-900 mb-2">Télévision Hôtel Premium</h3>
‎                        <p class="text-gray-600">Qualité professionnelle pour une expérience client exceptionnelle</p>
‎                    </div>
‎                </div>
‎                
‎                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
‎                    <img src="https://www.mdmcommercial.com/wp-content/uploads/2023/12/Lifestyle_Hospitality_ProCen-Smart.jpg" alt="Smart TV Hospitality" class="w-full h-48 object-cover">
‎                    <div class="p-6">
‎                        <h3 class="text-xl font-semibold text-gray-900 mb-2">Smart TV Hôtellerie</h3>
‎                        <p class="text-gray-600">Solutions adaptées aux besoins spécifiques de l'hôtellerie</p>
‎                    </div>
‎                </div>
‎                
‎                <div class="bg-white rounded-lg shadow-md overflow-hidden card-hover">
‎                    <img src="https://cdnwww.armembededsystem.com/wp-content/uploads/2023/06/Hospitality_1.jpg" alt="Hospitality IPTV Solution" class="w-full h-48 object-cover">
‎                    <div class="p-6">
‎                        <h3 class="text-xl font-semibold text-gray-900 mb-2">Solution Complète</h3>
‎                        <p class="text-gray-600">Écosystème complet pour tous vos besoins TV professionnels</p>
‎                    </div>
‎                </div>
‎            </div>
‎        </div>
‎    </section>
‎
‎    <!-- Section Divider -->
‎    <div class="section-divider"></div>
‎
‎    <!-- Forfaits Section -->
‎    <section id="forfaits" class="py-20 bg-white">
‎        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
‎            <div class="text-center mb-16">
‎                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
‎                    Nos Forfaits IPTV
‎                </h2>
‎                <p class="text-xl text-gray-600">
‎                    Choisissez le forfait qui correspond le mieux à vos besoins
‎                </p>
‎            </div>
‎            
‎            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-12">
‎                <!-- Hôtel Standard -->
‎                <div class="pricing-card bg-white rounded-lg shadow-lg p-8">
‎                    <div class="text-center mb-6">
‎                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Hôtel Standard</h3>
‎                        <p class="text-gray-600">Parfait pour les petits établissements</p>
‎                    </div>
‎                    <div class="mb-6">
‎                        <div class="flex justify-between items-center mb-2">
‎                            <span class="text-lg font-semibold">6 Mois</span>
‎                            <span class="text-2xl font-bold text-blue-600">15 000 FCFA</span>
‎                        </div>
‎                        <div class="flex justify-between items-center">
‎                            <span class="text-lg font-semibold">12 Mois</span>
‎                            <span class="text-2xl font-bold text-blue-600">20 000 FCFA</span>
‎                        </div>
‎                    </div>
‎                    <ul class="space-y-2 mb-6">
‎                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i>Chaînes essentielles</li>
‎                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i>Qualité HD</li>
‎                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i>Support technique</li>
‎                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i>Installation comprise</li>
‎                    </ul>
‎                    <a href="#contact" class="w-full bg-blue-600 text-white py-3 px-6 rounded-lg font-semibold hover:bg-blue-700 transition-colors block text-center">
‎                        Choisir ce forfait
‎                    </a>
‎                </div>
‎                
‎                <!-- Essentiel Pro -->
‎                <div class="pricing-card featured bg-white rounded-lg shadow-lg p-8 relative">
‎                    <div class="absolute top-0 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-yellow-500 text-white px-4 py-1 rounded-full text-sm font-semibold">
‎                        POPULAIRE
‎                    </div>
‎                    <div class="text-center mb-6">
‎                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Essentiel Pro</h3>
‎                        <p class="text-gray-600">Idéal pour les établissements moyens</p>
‎                    </div>
‎                    <div class="mb-6">
‎                        <div class="flex justify-between items-center mb-2">
‎                            <span class="text-lg font-semibold">6 Mois</span>
‎                            <span class="text-2xl font-bold text-yellow-600">18 500 FCFA</span>
‎                        </div>
‎                        <div class="flex justify-between items-center">
‎                            <span class="text-lg font-semibold">12 Mois</span>
‎                            <span class="text-2xl font-bold text-yellow-600">35 000 FCFA</span>
‎                        </div>
‎                    </div>
‎                    <ul class="space-y-2 mb-6">
‎                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i>Chaînes étendues</li>
‎                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i>Qualité HD/FHD</li>
‎                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i>Support prioritaire</li>
‎                        <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i>Chaînes sport</li>
‎                    </ul>
‎                    <a href="#contact" class="w-full btn-primary text-white py-3 px-6 rounded-lg font-semibold block text-center">
‎                        Choisir ce forfait
‎                    </a>
‎                </div>
‎                
‎                <!-- VIP Premium -->
‎                <div class="pricing-card bg-white rounded-lg shadow-lg p-8">
‎                    <div class="text-center mb-6">
‎                        <h3 class="text-2xl font-bold text-gray-900 mb-2">VIP Premium</h3>
‎                        <p class="text-gray-600">Pour les grands établissements</p>
‎                    </div>
‎                    <div class="mb-6">
‎                        <div class="flex justify-between items-center mb-2">
‎                            <span class="text-lg font-semibold">6 Mois</span>
‎                            <span class="text-2xl font-bold text-purple-600">20 000 FCFA</span>
‎                        </div>
‎                        <div class="flex justify-between items-center mb-2">
‎                            <span class="text-lg font-semibold">12 Mois</span>
‎                            <span class="text-2xl font-bold text-purple-600">40 000 FCFA</span>
‎                        </div>
‎                        <div class="flex justify-between items-center">
‎                            <span class="text-lg font-semibold">Lifetime</span>
‎                            <span class="text-2xl font-bold text-purple-600">100 000 FCFA</span>
‎                        </div>
‎                    </div>
‎                    <ul class="space-y-2 mb-6">
‎                        <li c
