# dramane-portfolio
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DRAMANE OUATTARA | Danseur Interprète & Pédagogue</title>
    <!-- Chargement de Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- FIX: Chargement de Lucide via CDN standard pour éviter l'erreur d'importation de module -->
    <script src="https://unpkg.com/lucide@latest/dist/umd/lucide.js"></script>
    
    <!-- Configuration de la police Inter -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f7f7;
            color: #1f2937;
        }
        /* Style pour les cartes/conteneurs */
        .card {
            background-color: white;
            padding: 1.5rem;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
        }
        .icon-blue {
            stroke: #3b82f6; /* Couleur bleue principale */
        }
    </style>
</head>
<body class="antialiased">

    <!-- Script d'initialisation des icônes Lucide après le chargement du corps -->
    <script>
        // La fonction lucide.createIcons est désormais disponible après le chargement du script UMD
        window.onload = function() {
            // S'assurer que 'lucide' est bien défini et que 'createIcons' existe
            if (typeof lucide !== 'undefined' && lucide.createIcons) {
                lucide.createIcons();
            }
        };
    </script>

    <!-- En-tête / Navigation (Fixe sur le dessus) -->
    <header class="sticky top-0 bg-white shadow-lg z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-extrabold text-[#1f2937] tracking-wider">DRAMANE OUATTARA</h1>
            <nav class="hidden md:flex space-x-6 text-sm font-medium">
                <a href="#accueil" class="text-[#3b82f6] hover:text-[#1d4ed8] transition duration-150">Accueil</a>
                <a href="#repertoire" class="text-gray-600 hover:text-[#3b82f6] transition duration-150">Répertoire</a>
                <a href="#competences" class="text-gray-600 hover:text-[#3b82f6] transition duration-150">Compétences</a>
                <a href="#pedagogie" class="text-gray-600 hover:text-[#3b82f6] transition duration-150">Pédagogie</a>
                <a href="#formation" class="text-gray-600 hover:text-[#3b82f6] transition duration-150">Formation</a>
                <a href="#contact" class="text-gray-600 hover:text-[#3b82f6] transition duration-150">Contact</a>
            </nav>
        </div>
    </header>

    <!-- Contenu Principal -->
    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 md:py-12 space-y-16">

        <!-- 1. Introduction & Bio Artistique -->
        <section id="accueil" class="flex flex-col md:flex-row items-center space-y-8 md:space-y-0 md:space-x-12 pt-10">
            <!-- Colonne de Texte -->
            <div class="md:w-3/5">
                <span class="text-sm font-semibold text-[#3b82f6] uppercase tracking-wider">Danseur Interprète & Pédagogue</span>
                <h2 class="mt-2 text-5xl md:text-6xl font-black leading-tight text-[#1f2937]">
                    L'expression en <span class="text-[#3b82f6]">Mouvement</span>.
                </h2>
                <p class="mt-6 text-lg text-gray-700 leading-relaxed">
                    **Bio Courte :** Issu du parcours INSAAC, Dramane Ouattara est spécialisé en danse contemporaine et afro-contemporaine. Fort d'expériences en tournée internationale (France, Afrique de l'Ouest) avec des compagnies renommées (Irène Tassembedo, Dumanle), il allie une solide formation scénique à des compétences pédagogiques certifiées (CAP), incluant le travail sur le répertoire PINA BAUSCH.
                </p>
                <div class="mt-8 flex space-x-4">
                    <a href="#repertoire" class="bg-[#3b82f6] text-white py-3 px-6 rounded-lg font-bold shadow-md hover:bg-[#1d4ed8] transition duration-300">Voir le Répertoire</a>
                    <a href="#contact" class="bg-gray-200 text-[#1f2937] py-3 px-6 rounded-lg font-bold hover:bg-gray-300 transition duration-300">Contacter</a>
                </div>
            </div>
            <!-- Colonne Image/Média (Placeholder) -->
            <div class="md:w-2/5 w-full">
                <!-- Placeholder pour la Photo / Vidéo principale -->
                <div class="bg-gray-300 rounded-xl overflow-hidden aspect-square flex items-center justify-center shadow-2xl">
                    <img src="https://placehold.co/600x600/3b82f6/ffffff?text=Photo+Principale+%26+Reel" alt="Photo professionnelle de Dramane Ouattara" class="w-full h-full object-cover opacity-80" onerror="this.onerror=null; this.src='https://placehold.co/600x600/3b82f6/ffffff?text=Photo+Principale+%26+Reel';" loading="lazy">
                </div>
            </div>
        </section>

        <!-- 2. Expérience et Répertoire (Galerie de Projets) -->
        <section id="repertoire" class="pt-16">
            <h2 class="text-4xl font-extrabold text-[#1f2937] border-b-4 border-[#3b82f6] pb-2 inline-block">2. Expérience et Répertoire</h2>
            <p class="mt-4 text-lg text-gray-600">Sélection de réalisations clés en tant que danseur interprète, incluant les tournées internationales.</p>

            <div class="mt-10 grid gap-8 md:grid-cols-2 lg:grid-cols-3">

                <!-- Projet 1: DES-ESPOIRS -->
                <div class="card bg-[#f1f5f9]">
                    <h3 class="text-xl font-bold text-[#1f2937]">"DES-ESPOIRS"</h3>
                    <p class="text-sm text-gray-500 mt-1">Tournée en HAUTS-DE-FRANCE (Sept. - Oct. 2025)</p>
                    <ul class="mt-4 text-sm space-y-1 list-disc list-inside text-gray-700">
                        <li>**Rôle :** Danseur Interprète</li>
                        <li>**Style :** Danse contemporaine</li>
                        <li>**Chorégraphe :** IRENE TASSEMBEDO</li>
                        <li>**Compagnie :** Cie Irène Tassembedo/Burkina Faso</li>
                    </ul>
                    <div class="mt-4 text-center">
                        <a href="#" class="text-[#3b82f6] hover:text-[#1d4ed8] font-medium text-sm">Voir la galerie du projet &rarr;</a>
                    </div>
                </div>

                <!-- Projet 2: SACRÉE FORÊT -->
                <div class="card bg-[#f1f5f9]">
                    <h3 class="text-xl font-bold text-[#1f2937]">"SACRÉE FORÊT"</h3>
                    <p class="text-sm text-gray-500 mt-1">Festival FRAGILE, Wuppertal/Allemagne (Sept. 2023)</p>
                    <ul class="mt-4 text-sm space-y-1 list-disc list-inside text-gray-700">
                        <li>**Rôle :** Danseur</li>
                        <li>**Style :** Afro-Contemporain & Cirque</li>
                        <li>**Chorégraphe :** YAO NIKOKO HERMANN</li>
                        <li>**Compagnie :** Cie Dumanle/Côte d'Ivoire</li>
                    </ul>
                    <div class="mt-4 text-center">
                        <a href="#" class="text-[#3b82f6] hover:text-[#1d4ed8] font-medium text-sm">Voir la vidéo de la performance &rarr;</a>
                    </div>
                </div>

                 <!-- Projet 4: Tournée Ouest-Africaine -->
                 <div class="card bg-[#f1f5f9]">
                    <h3 class="text-xl font-bold text-[#1f2937]">Tournée Ouest-Africaine</h3>
                    <p class="text-sm text-gray-500 mt-1">Cotonou, Lomé, Ouaga, Bobo-Dioulasso (Oct. - Nov. 2024)</p>
                    <ul class="mt-4 text-sm space-y-1 list-disc list-inside text-gray-700">
                        <li>**Rôle :** Danseur Interprète</li>
                        <li>**Spectacle :** *« Dans 978 ans »*</li>
                        <li>**Chorégraphe :** NIKOKO Yao</li>
                        <li>**Compagnie :** Cie Dumanle/Côte d'Ivoire</li>
                    </ul>
                    <div class="mt-4 text-center">
                        <a href="#" class="text-[#3b82f6] hover:text-[#1d4ed8] font-medium text-sm">Voir le journal de bord de la tournée &rarr;</a>
                    </div>
                </div>

                <!-- Autres Projets -->
                <div class="card lg:col-span-3 bg-white border border-gray-200">
                    <h3 class="text-xl font-bold text-[#1f2937]">Autres Projets Notables</h3>
                    <div class="mt-4 flex flex-wrap gap-4 text-sm font-medium">
                        <span class="bg-gray-100 text-gray-700 px-3 py-1 rounded-full flex items-center"><i data-lucide="sparkles" class="w-4 h-4 mr-1 text-[#3b82f6]"></i> ECHOS CÉLESTES (Danse Contemporaine)</span>
                        <span class="bg-gray-100 text-gray-700 px-3 py-1 rounded-full flex items-center"><i data-lucide="book-open" class="w-4 h-4 mr-1 text-[#3b82f6]"></i> Fresque d'ouverture FESPACO 2021</span>
                        <span class="bg-gray-100 text-gray-700 px-3 py-1 rounded-full flex items-center"><i data-lucide="castle" class="w-4 h-4 mr-1 text-[#3b82f6]"></i> Comédie Musicale (*« LE VOYAGE D'ELSA »*)</span>
                        <span class="bg-gray-100 text-gray-700 px-3 py-1 rounded-full flex items-center"><i data-lucide="map" class="w-4 h-4 mr-1 text-[#3b82f6]"></i> Danse Traditionnelle (*« BLAHON »*)</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- 3. Compétences Techniques et Formatives -->
        <section id="competences" class="pt-16">
            <h2 class="text-4xl font-extrabold text-[#1f2937] border-b-4 border-[#3b82f6] pb-2 inline-block">3. Compétences Techniques</h2>

            <div class="mt-8 grid gap-8 md:grid-cols-2">

                <!-- Maîtrise des Styles -->
                <div class="card">
                    <h3 class="text-2xl font-semibold text-[#1f2937]">Maîtrise des Styles et Techniques</h3>
                    <ul class="mt-4 space-y-3">
                        <li class="flex items-center space-x-3 text-gray-700">
                            <i data-lucide="footprints" class="w-5 h-5 icon-blue"></i>
                            <span>**Danse Contemporaine** (Niveau Expert - Formation ESMD/INSAAC)</span>
                        </li>
                        <li class="flex items-center space-x-3 text-gray-700">
                            <i data-lucide="flame" class="w-5 h-5 icon-blue"></i>
                            <span>**Danse Afro-Contemporaine** (Niveau Expert - Collaborations Ouest-Africaines)</span>
                        </li>
                        <li class="flex items-center space-x-3 text-gray-700">
                            <i data-lucide="music" class="w-5 h-5 icon-blue"></i>
                            <span>**Jazz Contemporain** (En Perfectionnement - Formation ATELIER H.)</span>
                        </li>
                        <li class="flex items-center space-x-3 text-gray-700">
                            <i data-lucide="drumstick" class="w-5 h-5 icon-blue"></i>
                            <span>**Danse Traditionnelle Ivoirienne** (Expérience *« BLAHON »*)</span>
                        </li>
                    </ul>
                </div>

                <!-- Chorégraphie et Création -->
                <div class="card">
                    <h3 class="text-2xl font-semibold text-[#1f2937]">Chorégraphie et Adaptabilité</h3>
                    <ul class="mt-4 space-y-3">
                        <li class="flex items-center space-x-3 text-gray-700">
                            <i data-lucide="settings-2" class="w-5 h-5 icon-blue"></i>
                            <span>**Outillage Chorégraphique** (Analyse et Construction du Mouvement - Formation UPVA)</span>
                        </li>
                        <li class="flex items-center space-x-3 text-gray-700">
                            <i data-lucide="zap" class="w-5 h-5 icon-blue"></i>
                            <span>**Capacité d'Adaptation** (Expérience : Cirque, Comédie musicale, Théâtre-Danse)</span>
                        </li>
                        <li class="flex items-center space-x-3 text-gray-700">
                            <i data-lucide="book-mark" class="w-5 h-5 icon-blue"></i>
                            <span>**Travail de Répertoire** (Maîtrise du langage PINA BAUSCH - Repertory Lab)</span>
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- 4. Compétences Pédagogiques (Le "CAP" Pédagogue) -->
        <section id="pedagogie" class="pt-16">
            <h2 class="text-4xl font-extrabold text-[#1f2937] border-b-4 border-[#3b82f6] pb-2 inline-block">4. Pédagogie et Transmission</h2>

            <div class="mt-8 grid gap-8 md:grid-cols-3">

                <!-- Diplôme Clé -->
                <div class="card bg-white md:col-span-1 border-l-4 border-[#3b82f6]">
                    <h3 class="text-xl font-bold text-[#1f2937] flex items-center"><i data-lucide="graduation-cap" class="w-5 h-5 icon-blue mr-2"></i> Certification Officielle</h3>
                    <p class="mt-2 text-sm text-gray-700">
                        **Certificat d'Aptitude Pédagogique (CAP)** option DANSE ET CHORÉGRAPHIE (CFPAC/INSAAC).
                    </p>
                </div>

                <!-- Formations en Pédagogie -->
                <div class="card md:col-span-2">
                    <h3 class="text-2xl font-semibold text-[#1f2937]">Formations Spécifiques</h3>
                    <ul class="mt-4 space-y-2 text-gray-700">
                        <li class="flex items-start">
                            <i data-lucide="school" class="w-5 h-5 icon-blue mr-3"></i>
                            <span class="flex-1">***« DANSER, L'art De La Transmission »*** : Formation en pédagogie de la danse (CDC LA TERMITIÈRE).</span>
                        </li>
                        <li class="flex items-start">
                            <i data-lucide="users" class="w-5 h-5 icon-blue mr-3"></i>
                            <span class="flex-1">**Coaching Chorégraphique** : Expertise dans l'accompagnement et l'encadrement des interprètes (Biennale de la Danse).</span>
                        </li>
                    </ul>
                    <p class="mt-4 text-sm font-semibold text-gray-500">
                        *A disposition pour animer des ateliers, des stages d'initiation et des sessions de coaching professionnelles.*
                    </p>
                </div>
            </div>
        </section>

        <!-- 5. Formation Académique & Continue (Nouveauté) -->
        <section id="formation" class="pt-16">
            <h2 class="text-4xl font-extrabold text-[#1f2937] border-b-4 border-[#3b82f6] pb-2 inline-block">5. Formation Académique & Continue</h2>
            
            <div class="mt-8 grid gap-6 sm:grid-cols-2 lg:grid-cols-4">
                 <!-- Formation Continue : Pina Bausch -->
                 <div class="card text-center bg-gray-100 border-t-4 border-yellow-500">
                    <p class="text-lg font-bold text-gray-800">PINA BAUSCH REPERTORY LAB</p>
                    <p class="text-sm mt-1 text-gray-700">Dirigé par anciens danseurs du Tanztheater Wuppertal (Juillet 2024).</p>
                </div>
                <!-- Formation Continue : Écoles des Sables -->
                <div class="card text-center bg-gray-100 border-t-4 border-yellow-500">
                    <p class="text-lg font-bold text-gray-800">ÉCHANGE ÉCOLE DES SABLES</p>
                    <p class="text-sm mt-1 text-gray-700">Résidence & Stage au Sénégal avec Patrick Acogny (Mars 2023).</p>
                </div>
                <!-- Diplômes Académiques -->
                <div class="card text-center bg-gray-100">
                    <p class="text-lg font-bold text-[#3b82f6]">LICENCE PRO & DEAG</p>
                    <p class="text-sm mt-1 text-gray-700">Danse et Chorégraphie (ESMD/INSAAC)</p>
                </div>
                <div class="card text-center bg-gray-100">
                    <p class="text-lg font-bold text-[#3b82f6]">BAC SÉRIE C</p>
                    <p class="text-sm mt-1 text-gray-700">Parcours Scientifique (Lycée Scientifique Yamoussoukro)</p>
                </div>
            </div>
        </section>


        <!-- 6. Contact & Références -->
        <section id="contact" class="pt-16 pb-20">
            <h2 class="text-4xl font-extrabold text-[#1f2937] border-b-4 border-[#3b82f6] pb-2 inline-block">6. Contact & Collaboration</h2>

            <div class="mt-8 grid gap-8 md:grid-cols-3">
                
                <!-- Contact Direct -->
                <div class="card md:col-span-1">
                    <h3 class="text-2xl font-semibold text-[#1f2937] flex items-center"><i data-lucide="send" class="w-6 h-6 icon-blue mr-2"></i> Contact Direct</h3>
                    <ul class="mt-4 space-y-3 text-gray-700">
                        <li class="flex items-center space-x-2">
                            <i data-lucide="mail" class="w-5 h-5 icon-blue"></i>
                            <span>dramaneouattara098@gmail.com</span>
                        </li>
                        <li class="flex items-center space-x-2">
                            <i data-lucide="phone" class="w-5 h-5 icon-blue"></i>
                            <span>+225 07 57 50 96 91 / +225 05 86 54 91 27</span>
                        </li>
                        <li class="flex items-center space-x-2">
                            <i data-lucide="map-pin" class="w-5 h-5 icon-blue"></i>
                            <span>Abidjan Cocody, Côte d'Ivoire</span>
                        </li>
                    </ul>
                    <div class="mt-6">
                        <a href="https:/www.instagram.com/dramo_ouattara/" target="_blank" class="text-white bg-pink-500 hover:bg-pink-600 py-2 px-4 rounded-lg flex items-center justify-center font-bold transition duration-300">
                            <i data-lucide="instagram" class="w-5 h-5 mr-2"></i>
                            @dramo_ouattara
                        </a>
                    </div>
                </div>

                <!-- Références -->
                <div class="card md:col-span-2">
                    <h3 class="text-2xl font-semibold text-[#1f2937] flex items-center"><i data-lucide="user-check" class="w-6 h-6 icon-blue mr-2"></i> Références Clés</h3>
                    <div class="mt-4 space-y-4">
                        <div class="border-b pb-4">
                            <p class="text-lg font-bold text-[#3b82f6]">IRENE TASSEMBEDO</p>
                            <p class="text-sm text-gray-700">Chorégraphe et directrice artistique de l'École de danse IRENE TASSEMBEDO (Burkina Faso)</p>
                            <p class="text-xs text-gray-500 mt-1">Contact disponible sur demande pour les projets professionnels.</p>
                        </div>
                        <div class="pb-2">
                            <p class="text-lg font-bold text-[#3b82f6]">PATRICK ACOGNY</p>
                            <p class="text-sm text-gray-700">Chorégraphe, pédagogue, chercheur et conférencier</p>
                            <p class="text-xs text-gray-500 mt-1">Contact disponible sur demande pour les projets professionnels.</p>
                        </div>
                    </div>
                </div>
            </div>
             <!-- Langues -->
             <div class="mt-8 card bg-white border border-gray-200">
                <h3 class="text-xl font-bold text-[#1f2937] flex items-center"><i data-lucide="globe" class="w-5 h-5 icon-blue mr-2"></i> Langues de travail</h3>
                <p class="mt-2 text-md text-gray-700">
                    **Français** (Langue maternelle / Courant) | **Anglais** (Niveau A2)
                </p>
            </div>
        </section>

    </main>

    <!-- Pied de Page -->
    <footer class="bg-gray-800 text-white py-6 mt-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center text-sm">
            &copy; 2025 Dramane Ouattara. Tous droits réservés. Design par Gemini.
        </div>
    </footer>

</body>
</html>
