<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kevin S. - Accomplished Flutter Developer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <!-- Lottie Player for dynamic animations -->
    <script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;900&display=swap" rel="stylesheet">
    
    <!-- Chosen Palette: Slate Greys, Teal, and Warm Neutrals -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f9fb; /* Softer background */
            color: #1f2937; /* Darker text for better contrast */
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 500px;
            margin-left: auto;
            margin-right: auto;
            height: 350px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .timeline-item::before {
            content: '';
            position: absolute;
            left: -31px;
            top: 5px;
            width: 16px; /* Smaller, cleaner dot */
            height: 16px;
            border-radius: 50%;
            background-color: #0d9488; /* Teal */
            border: 4px solid #f7f9fb; /* Match background */
            z-index: 10;
            transition: all 0.3s ease;
        }
        /* Custom class for smooth expand/collapse */
        .timeline-details {
            max-height: 0;
            overflow: hidden;
            opacity: 0;
            transition: max-height 0.5s ease-in-out, opacity 0.4s ease-in-out;
        }
        .timeline-details.active {
            max-height: 500px; /* Needs to be larger than content height */
            opacity: 1;
            margin-top: 0.75rem;
        }
        /* Custom button style for gradient/shadow effect */
        .creative-button {
            background-image: linear-gradient(to right, #0d9488, #059669); /* Teal to Emerald gradient */
            box-shadow: 0 4px 15px rgba(13, 148, 136, 0.4);
        }
        .creative-button:hover {
            box-shadow: 0 6px 20px rgba(13, 148, 136, 0.6);
            transform: translateY(-1px);
        }
    </style>
</head>
<body class="antialiased">

    <!-- Sticky Header with Shadow and Blur -->
    <header id="navbar" class="bg-white/90 backdrop-blur-sm shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-black text-teal-700">Kevin S.<span class="text-teal-400">/Dev</span></h1>
            <nav class="hidden md:flex space-x-8">
                <a href="#about" class="text-gray-600 hover:text-teal-600 transition font-medium">About</a>
                <a href="#skills" class="text-gray-600 hover:text-teal-600 transition font-medium">Skills</a>
                <a href="#experience" class="text-gray-600 hover:text-teal-600 transition font-medium">Experience</a>
                <a href="#projects" class="text-gray-600 hover:text-teal-600 transition font-medium">Projects</a>
                <a href="#match" class="text-teal-700 font-extrabold hover:text-teal-500 transition border-b-2 border-teal-500">Match ✨</a>
            </nav>
            <button id="mobile-menu-button" class="md:hidden text-gray-600">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
            </button>
        </div>
        <div id="mobile-menu" class="hidden md:hidden px-6 pb-4 bg-white">
            <a href="#about" class="block py-2 text-gray-600 hover:text-teal-600">About</a>
            <a href="#skills" class="block py-2 text-gray-600 hover:text-teal-600">Skills</a>
            <a href="#experience" class="block py-2 text-gray-600 hover:text-teal-600">Experience</a>
            <a href="#projects" class="block py-2 text-gray-600 hover:text-teal-500">Projects</a>
            <a href="#match" class="block py-2 text-teal-700 font-semibold hover:text-teal-500">Match ✨</a>
        </div>
    </header>

    <main class="container mx-auto px-6 py-12">
        
        <!-- About Section -->
        <section id="about" class="text-center min-h-[60vh] flex flex-col justify-center items-center pt-10 pb-20">
            <div class="p-8 bg-white rounded-xl shadow-xl max-w-4xl w-full">
                <h2 class="text-5xl md:text-6xl font-extrabold text-gray-800 mb-2">Kevin S.</h2>
                <p class="text-xl md:text-3xl font-light text-teal-600 mb-6 tracking-wider">Accomplished Flutter Developer</p>
                <p class="text-lg text-gray-600 mb-8 leading-relaxed">
                    Highly experienced and results-driven **Flutter Developer** with 4+ years of expertise in building robust, cross-platform applications for Android, iOS, Web, and Desktop. Proven ability to design and implement responsive UI/UX that drives engagement, manage the full application lifecycle from concept to successful store deployment, and write clean, well-documented code. Expert in integrating critical third-party tools, APIs, and modern Firebase services.
                </p>
                <div class="flex flex-col sm:flex-row justify-center items-center space-y-3 sm:space-y-0 sm:space-x-8 text-gray-700 font-medium">
                     <a href="mailto:kevinshingala73462@gmail.com" class="hover:text-teal-600 flex items-center space-x-2 transition duration-200">
                        <span class="text-2xl text-teal-500">&#9993;</span>
                        <span>kevinshingala73462@gmail.com</span>
                    </a>
                    <a href="tel:+919601700658" class="hover:text-teal-600 flex items-center space-x-2 transition duration-200">
                        <span class="text-2xl text-teal-500">&#128222;</span>
                        <span>+91 96017 00658</span>
                    </a>
                </div>
            </div>
        </section>

        <!-- Role Match Analyzer (Gemini Feature) -->
        <section id="match" class="py-20 bg-teal-50 rounded-2xl p-8 shadow-2xl my-16">
            <h3 class="text-3xl font-extrabold text-center mb-6 text-teal-700 flex justify-center items-center space-x-3">
                <span>Role Match Analyzer</span>
                <span class="text-4xl">✨</span>
            </h3>
            <p class="text-center text-gray-600 max-w-3xl mx-auto mb-8">
                **Recruiter Assist Mode:** Paste a job description below and our **Gemini AI assistant** will analyze the requirements against Kevin's profile to generate a concise, tailored summary highlighting the strongest relevant skills and experience.
            </p>
            <div class="max-w-4xl mx-auto space-y-4">
                <textarea id="jd-input" rows="7" class="w-full p-4 border border-teal-300 rounded-xl focus:ring-teal-500 focus:border-teal-500 text-gray-700 shadow-inner resize-none" placeholder="Paste the Job Description here (e.g., 'Senior Flutter Developer with deep expertise in Firebase, state management, and deploying large-scale consumer applications...')."></textarea>
                <button id="analyze-button" class="creative-button text-white font-extrabold py-4 rounded-xl transition duration-300 transform w-full flex items-center justify-center">
                    <span id="analyze-text">Analyze Job Match ✨</span>
                    <div id="analyze-loading" class="hidden flex items-center ml-4">
                        <lottie-player id="lottie-analyze" src="https://lottie.host/81f885e3-4d4b-4b2a-8406-38295b9d29e7/L3L853jUeA.json" 
                                background="transparent" speed="1" style="width: 50px; height: 50px;" loop autoplay></lottie-player>
                        <span class="ml-2 text-sm">Analyzing...</span>
                    </div>
                </button>
            </div>
            <div id="match-output-container" class="mt-10 bg-white p-6 rounded-xl shadow-xl hidden border-l-4 border-teal-500">
                <h4 class="text-xl font-bold mb-3 text-gray-800">🎯 Candidate Alignment Summary:</h4>
                <p id="match-output" class="text-gray-700 leading-relaxed"></p>
                <p class="mt-4 text-xs text-gray-500">Analysis powered by Gemini AI.</p>
            </div>
        </section>

        <!-- Technical Expertise Section -->
        <section id="skills" class="py-20">
            <h3 class="text-3xl font-bold text-center mb-12 text-gray-800">Technical Expertise</h3>
             <p class="text-center text-gray-600 max-w-2xl mx-auto mb-16">
                A visual and detailed breakdown of my technical capabilities. The radar chart highlights core competency areas, while the lists specify the key technologies and frameworks used to build high-quality software.
            </p>
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center bg-white p-8 rounded-xl shadow-lg">
                <div class="chart-container">
                    <canvas id="skillsChart"></canvas>
                </div>
                <div class="space-y-6">
                    <div>
                        <h4 class="text-xl font-extrabold mb-2 text-teal-700 border-b pb-1 border-teal-100">Cross-Platform Development</h4>
                        <p class="text-gray-600 font-medium">Flutter, Dart (Android, iOS, Web, Desktop)</p>
                    </div>
                    <div>
                        <h4 class="text-xl font-extrabold mb-2 text-teal-700 border-b pb-1 border-teal-100">Database & State Management</h4>
                        <p class="text-gray-600 font-medium">Offline Database (Sqflite, Hive), Firebase (Authentication, Firestore, Cloud Functions, Notifications)</p>
                    </div>
                    <div>
                        <h4 class="text-xl font-extrabold mb-2 text-teal-700 border-b pb-1 border-teal-100">Networking & Real-time</h4>
                        <p class="text-gray-600 font-medium">REST APIs, Socket Programming, Agora SDK, Google Maps, Razorpay</p>
                    </div>
                    <div>
                        <h4 class="text-xl font-extrabold mb-2 text-teal-700 border-b pb-1 border-teal-100">Backend Experience</h4>
                        <p class="text-gray-600 font-medium">NodeJS, ReactJS, MongoDB, PHP, GOLANG, Laravel, PostgreSQL</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Professional Experience Section -->
        <section id="experience" class="py-20">
            <h3 class="text-3xl font-bold text-center mb-16 text-gray-800">Professional Experience</h3>
            <p class="text-center text-gray-600 max-w-2xl mx-auto mb-12">
                My career path shows a progression of skill and responsibility. Click on any role in the timeline to expand and view specific contributions and achievements.
            </p>
            <div id="timeline-container" class="relative max-w-3xl mx-auto border-l-4 border-teal-300 pl-8 pt-2 pb-4">
            </div>
        </section>

        <!-- Select Projects Section -->
        <section id="projects" class="py-20">
            <h3 class="text-3xl font-bold text-center mb-12 text-gray-800">Select Projects</h3>
             <p class="text-center text-gray-600 max-w-2xl mx-auto mb-12">
                A selection of key projects. Click on any card to learn more and use the "Deep Dive" feature to generate a technical summary.
            </p>
            <div id="projects-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            </div>
        </section>
    </main>

    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-6 text-center">
            <p class="mb-2 text-gray-300">Connect with Kevin:</p>
            <p class="mb-4">
                <a href="mailto:kevinshingala73462@gmail.com" class="hover:text-teal-300 transition">Email</a> | 
                <a href="tel:+919601700658" class="hover:text-teal-300 transition">Phone</a>
            </p>
            <p class="text-xs text-gray-500">&copy; 2024 Kevin S. Built with Flutter & Powered by Gemini AI.</p>
        </div>
    </footer>
    
    <!-- Project Modal -->
    <div id="project-modal" class="fixed inset-0 bg-black bg-opacity-80 z-50 hidden flex justify-center items-center p-4 backdrop-blur-sm">
        <div class="bg-white rounded-2xl shadow-3xl max-w-2xl w-full max-h-[90vh] overflow-y-auto transform scale-95 transition-transform duration-300" id="modal-content">
            <div class="p-8 relative">
                 <button id="close-modal" class="absolute top-4 right-4 text-gray-500 hover:text-gray-800 text-4xl font-light leading-none transition-colors">&times;</button>
                 <h4 id="modal-title" class="text-3xl font-extrabold mb-2 text-teal-700 border-b pb-2 border-teal-100"></h4>
                 <div class="flex flex-wrap items-center text-sm mb-4 space-x-4">
                     <p class="font-semibold text-gray-700">Role: <span id="modal-role" class="font-normal"></span></p>
                 </div>
                 <div id="modal-stack" class="mb-6"></div>
                 <div id="modal-description" class="text-gray-600 space-y-3 leading-relaxed border-t pt-4"></div>
                 
                 <div id="modal-project-link-container" class="mt-4 pt-4 border-t border-gray-200 hidden">
                    <a id="modal-project-link" href="#" target="_blank" class="w-full inline-flex items-center justify-center bg-green-600 text-white font-extrabold py-3 rounded-xl shadow-lg hover:bg-green-700 transition duration-300 space-x-2">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14"></path></svg>
                        <span>View Live Project</span>
                    </a>
                 </div>

                 <!-- Gemini Deep Dive Area -->
                 <div class="mt-8 pt-4 border-t border-gray-200">
                    <button id="deep-dive-button" class="w-full bg-indigo-600 text-white font-extrabold py-3 rounded-xl shadow-lg hover:bg-indigo-700 transition duration-300 flex items-center justify-center space-x-2">
                        <span id="deep-dive-text">Generate Technical Deep Dive ✨</span>
                        <div id="deep-dive-loading" class="hidden flex items-center ml-2">
                             <lottie-player id="lottie-deep-dive" src="https://lottie.host/d193132e-5975-430c-9397-6a2d9a602f9e/u1lV6l75rM.json" 
                                background="transparent" speed="1" style="width: 30px; height: 30px;" loop autoplay></lottie-player>
                             <span class="ml-1 text-sm">Generating...</span>
                        </div>
                    </button>
                    <div id="deep-dive-output-container" class="mt-4 p-5 bg-indigo-50 rounded-xl shadow-inner hidden border-l-4 border-indigo-300">
                        <h5 class="font-extrabold text-indigo-800 mb-2">Technical Insight (AI Generated):</h5>
                        <p id="deep-dive-output" class="text-indigo-900 leading-relaxed"></p>
                    </div>
                 </div>
            </div>
        </div>
    </div>


    <script>
        const apiKey = "";
        const GEMINI_API_URL = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-05-20:generateContent?key=${apiKey}`;

        const RESUME_STATIC_DATA = {
            summary: "Highly experienced and results-driven Flutter Developer with 4+ years of expertise in building robust, cross-platform applications for Android, iOS, Web, and Desktop. Expert in integrating critical third-party tools, REST APIs, Socket Programming, and modern Firebase services (Firestore, Auth, Functions).",
            skills: [
                "Flutter", "Dart", "Firebase", "Firestore", "Sqflite", "Hive", "REST APIs", "Socket Programming", 
                "Agora SDK", "Google Maps", "Razorpay", "Platform Channels", "NodeJS", "ReactJS", "MongoDB", 
                "PHP", "GOLANG", "Laravel", "PostgreSQL", "UI/UX Design"
            ],
            // Project data updated to split WePace into two distinct applications (Customer and Provider)
            projects: [
                { title: "Bill Saathi - Easy Billing App", role: "Sr. Mobile App Developer", stack: "Flutter, Firebase, NodeJS, ReactJS, MongoDB, REST API", link: null, description: ["Led the digital transformation of a non-tech-savvy client's paper-based billing process into an intuitive digital management application.", "Focused heavily on UI/UX design to ensure the application was easy-to-use, resulting in positive customer feedback regarding significant time-saving and operational simplicity.", "Responsible for developing and implementing new features, enhancing the user experience based on customer feedback, and managing application publication on stores."] },
                { title: "PublicNext (iOS)", role: "Core Developer", stack: "Flutter, iOS, PHP, GOLANG", link: null, description: ["Core developer for a regional news application, focusing on real-time content delivery. Implemented key backend-integrated features including Firebase Push Notifications, Contact Syncing, caching, and buffering to ensure optimal performance and user experience."] },
                { title: "SaatBaar Real Estate", role: "Mobile Application Developer / Team Management", stack: "Flutter, NodeJS, ReactJS, MongoDB, REST API, Firebase", link: null, description: ["Developed a comprehensive Real Estate Marketplace connecting property owners, brokers, agents, and advocates.", "Integrated Google Maps API for location-based property listing and search, and Razorpay for in-app payment solutions.", "Contributed to team management alongside development responsibilities."] },
                { title: "Zuooa", role: "App Enhancer & Publication Manager", stack: "Flutter, Laravel, PostgreSQL", link: null, description: ["Enhanced and maintained a multi-vendor/customer application for online ordering from retail shops (similar to Swiggy/Zomato) for the Delhi NCR startup market.", "Managed the end-to-end process of publishing the enhanced application across mobile and web stores."] },
                { title: "WePace Customer App", role: "Application Developer", stack: "Flutter", link: "https://play.google.com/store/apps/details?id=com.wepace.customer", description: ["Developed the customer-facing side of the service marketplace for booking and paying for various services.", "The application focused on user experience for easy service discovery and booking.", "Managed publication of the application to the respective stores."] },
                { title: "WePace Provider App", role: "Application Developer", stack: "Flutter", link: "https://play.google.com/store/apps/details?id=my.wepace.provider", description: ["Developed the provider-facing application for the service marketplace, enabling service professionals to manage appointments, view customer requests, and update their availability and service listings.", "Focused on efficient data synchronization for real-time request handling.", "Managed publication of the application to the respective stores."] }
            ]
        };

        async function fetchWithExponentialBackoff(apiUrl, payload, maxRetries = 5) {
            for (let attempt = 0; attempt < maxRetries; attempt++) {
                try {
                    const response = await fetch(apiUrl, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });

                    if (response.ok) {
                        const result = await response.json();
                        const text = result.candidates?.[0]?.content?.parts?.[0]?.text;
                        if (text) return text;
                    }

                    if (response.status === 429 && attempt < maxRetries - 1) {
                        const delay = Math.pow(2, attempt) * 1000 + Math.random() * 1000;
                        await new Promise(resolve => setTimeout(resolve, delay));
                        continue;
                    }

                    throw new Error(`API failed with status ${response.status}`);
                } catch (error) {
                    if (attempt === maxRetries - 1) throw error;
                    const delay = Math.pow(2, attempt) * 1000 + Math.random() * 1000;
                    await new Promise(resolve => setTimeout(resolve, delay));
                }
            }
        }

        async function generateProjectDeepDive(projectTitle, description) {
            const systemPrompt = "You are a Senior Technical Writer. Given a project title and its high-level description, generate a new paragraph (4-5 sentences max) focusing on the key technical challenges, the specific architecture implemented, or the most impactful result achieved. The tone must be technically insightful and professional.";
            const userQuery = `Project Title: ${projectTitle}. Existing Description: ${description}. Generate a technical deep dive paragraph.`;

            const payload = {
                contents: [{ parts: [{ text: userQuery }] }],
                systemInstruction: { parts: [{ text: systemPrompt }] },
            };

            return fetchWithExponentialBackoff(GEMINI_API_URL, payload);
        }

        async function analyzeJobDescription(jobDescription) {
            const candidateProfile = `
                Candidate Summary: ${RESUME_STATIC_DATA.summary}
                Technical Skills: ${RESUME_STATIC_DATA.skills.join(', ')}
                Relevant Projects (Titles & Key achievements):
                ${RESUME_STATIC_DATA.projects.map(p => `- ${p.title}: ${p.description.join(' ')}`).join('\n')}
            `;

            const systemPrompt = "You are an expert HR Analyst and Career Consultant. Your task is to analyze the provided Job Description (JD) and the Candidate Profile data. Generate a concise, persuasive, single-paragraph summary explaining why the candidate is a strong fit. Mention 2-3 specific technical skills or projects from the candidate's profile that directly align with the JD's requirements. Use a professional and confident tone.";
            const userQuery = `Analyze the following Job Description against the Candidate Profile provided.
            Job Description: ${jobDescription}
            Candidate Profile: ${candidateProfile}
            `;

            const payload = {
                contents: [{ parts: [{ text: userQuery }] }],
                tools: [{ "google_search": {} }],
                systemInstruction: { parts: [{ text: systemPrompt }] },
            };

            return fetchWithExponentialBackoff(GEMINI_API_URL, payload);
        }


        document.addEventListener('DOMContentLoaded', function () {
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            const jdInput = document.getElementById('jd-input');
            const analyzeButton = document.getElementById('analyze-button');
            const analyzeText = document.getElementById('analyze-text');
            const analyzeLoading = document.getElementById('analyze-loading');
            const matchOutputContainer = document.getElementById('match-output-container');
            const matchOutput = document.getElementById('match-output');
            const lottieAnalyze = document.getElementById('lottie-analyze');
            
            const deepDiveButton = document.getElementById('deep-dive-button');
            const deepDiveText = document.getElementById('deep-dive-text');
            const deepDiveLoading = document.getElementById('deep-dive-loading');
            const deepDiveOutputContainer = document.getElementById('deep-dive-output-container');
            const deepDiveOutput = document.getElementById('deep-dive-output');
            const modal = document.getElementById('project-modal');
            const lottieDeepDive = document.getElementById('lottie-deep-dive');
            const modalProjectLinkContainer = document.getElementById('modal-project-link-container');
            const modalProjectLink = document.getElementById('modal-project-link');


            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });
            
            document.querySelectorAll('#mobile-menu a').forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                });
            });

            // --- Skills Radar Chart ---
            const skillsCtx = document.getElementById('skillsChart').getContext('2d');
            new Chart(skillsCtx, {
                type: 'radar',
                data: {
                    labels: ['Flutter & Dart', 'State Management', 'Backend & API', 'Native Integration', 'UI/UX Design', 'Database'],
                    datasets: [{
                        label: 'Proficiency',
                        data: [9, 8, 8, 7, 9, 8],
                        backgroundColor: 'rgba(13, 148, 136, 0.4)', /* More visible fill */
                        borderColor: 'rgba(13, 148, 136, 1)',
                        borderWidth: 3, /* Thicker line */
                        pointBackgroundColor: '#0d9488',
                        pointBorderColor: '#fff',
                        pointHoverBackgroundColor: '#fff',
                        pointHoverBorderColor: '#0d9488'
                    }]
                },
                options: {
                    maintainAspectRatio: false,
                    scales: {
                        r: {
                            angleLines: { color: 'rgba(0, 0, 0, 0.1)' },
                            grid: { color: 'rgba(0, 0, 0, 0.1)' },
                            pointLabels: {
                                font: {
                                    size: 14,
                                    weight: 'bold'
                                },
                                color: '#1f2937'
                            },
                            ticks: {
                                beginAtZero: true,
                                max: 10,
                                stepSize: 2,
                                display: false, /* Hide numeric ticks for cleaner look */
                                backdropColor: 'transparent'
                            }
                        }
                    },
                    plugins: {
                        legend: { display: false },
                        tooltip: { callbacks: { label: (context) => `Level: ${context.raw}/10` } }
                    }
                }
            });

            // --- Experience Timeline Setup ---
            const experienceData = [
                {
                    company: "Freelancer",
                    role: "Sr. Mobile Application Developer",
                    period: "2024 – Present",
                    details: [
                        "Engaged in full-stack mobile development projects, utilizing expertise in Flutter to deliver high-quality, user-friendly applications across various client needs.",
                        "Focused on implementing new features, bug fixing, and performance tuning for existing application improvements."
                    ]
                },
                {
                    company: "PublicNext",
                    role: "Flutter Application Developer (iOS)",
                    period: "2023 – Feb 2024",
                    details: [
                        "Specialized in iOS app development (iPhone and iPad) for a news application targeting the Karnataka audience.",
                        "Implemented complex features, including an in-app video player utilizing Method Channels for native-side implementation (similar to Instagram Reels and Inshot).",
                        "Developed a proprietary Ad publishing module utilizing the Hive Database for local ad caching and delivery, mirroring Google AdMob functionality."
                    ]
                },
                {
                    company: "Artrue Infotech",
                    role: "Flutter Developer",
                    period: "Jan 2021 – Dec 2022",
                    details: [
                        "Worked on various mobile development projects, applying strong foundational skills in Flutter to design and build initial application features."
                    ]
                }
            ];

            const timelineContainer = document.getElementById('timeline-container');
            experienceData.forEach(item => {
                const timelineItem = document.createElement('div');
                timelineItem.className = 'timeline-item mb-10 relative';
                timelineItem.innerHTML = `
                    <div class="cursor-pointer hover:bg-teal-50 p-3 rounded-lg transition duration-200">
                        <h4 class="text-xl font-bold text-gray-800">${item.role}</h4>
                        <p class="font-semibold text-teal-600">${item.company}</p>
                        <p class="text-sm text-gray-500 mb-2">${item.period}</p>
                    </div>
                    <div class="timeline-details pl-4 pt-2 border-l-2 border-gray-100 ml-4">
                        <ul class="list-disc list-inside text-gray-600 space-y-2">
                            ${item.details.map(d => `<li>${d}</li>`).join('')}
                        </ul>
                    </div>
                `;
                timelineItem.querySelector('.cursor-pointer').addEventListener('click', (e) => {
                    const details = e.currentTarget.nextElementSibling;
                    details.classList.toggle('active');
                });
                timelineContainer.appendChild(timelineItem);
            });

            // --- Projects Grid Setup ---
            const projectsData = RESUME_STATIC_DATA.projects;

            const projectsGrid = document.getElementById('projects-grid');
            const closeModal = document.getElementById('close-modal');

            projectsData.forEach(project => {
                const projectCard = document.createElement('div');
                projectCard.className = 'bg-white rounded-xl shadow-lg p-6 cursor-pointer hover:shadow-xl hover:-translate-y-1 transition-all duration-300 border border-gray-100';
                projectCard.innerHTML = `
                    <h4 class="text-xl font-extrabold text-teal-700 mb-2">${project.title}</h4>
                    <div class="mb-4">
                        ${project.stack.split(', ').slice(0, 3).map(s => `<span class="inline-block bg-gray-100 text-gray-600 text-xs font-medium mr-1 px-2 py-0.5 rounded-full">${s}</span>`).join('')}...
                    </div>
                    <p class="text-gray-600">${project.description[0].substring(0, 100)}... <span class="text-teal-500 font-semibold">Read more</span></p>
                `;
                projectCard.addEventListener('click', () => {
                    document.getElementById('modal-title').textContent = project.title;
                    document.getElementById('modal-role').textContent = project.role;
                    document.getElementById('modal-stack').innerHTML = project.stack.split(', ').map(s => `<span class="inline-block bg-teal-100 text-teal-800 text-sm font-medium mr-2 mb-2 px-3 py-1 rounded-full">${s}</span>`).join('');
                    document.getElementById('modal-description').innerHTML = project.description.map(d => `<p>${d}</p>`).join('');
                    
                    // Set current project data for deep dive
                    deepDiveButton.dataset.title = project.title;
                    deepDiveButton.dataset.description = project.description.join(' ');
                    
                    // Handle project link display
                    if (project.link) {
                        modalProjectLink.href = project.link;
                        modalProjectLinkContainer.classList.remove('hidden');
                    } else {
                        modalProjectLinkContainer.classList.add('hidden');
                    }
                    
                    // Reset deep dive area
                    deepDiveOutputContainer.classList.add('hidden');
                    deepDiveOutput.textContent = '';
                    deepDiveText.textContent = 'Generate Technical Deep Dive ✨';
                    deepDiveButton.disabled = false;
                    
                    modal.classList.remove('hidden');
                });
                projectsGrid.appendChild(projectCard);
            });
            
            closeModal.addEventListener('click', () => {
                modal.classList.add('hidden');
            });
            
            modal.addEventListener('click', (e) => {
                if (e.target === modal) {
                    modal.classList.add('hidden');
                }
            });


            // --- Gemini API Logic ---

            analyzeButton.addEventListener('click', async () => {
                const jd = jdInput.value.trim();
                if (jd.length < 50) {
                    matchOutputContainer.classList.remove('hidden');
                    matchOutput.textContent = "Please paste a detailed job description (at least 50 characters) to get a meaningful analysis.";
                    return;
                }

                analyzeButton.disabled = true;
                analyzeText.classList.add('hidden');
                analyzeLoading.classList.remove('hidden');
                matchOutputContainer.classList.remove('hidden');
                matchOutput.textContent = 'Analyzing job requirements and candidate profile...';
                lottieAnalyze.play();

                try {
                    const result = await analyzeJobDescription(jd);
                    matchOutput.textContent = result;
                } catch (error) {
                    matchOutput.textContent = "Analysis failed. A connection error occurred or the API key is missing. Please try again.";
                    console.error("Gemini Analysis Error:", error);
                } finally {
                    analyzeButton.disabled = false;
                    analyzeText.classList.remove('hidden');
                    analyzeLoading.classList.add('hidden');
                    lottieAnalyze.stop();
                }
            });

            deepDiveButton.addEventListener('click', async () => {
                const title = deepDiveButton.dataset.title;
                const description = deepDiveButton.dataset.description;
                
                deepDiveButton.disabled = true;
                deepDiveText.classList.add('hidden');
                deepDiveLoading.classList.remove('hidden');
                deepDiveOutputContainer.classList.remove('hidden');
                deepDiveOutput.textContent = 'Generating technical deep dive...';
                lottieDeepDive.play();


                try {
                    const result = await generateProjectDeepDive(title, description);
                    deepDiveOutput.textContent = result;
                } catch (error) {
                    deepDiveOutput.textContent = "Technical deep dive generation failed. A connection error occurred or the API key is missing.";
                    console.error("Gemini Deep Dive Error:", error);
                } finally {
                    deepDiveButton.disabled = false;
                    deepDiveText.classList.remove('hidden');
                    deepDiveLoading.classList.add('hidden');
                    deepDiveText.textContent = 'Regenerate Deep Dive';
                    lottieDeepDive.stop();
                }
            });
        });
    </script>
</body>
</html>
