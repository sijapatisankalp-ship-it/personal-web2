# personal-web2
this is my personal website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nirdip Sijapati - Civil Engineering Student</title>
    <!-- Load Tailwind CSS --><script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #06b6d4; /* New: Cyan-500 */
            --secondary: #2563eb; /* New: Blue-600 */
            --bg-dark: #1f2937; /* Gray-800 */
            --bg-light: #f9fafb; /* Gray-50 */
        }
        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-light);
            color: #1f2937;
        }
        .section-title {
            position: relative;
            display: inline-block;
            padding-bottom: 0.5rem;
            margin-bottom: 1.5rem;
            font-size: 1.5rem;
            font-weight: 700;
            /* Uses new primary color */
            color: var(--primary); 
        }
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50%;
            height: 4px;
            /* Uses new secondary color */
            background-color: var(--secondary);
            border-radius: 9999px;
        }
        .card {
            background-color: white;
            padding: 1.5rem;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05), 0 10px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        .card:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1), 0 20px 25px rgba(0, 0, 0, 0.15);
        }

        /* Animations for Header */
        @keyframes fadeInSlideUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .animate-name {
            animation: fadeInSlideUp 1s ease-out forwards;
        }

        .animate-header-bg {
            animation: gradientShift 15s ease infinite alternate;
            background-size: 200% 200%; /* Ensure the gradient has room to move */
        }

        /* Initial states */
        .initial-hidden {
            opacity: 0;
        }
    </style>
</head>
<body class="min-h-screen">

    <!-- Header & Hero Section (Updated Gradient: Cyan to Blue) -->
    <header id="main-header" class="bg-gradient-to-r from-cyan-500 to-blue-600 text-white shadow-xl py-12 md:py-20 initial-hidden">
        <div class="max-w-4xl mx-auto px-4 text-center">
            <div class="mb-4">
                <!-- Profile Picture: Increased size to h-28 w-28 and added transition for refresh -->
                <img src="ChatGPT Image Nov 18, 2025, 04_05_58 PM_11zon.jpg" 
                     alt="Nirdip Sijapati Profile Picture"
                     class="h-28 w-28 mx-auto rounded-full object-cover ring-4 ring-white shadow-xl transition duration-300">
            </div>
            <h1 id="nirdip-name" class="text-4xl md:text-5xl font-extrabold tracking-tight mb-2 initial-hidden">
                Nirdip Sijapati
            </h1>
            <p class="text-xl md:text-2xl font-light opacity-90 mb-4 initial-hidden animate-name" style="animation-delay: 0.5s;">
                Civil Engineering Student | Driven by Analysis and Design
            </p>
            <p class="text-sm italic font-medium pt-2 border-t border-cyan-500/50 initial-hidden animate-name" style="animation-delay: 1s;">
                "A champion is a failure who tried one more time"
            </p>
        </div>
    </header>

    <main class="max-w-5xl mx-auto p-4 md:p-8 space-y-12">

        <!-- Personal Info & Social Links --><section class="grid grid-cols-1 md:grid-cols-3 gap-6">
            <div class="card md:col-span-2">
                <h2 class="section-title">About Me</h2>
                <div class="space-y-3 text-gray-700">
                    <p>I am a 19-year-old Bachelors student specializing in Civil Engineering, based in Nepalgunj, Banke.</p>
                    <p>My passion lies in **structure analysis** and **design**, driven by a strong foundation in **analytical thinking** and a proactive **team spirit** approach to complex problem-solving. I am currently in my 1st year, eager to translate theoretical knowledge into practical solutions.</p>
                </div>
                <div class="mt-6 pt-4 border-t">
                    <p class="text-sm text-gray-500">
                        <span class="font-semibold text-cyan-600">Location:</span> Nepalgunj, Banke
                    </p>
                    <p class="text-sm text-gray-500">
                        <!-- Link colors updated -->
                        <span class="font-semibold text-cyan-600">Email:</span> <a href="mailto:nirdipsijapati@gmail.com" class="text-cyan-600 hover:text-cyan-800">nirdipsijapati@gmail.com</a>
                    </p>
                </div>
            </div>

            <!-- Card background updated -->
            <div class="card flex flex-col justify-center items-center p-6 bg-cyan-50/50">
                <h3 class="font-bold text-blue-700 mb-4">Connect with Me</h3>
                <div class="flex flex-col space-y-4 w-full max-w-xs">
                    <a href="https://www.linkedin.com/in/nirdip-sijapati-043a15391/" target="_blank" class="flex items-center justify-center p-3 bg-blue-700 text-white rounded-lg hover:bg-blue-800 transition shadow-md">
                        <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764 0-.974.784-1.764 1.75-1.764 1 0 1.75.79 1.75 1.764 0 .974-.74 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.528-4 0v5.604h-3v-11h3v1.765c1.397-2.35 4-2.585 4-2.585s1.25.109 1.75 1.439v-1.765c0 0 1.75 2.222 1.75 5.604z"/></svg>
                        LinkedIn
                    </a>
                    <a href="https://github.com/sijapatisankalp-ship-it" target="_blank" class="flex items-center justify-center p-3 bg-gray-800 text-white rounded-lg hover:bg-gray-900 transition shadow-md">
                        <svg class="w-5 h-5 mr-2" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.082-.742.083-.727.083-.727 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.492.998.108-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.046.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.873.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.923.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.771-1.587 8.2-6.085 8.2-11.389 0-6.627-5.373-12-12-12z"/></svg>
                        GitHub
                    </a>
                </div>
            </div>
        </section>

        <!-- Skills & Education --><section class="grid grid-cols-1 md:grid-cols-2 gap-6">

            <!-- Skills --><div class="card">
                <h2 class="section-title">Skills & Languages</h2>
                <div class="space-y-4">
                    <!-- Technical --><div>
                        <!-- Tag colors updated -->
                        <h4 class="font-semibold text-cyan-600 mb-2">Technical Capabilities</h4>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-cyan-100 text-cyan-700 text-sm font-medium rounded-full">Mentorship</span>
                            <span class="px-3 py-1 bg-cyan-100 text-cyan-700 text-sm font-medium rounded-full">Surveyer</span>
                        </div>
                    </div>
                    <!-- Soft --><div>
                        <h4 class="font-semibold text-cyan-600 mb-2">Soft Skills</h4>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-green-100 text-green-700 text-sm font-medium rounded-full">Analytical Thinking</span>
                            <span class="px-3 py-1 bg-green-100 text-green-700 text-sm font-medium rounded-full">Team Spirit</span>
                            <span class="px-3 py-1 bg-green-100 text-green-700 text-sm font-medium rounded-full">Communication</span>
                        </div>
                    </div>
                    <!-- Languages --><div>
                        <h4 class="font-semibold text-cyan-600 mb-2">Languages</h4>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-yellow-100 text-yellow-700 text-sm font-medium rounded-full">English</span>
                            <span class="px-3 py-1 bg-yellow-100 text-yellow-700 text-sm font-medium rounded-full">Nepali</span>
                            <span class="px-3 py-1 bg-yellow-100 text-yellow-700 text-sm font-medium rounded-full">Hindi</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Education --><div class="card">
                <h2 class="section-title">Education & Interests</h2>
                <div class="space-y-6">
                    <!-- Education --><div>
                        <!-- Title color updated -->
                        <h4 class="font-semibold text-cyan-600 mb-2">Academic Path</h4>
                        <p class="text-gray-800 font-medium">Bachelors in Civil Engineering</p>
                        <p class="text-sm text-gray-600">Year: 1st Year</p>
                        <p class="text-sm text-gray-500 mt-1 italic">Focused on foundational principles of structural integrity and design.</p>
                    </div>
                    <!-- Hobbies --><div class="pt-4 border-t">
                        <!-- Title color updated -->
                        <h4 class="font-semibold text-cyan-600 mb-2">Interests</h4>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-purple-100 text-purple-700 text-sm font-medium rounded-full">Structure Analysis</span>
                            <span class="px-3 py-1 bg-purple-100 text-purple-700 text-sm font-medium rounded-full">Design</span>
                            <span class="px-3 py-1 bg-purple-100 text-purple-700 text-sm font-medium rounded-full">Travelling</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Form --><section class="max-w-3xl mx-auto py-8">
            <h2 class="section-title text-center mx-auto mb-6">Get In Touch</h2>
            <div class="card bg-gray-50 p-6">
                <form id="contact-form" class="space-y-4">
                    <div>
                        <label for="visitor-name" class="block text-sm font-medium text-gray-700">Your Name</label>
                        <input type="text" id="visitor-name" required class="mt-1 block w-full rounded-lg border-gray-300 shadow-sm focus:border-cyan-500 focus:ring-cyan-500 p-3 border">
                    </div>
                    <div>
                        <label for="visitor-email" class="block text-sm font-medium text-gray-700">Your Email</label>
                        <input type="email" id="visitor-email" required class="mt-1 block w-full rounded-lg border-gray-300 shadow-sm focus:border-cyan-500 focus:ring-cyan-500 p-3 border">
                    </div>
                    <div>
                        <label for="visitor-message" class="block text-sm font-medium text-gray-700">Message</label>
                        <textarea id="visitor-message" rows="4" required class="mt-1 block w-full rounded-lg border-gray-300 shadow-sm focus:border-cyan-500 focus:ring-cyan-500 p-3 border"></textarea>
                    </div>
                    <!-- Button color updated -->
                    <button type="submit" class="w-full py-3 px-4 border border-transparent rounded-lg shadow-md text-sm font-medium text-white bg-cyan-600 hover:bg-cyan-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-cyan-500 transition duration-150">
                        Send Message & Analyze
                    </button>
                </form>

                <!-- Feedback Container colors updated -->
                <div id="feedback-container" class="mt-6 p-4 rounded-lg bg-cyan-100 text-cyan-800 border border-cyan-200 hidden">
                    <p class="font-semibold mb-2">Message Analysis (Simulated):</p>
                    <p id="feedback-message" class="text-sm"></p>
                    <div id="loading-indicator" class="flex items-center space-x-2 hidden mt-2">
                        <!-- Spinner color updated -->
                        <svg class="animate-spin h-5 w-5 text-cyan-600" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
                            <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                            <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
                        </svg>
                        <span>Analyzing message...</span>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer --><footer class="bg-gray-800 text-white py-6 mt-12">
        <div class="max-w-4xl mx-auto px-4 text-center text-sm">
            &copy; <span id="current-year"></span> Nirdip Sijapati. Built with Tailwind CSS.
        </div>
    </footer>

    <script>
        document.getElementById('current-year').textContent = new Date().getFullYear();

        // Animation logic for header and name
        document.addEventListener('DOMContentLoaded', () => {
            const mainHeader = document.getElementById('main-header');
            const nirdipName = document.getElementById('nirdip-name');
            const subtitle = document.querySelector('header p:nth-of-type(1)');
            const quote = document.querySelector('header p:nth-of-type(2)');

            // Remove initial-hidden from header to start background animation
            mainHeader.classList.remove('initial-hidden');
            mainHeader.classList.add('animate-header-bg');

            // Animate name after a short delay
            setTimeout(() => {
                nirdipName.classList.remove('initial-hidden');
                nirdipName.classList.add('animate-name');
            }, 500); // Start name animation after 0.5s

            // Animate subtitle after another delay
            setTimeout(() => {
                subtitle.classList.remove('initial-hidden');
                subtitle.classList.add('animate-name');
            }, 1000); // Start subtitle animation after 1s

            // Animate quote after another delay
            setTimeout(() => {
                quote.classList.remove('initial-hidden');
                quote.classList.add('animate-name');
            }, 1500); // Start quote animation after 1.5s
        });


        const form = document.getElementById('contact-form');
        const feedbackContainer = document.getElementById('feedback-container');
        const feedbackMessage = document.getElementById('feedback-message');
        const loadingIndicator = document.getElementById('loading-indicator');

        // Gemini API Configuration
        const MODEL_NAME = "gemini-2.5-flash-preview-09-2025";
        const API_URL = `https://generativelanguage.googleapis.com/v1beta/models/${MODEL_NAME}:generateContent?key=`;
        const SYSTEM_PROMPT = "You are an AI assistant for a professional portfolio. Your task is to analyze a visitor's contact message and generate a short, structured JSON response suitable for an email subject line and a brief action item for the portfolio owner, Nirdip Sijapati. The tone should be professional and direct.";
        
        // Function to handle the API call with exponential backoff
        async function fetchWithRetry(url, options, retries = 3) {
            for (let i = 0; i < retries; i++) {
                try {
                    const response = await fetch(url, options);
                    if (!response.ok) {
                        // Throw error if response is not ok (e.g., 400, 500)
                        throw new Error(`HTTP error! status: ${response.status}`);
                    }
                    return response;
                } catch (error) {
                    if (i < retries - 1) {
                        const delay = Math.pow(2, i) * 1000 + Math.random() * 1000;
                        await new Promise(resolve => setTimeout(resolve, delay));
                        // console.log(`Retrying API call in ${delay}ms...`); // Silent retry
                    } else {
                        throw error; // Re-throw the error on the last attempt
                    }
                }
            }
        }

        form.addEventListener('submit', async (e) => {
            e.preventDefault();

            const name = document.getElementById('visitor-name').value;
            const email = document.getElementById('visitor-email').value;
            const message = document.getElementById('visitor-message').value;

            feedbackContainer.classList.remove('hidden');
            feedbackContainer.classList.remove('bg-red-100', 'border-red-200');
            feedbackContainer.classList.add('bg-cyan-100', 'border-cyan-200');
            feedbackMessage.textContent = '';
            loadingIndicator.classList.remove('hidden');

            const userQuery = `Visitor Name: ${name}. Visitor Email: ${email}. Message: "${message}"`;

            const payload = {
                contents: [{ parts: [{ text: userQuery }] }],
                systemInstruction: { parts: [{ text: SYSTEM_PROMPT }] },
                generationConfig: {
                    responseMimeType: "application/json",
                    responseSchema: {
                        type: "OBJECT",
                        properties: {
                            summary: {
                                type: "STRING",
                                description: "A concise, professional subject line summarizing the purpose of the visitor's message."
                            },
                            actionItem: {
                                type: "STRING",
                                description: "A brief, suggested next step or category for Nirdip to follow up on (e.g., 'Reply with availability', 'File under networking', 'Request more details')."
                            }
                        },
                        required: ["summary", "actionItem"]
                    }
                },
            };

            try {
                const response = await fetchWithRetry(API_URL, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });
                
                const result = await response.json();
                
                let summaryData = null;
                const jsonText = result.candidates?.[0]?.content?.parts?.[0]?.text;

                if (jsonText) {
                    try {
                        summaryData = JSON.parse(jsonText);
                    } catch (err) {
                        console.error("Failed to parse JSON response:", err);
                        // Fallback to raw text if parsing fails
                        summaryData = {
                            summary: "Analysis Error: Could not parse structured data.",
                            actionItem: jsonText
                        };
                    }
                }

                loadingIndicator.classList.add('hidden');
                
                if (summaryData && summaryData.summary) {
                    feedbackMessage.innerHTML = `
                        <span class="font-bold block">Message Sent Successfully!</span>
                        <hr class="my-2 border-cyan-300/50">
                        <p><strong>Subject Idea:</strong> ${summaryData.summary}</p>
                        <p><strong>Suggested Action:</strong> ${summaryData.actionItem}</p>
                        <p class="text-xs mt-2"><em>This is a simulation. The message has been analyzed but not sent via email.</em></p>
                    `;
                    form.reset();
                } else {
                    throw new Error("API response was empty or malformed.");
                }

            } catch (error) {
                console.error("Error communicating with the API:", error);
                loadingIndicator.classList.add('hidden');
                feedbackContainer.classList.remove('bg-cyan-100', 'border-cyan-200');
                feedbackContainer.classList.add('bg-red-100', 'border-red-200', 'text-red-800');
                feedbackMessage.textContent = 'Sorry, the dynamic analysis failed due to a network or API error. Please check the console for details.';
            }
        });
    </script>
</body>
</html>
