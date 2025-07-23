<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Al-Majlis Al-Raqami | Key Features</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700&display=swap');
        
        :root {
            --uae-red: #ef233c;
            --uae-green: #00732f;
            --uae-black: #000000;
            --uae-white: #ffffff;
            --gold: #d4af37;
        }
        
        body {
            font-family: 'Tajawal', sans-serif;
            scroll-behavior: smooth;
        }
        
        .arabic {
            font-family: 'Tajawal', sans-serif;
            direction: rtl;
        }
        
        .hero-pattern {
            background-color: #ffffff;
            background-image: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23d4af37' fill-opacity='0.1'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
        }
        
        .feature-card {
            transition: all 0.3s ease;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        
        .calligraphy-bg {
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='400' height='200' viewBox='0 0 400 200'%3E%3Cpath fill='none' stroke='%23d4af37' stroke-width='1.5' d='M20,50 C80,30 100,100 160,80 C220,60 240,120 300,100 C360,80 380,140 380,140'/%3E%3Cpath fill='none' stroke='%23d4af37' stroke-width='1.5' d='M20,100 C80,80 100,150 160,130 C220,110 240,170 300,150 C360,130 380,190 380,190'/%3E%3C/svg%3E");
            background-repeat: no-repeat;
            background-position: center;
            background-size: cover;
        }
        
        .btn-primary {
            background-color: var(--uae-green);
            color: white;
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            background-color: #005a25;
            transform: translateY(-2px);
        }
        
        .btn-secondary {
            background-color: var(--uae-red);
            color: white;
            transition: all 0.3s ease;
        }
        
        .btn-secondary:hover {
            background-color: #d01e34;
            transform: translateY(-2px);
        }
        
        .gold-accent {
            color: var(--gold);
        }
        
        .tab-active {
            border-bottom: 3px solid var(--uae-green);
            color: var(--uae-green);
        }
        
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        
        ::-webkit-scrollbar-thumb {
            background: var(--uae-green);
            border-radius: 10px;
        }
        
        ::-webkit-scrollbar-thumb:hover {
            background: #004a1f;
        }
        
        /* Animation */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .animate-fadeIn {
            animation: fadeIn 0.8s ease forwards;
        }
        
        .delay-100 { animation-delay: 0.1s; }
        .delay-200 { animation-delay: 0.2s; }
        .delay-300 { animation-delay: 0.3s; }
        .delay-400 { animation-delay: 0.4s; }
        .delay-500 { animation-delay: 0.5s; }
        
        /* Feature demo animation */
        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.7; }
        }
        
        .animate-pulse {
            animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
        }
        
        /* Progress bar animation */
        @keyframes progress {
            0% { width: 0%; }
            100% { width: 100%; }
        }
        
        .progress-animation {
            animation: progress 3s ease-in-out forwards;
        }
        
        /* Feature tabs */
        .feature-tab {
            transition: all 0.3s ease;
        }
        
        .feature-tab.active {
            background-color: var(--uae-green);
            color: white;
            border-color: var(--uae-green);
        }
        
        .feature-content {
            display: none;
        }
        
        .feature-content.active {
            display: block;
            animation: fadeIn 0.5s ease forwards;
        }
        
        /* Tooltip */
        .tooltip {
            position: relative;
            display: inline-block;
        }
        
        .tooltip .tooltip-text {
            visibility: hidden;
            width: 200px;
            background-color: #333;
            color: #fff;
            text-align: center;
            border-radius: 6px;
            padding: 8px;
            position: absolute;
            z-index: 1;
            bottom: 125%;
            left: 50%;
            margin-left: -100px;
            opacity: 0;
            transition: opacity 0.3s;
        }
        
        .tooltip:hover .tooltip-text {
            visibility: visible;
            opacity: 1;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-md fixed w-full z-10">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <div class="flex items-center">
                    <!-- UAE-inspired logo -->
                    <svg class="h-10 w-10 mr-2" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
                        <rect x="0" y="0" width="100" height="25" fill="#ef233c" />
                        <rect x="0" y="25" width="100" height="25" fill="#ffffff" />
                        <rect x="0" y="50" width="100" height="25" fill="#00732f" />
                        <rect x="0" y="75" width="100" height="25" fill="#000000" />
                        <circle cx="50" cy="50" r="20" fill="#d4af37" opacity="0.8" />
                        <path d="M40,50 Q50,35 60,50 T80,50" stroke="#ffffff" stroke-width="2" fill="none" />
                    </svg>
                    <div>
                        <h1 class="text-xl font-bold text-gray-800">Al-Majlis Al-Raqami</h1>
                        <p class="text-sm text-gray-600">The Digital Majlis</p>
                    </div>
                </div>
            </div>
            <div class="hidden md:flex space-x-8 items-center">
                <a href="#" class="text-gray-700 hover:text-green-700 transition">Home</a>
                <a href="#" class="text-green-700 font-medium">Features</a>
                <a href="#" class="text-gray-700 hover:text-green-700 transition">About</a>
                <a href="#" class="text-gray-700 hover:text-green-700 transition">Contact</a>
                <button id="download-app" class="bg-green-700 text-white px-4 py-2 rounded-md hover:bg-green-800 transition">
                    Download App
                </button>
            </div>
            <div class="md:hidden">
                <button id="menu-toggle" class="text-gray-700 focus:outline-none">
                    <svg class="h-6 w-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t">
            <div class="container mx-auto px-4 py-2 space-y-3">
                <a href="#" class="block text-gray-700 hover:text-green-700 transition py-2">Home</a>
                <a href="#" class="block text-green-700 font-medium py-2">Features</a>
                <a href="#" class="block text-gray-700 hover:text-green-700 transition py-2">About</a>
                <a href="#" class="block text-gray-700 hover:text-green-700 transition py-2">Contact</a>
                <button id="download-app-mobile" class="w-full bg-green-700 text-white px-4 py-2 rounded-md hover:bg-green-800 transition">
                    Download App
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="pt-24 pb-16 bg-cover bg-center">
        <div class="container mx-auto px-4">
            <div class="max-w-4xl mx-auto text-center animate-fadeIn opacity-0">
                <h1 class="text-4xl md:text-5xl font-bold mb-6 text-gray-800">
                    Powerful <span class="text-green-700">Features</span> for Civic Engagement
                </h1>
                <p class="text-xl mb-8 text-gray-600">
                    Al-Majlis Al-Raqami combines traditional consultative values with modern technology to create an inclusive platform for all UAE citizens and residents.
                </p>
                <div class="flex flex-wrap justify-center gap-4">
                    <a href="#submission" class="px-6 py-2 bg-green-700 text-white rounded-full hover:bg-green-800 transition">Voice & Text Submission</a>
                    <a href="#tracking" class="px-6 py-2 bg-green-100 text-green-800 rounded-full hover:bg-green-200 transition">Issue Tracking</a>
                    <a href="#announcements" class="px-6 py-2 bg-green-100 text-green-800 rounded-full hover:bg-green-200 transition">Announcements</a>
                    <a href="#directory" class="px-6 py-2 bg-green-100 text-green-800 rounded-full hover:bg-green-200 transition">Representative Directory</a>
                    <a href="#knowledge" class="px-6 py-2 bg-green-100 text-green-800 rounded-full hover:bg-green-200 transition">Knowledge Hub</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Feature Overview -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="max-w-5xl mx-auto">
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <div class="col-span-1 md:col-span-3">
                        <div class="bg-green-50 rounded-xl p-6 border border-green-100 animate-fadeIn opacity-0 bg-cover bg-center" style="background-image: url('https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/4f8c50d4-7e0e-440e-acc3-328311bed1ed.png'); background-blend-mode: overlay;">
                            <div class="flex items-center mb-4">
                                <div class="w-12 h-12 bg-green-100 rounded-full flex items-center justify-center mr-4">
                                    <svg class="w-6 h-6 text-green-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                    </svg>
                                </div>
                                <div>
                                    <h2 class="text-2xl font-bold text-gray-800">What Makes Al-Majlis Al-Raqami Special?</h2>
                                    <p class="text-gray-600">A modern approach to the traditional Majlis concept</p>
                                </div>
                            </div>
                            <p class="text-gray-700 mb-4">
                                Al-Majlis Al-Raqami brings the traditional consultative Majlis into the digital age, creating a direct channel between citizens and government. Our platform combines the best of UAE's cultural heritage with modern technology to foster inclusive civic engagement.
                            </p>
                            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 mt-6">
                                <div class="bg-white p-4 rounded-lg border border-green-100 flex items-center">
                                    <div class="w-10 h-10 bg-green-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-green-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h3 class="font-medium text-gray-800">Real-time Updates</h3>
                                        <p class="text-sm text-gray-600">Track your submissions instantly</p>
                                    </div>
                                </div>
                                <div class="bg-white p-4 rounded-lg border border-green-100 flex items-center">
                                    <div class="w-10 h-10 bg-green-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-green-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5h12M9 3v2m1.048 9.5A18.022 18.022 0 016.412 9m6.088 9h7M11 21l5-10 5 10M12.751 5C11.783 10.77 8.07 15.61 3 18.129"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h3 class="font-medium text-gray-800">Multilingual Support</h3>
                                        <p class="text-sm text-gray-600">Accessible in multiple languages</p>
                                    </div>
                                </div>
                                <div class="bg-white p-4 rounded-lg border border-green-100 flex items-center">
                                    <div class="w-10 h-10 bg-green-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-green-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h3 class="font-medium text-gray-800">Privacy & Security</h3>
                                        <p class="text-sm text-gray-600">Anonymous submission option</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Voice & Text Submission Section -->
    <section id="submission" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="max-w-5xl mx-auto">
                <div class="text-center mb-12 animate-fadeIn opacity-0">
                    <span class="inline-block px-4 py-1 bg-green-100 text-green-800 rounded-full text-sm font-medium mb-4">Communication</span>
                    <h2 class="text-3xl font-bold mb-4">Voice & Text Submission</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">
                        Share your ideas, concerns, and feedback directly with government entities through multiple channels.
                    </p>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                    <!-- Voice Majlis -->
                    <div class="bg-white rounded-xl shadow-md overflow-hidden animate-fadeIn opacity-0 delay-100">
                        <div class="p-6">
                            <div class="flex items-center mb-4">
                                <div class="w-12 h-12 bg-green-100 rounded-full flex items-center justify-center mr-4">
                                    <svg class="w-6 h-6 text-green-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11a7 7 0 01-7 7m0 0a7 7 0 01-7-7m7 7v4m0 0H8m4 0h4m-4-8a3 3 0 01-3-3V5a3 3 0 116 0v6a3 3 0 01-3 3z"></path>
                                    </svg>
                                </div>
                                <h3 class="text-xl font-bold">Voice Majlis</h3>
                            </div>
                            <p class="text-gray-600 mb-6">
                                Record and submit voice notes up to 2 minutes long, replicating the oral tradition of the Majlis. Perfect for those who prefer speaking over typing.
                            </p>
                            
                            <!-- Voice Recorder Demo -->
                            <div class="bg-gray-50 rounded-lg p-6 mb-6 border border-gray-200 bg-cover bg-center" style="background-image: url('https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/e6be0612-13f5-4a39-9692-373cbb089df9.png');">
                                <div class="flex flex-col items-center">
                                    <div class="w-20 h-20 bg-green-100 rounded-full flex items-center justify-center mb-4">
                                        <svg class="w-10 h-10 text-green-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11a7 7 0 01-7 7m0 0a7 7 0 01-7-7m7 7v4m0 0H8m4 0h4m-4-8a3 3 0 01-3-3V5a3 3 0 116 0v6a3 3 0 01-3 3z"></path>
                                        </svg>
                                    </div>
                                    <div class="w-full bg-gray-200 rounded-full h-2.5 mb-4">
                                        <div id="voice-progress-bar" class="bg-green-700 h-2.5 rounded-full w-0"></div>
                                    </div>
                                    <p class="text-gray-500 mb-4">Recording... <span id="voice-timer">00:00</span> / 02:00</p>
                                    <div class="flex space-x-4">
                                        <button id="start-recording" class="px-4 py-2 bg-green-600 text-white rounded-md hover:bg-green-700 transition">
                                            Start Recording
                                        </button>
                                        <button id="stop-recording" class="px-4 py-2 bg-red-600 text-white rounded-md hover:bg-red-700 transition" disabled>
                                            Stop Recording
                                        </button>
                                        <button id="play-recording" class="px-4 py-2 bg-blue-600 text-white rounded-md hover:bg-blue-700 transition" disabled>
                                            Play Recording
                                        </button>
                                    </div>
                                    <audio id="audio-playback" controls class="mt-4 hidden"></audio>
                                </div>
                            </div>
                            
                            <div class="flex flex-col sm:flex-row sm:items-center justify-between">
                                <div class="mb-4 sm:mb-0">
                                    <span class="text-sm font-medium text-gray-700">Key Benefits:</span>
                                    <div class="flex flex-wrap gap-2 mt-2">
                                        <span class="px-2 py-1 bg-green-50 text-green-700 rounded text-xs">Accessibility</span>
                                        <span class="px-2 py-1 bg-green-50 text-green-700 rounded text-xs">Preserves Tradition</span>
                                        <span class="px-2 py-1 bg-green-50 text-green-700 rounded text-xs">Easy to Use</span>
                                    </div>
                                </div>
                                <button id="submit-voice-majlis" class="px-4 py-2 bg-green-700 text-white rounded-md hover:bg-green-800 transition">
                                    Submit Voice Majlis
                                </button>
                            </div>
                        </div>
                    </div>
                    
                    <!-- Text Majlis -->
                    <div class="bg-white rounded-xl shadow-md overflow-hidden animate-fadeIn opacity-0 delay-200">
                        <div class="p-6">
                            <div class="flex items-center mb-4">
                                <div class="w-12 h-12 bg-red-100 rounded-full flex items-center justify-center mr-4">
                                    <svg class="w-6 h-6 text-red-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z"></path>
                                    </svg>
                                </div>
                                <h3 class="text-xl font-bold">Text Majlis</h3>
                            </div>
                            <p class="text-gray-600 mb-6">
                                Submit written concerns, suggestions, and feedback in multiple local languages to ensure inclusivity. Choose between concise proposals or detailed explanations.
                            </p>
                            
                            <!-- Text Submission Demo -->
                            <div class="bg-gray-50 rounded-lg p-6 mb-6 border border-gray-200">
                                <div class="mb-4">
                                    <label class="block text-gray-700 text-sm font-medium mb-2" for="subject">Subject</label>
                                    <input class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-green-500" type="text" id="subject" placeholder="Enter subject" value="Community Park Proposal">
                                </div>
                                <div class="mb-4">
                                    <label class="block text-gray-700 text-sm font-medium mb-2" for="message">
                                        Message <span class="text-gray-500 text-xs">(1000 characters max)</span>
                                    </label>
                                    <textarea class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-green-500" id="message" rows="3" placeholder="Type your message">I would like to propose the development of a new community park in the Al Wasl area. The neighborhood currently lacks sufficient green spaces for families and children...</textarea>
                                </div>
                                <div class="flex justify-between items-center">
                                    <div class="flex items-center">
                                        <label class="inline-flex items-center text-sm text-gray-700">
                                            <input type="checkbox" class="form-checkbox h-4 w-4 text-green-700" checked>
                                            <span class="ml-2">Submit anonymously</span>
                                        </label>
                                    </div>
                                    <span class="text-sm text-gray-500">Characters: 142/1000</span>
                                </div>
                            </div>
                            
                            <div class="flex flex-col sm:flex-row sm:items-center justify-between">
                                <div class="mb-4 sm:mb-0">
                                    <span class="text-sm font-medium text-gray-700">Key Benefits:</span>
                                    <div class="flex flex-wrap gap-2 mt-2">
                                        <span class="px-2 py-1 bg-red-50 text-red-700 rounded text-xs">Multilingual</span>
                                        <span class="px-2 py-1 bg-red-50 text-red-700 rounded text-xs">Detailed Feedback</span>
                                        <span class="px-2 py-1 bg-red-50 text-red-700 rounded text-xs">Precision</span>
                                    </div>
                                </div>
                                <button id="submit-text-majlis" class="px-4 py-2 bg-red-700 text-white rounded-md hover:bg-red-800 transition">
                                    Submit Text Majlis
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Share Your Idea Module -->
                <div class="mt-8 bg-white rounded-xl shadow-md overflow-hidden animate-fadeIn opacity-0 delay-300">
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="w-12 h-12 bg-blue-100 rounded-full flex items-center justify-center mr-4">
                                <svg class="w-6 h-6 text-blue-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z"></path>
                                </svg>
                            </div>
                            <h3 class="text-xl font-bold">Share Your Idea Module</h3>
                        </div>
                        <p class="text-gray-600 mb-6">
                            A dedicated section for citizens to submit innovative ideas for community improvement or policy suggestions. Help shape the future of your community with your creative solutions.
                        </p>
                        
                        <!-- Idea Submission Demo -->
                        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-6">
                            <div class="md:col-span-2">
                                <div class="bg-gray-50 rounded-lg p-6 border border-gray-200 h-full">
                                    <h4 class="font-medium text-gray-800 mb-4">Submit Your Innovative Idea</h4>
                                    <div class="mb-4">
                                        <label class="block text-gray-700 text-sm font-medium mb-2" for="idea-title">Title</label>
                                        <input class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" type="text" id="idea-title" placeholder="Give your idea a catchy title">
                                    </div>
                                    <div class="mb-4">
                                        <label class="block text-gray-700 text-sm font-medium mb-2" for="idea-category">Category</label>
                                        <select class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" id="idea-category">
                                            <option>Select a category</option>
                                            <option>Infrastructure</option>
                                            <option>Education</option>
                                            <option>Environment</option>
                                            <option>Healthcare</option>
                                            <option>Technology</option>
                                            <option>Community Services</option>
                                        </select>
                                    </div>
                                    <div class="mb-4">
                                        <label class="block text-gray-700 text-sm font-medium mb-2" for="idea-description">Description</label>
                                        <textarea class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" id="idea-description" rows="4" placeholder="Describe your idea in detail"></textarea>
                                    </div>
                                    <div class="mb-4">
                                        <label class="block text-gray-700 text-sm font-medium mb-2" for="idea-impact">Expected Impact</label>
                                        <textarea class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500" id="idea-impact" rows="2" placeholder="How will your idea benefit the community?"></textarea>
                                    </div>
                                    <div class="flex justify-end">
                                        <button class="px-4 py-2 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                            Submit Idea
                                        </button>
                                    </div>
                                </div>
                            </div>
                            <div>
                                <div class="bg-blue-50 rounded-lg p-6 border border-blue-100 h-full">
                                    <h4 class="font-medium text-gray-800 mb-4">Featured Ideas</h4>
                                    <div class="space-y-4">
                                        <div class="bg-white p-3 rounded border border-gray-200">
                                            <h5 class="font-medium text-gray-800">Smart Street Lighting</h5>
                                            <p class="text-sm text-gray-600 mb-2">Energy-efficient LED lights that adjust based on pedestrian activity.</p>
                                            <div class="flex justify-between items-center">
                                                <span class="text-xs bg-blue-100 text-blue-800 px-2 py-1 rounded">Infrastructure</span>
                                                <span class="text-xs text-gray-500">2 days ago</span>
                                            </div>
                                        </div>
                                        <div class="bg-white p-3 rounded border border-gray-200">
                                            <h5 class="font-medium text-gray-800">Community Recycling Program</h5>
                                            <p class="text-sm text-gray-600 mb-2">Incentive-based recycling system for residential areas.</p>
                                            <div class="flex justify-between items-center">
                                                <span class="text-xs bg-green-100 text-green-800 px-2 py-1 rounded">Environment</span>
                                                <span class="text-xs text-gray-500">1 week ago</span>
                                            </div>
                                        </div>
                                        <div class="bg-white p-3 rounded border border-gray-200">
                                            <h5 class="font-medium text-gray-800">Youth Mentorship Network</h5>
                                            <p class="text-sm text-gray-600 mb-2">Connecting students with industry professionals.</p>
                                            <div class="flex justify-between items-center">
                                                <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded">Education</span>
                                                <span class="text-xs text-gray-500">2 weeks ago</span>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="flex flex-col sm:flex-row sm:items-center justify-between">
                            <div class="mb-4 sm:mb-0">
                                <span class="text-sm font-medium text-gray-700">Key Benefits:</span>
                                <div class="flex flex-wrap gap-2 mt-2">
                                    <span class="px-2 py-1 bg-blue-50 text-blue-700 rounded text-xs">Innovation</span>
                                    <span class="px-2 py-1 bg-blue-50 text-blue-700 rounded text-xs">Community Involvement</span>
                                    <span class="px-2 py-1 bg-blue-50 text-blue-700 rounded text-xs">Collaborative Solutions</span>
                                </div>
                            </div>
                            <button class="px-4 py-2 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                Explore Ideas
                            </button>
                        </div>
                    </div>
                </div>
                
                <!-- Issue Categorization & Tagging -->
                <div class="mt-8 bg-white rounded-xl shadow-md overflow-hidden animate-fadeIn opacity-0 delay-400">
                    <div class="p-6">
                        <div class="flex items-center mb-4">
                            <div class="w-12 h-12 bg-purple-100 rounded-full flex items-center justify-center mr-4">
                                <svg class="w-6 h-6 text-purple-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 7h.01M7 3h5c.512 0 1.024.195 1.414.586l7 7a2 2 0 010 2.828l-7 7a2 2 0 01-2.828 0l-7-7A1.994 1.994 0 013 12V7a4 4 0 014-4z"></path>
                                </svg>
                            </div>
                            <h3 class="text-xl font-bold">Issue Categorization & Tagging</h3>
                        </div>
                        <p class="text-gray-600 mb-6">
                            Select categories and add keywords for easier sorting and routing to relevant departments. Our smart tagging system ensures your concerns reach the right government officials efficiently.
                        </p>
                        
                        <!-- Categorization Demo -->
                        <div class="bg-gray-50 rounded-lg p-6 mb-6 border border-gray-200">
                            <h4 class="font-medium text-gray-800 mb-4">Select Categories & Tags</h4>
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                                <div>
                                    <label class="block text-gray-700 text-sm font-medium mb-2">Primary Category</label>
                                    <div class="grid grid-cols-2 gap-3">
                                        <div class="bg-white p-3 rounded border border-purple-200 cursor-pointer hover:bg-purple-50 transition flex items-center">
                                            <input type="radio" name="category" class="form-radio h-4 w-4 text-purple-700 mr-2">
                                            <span>Infrastructure</span>
                                        </div>
                                        <div class="bg-white p-3 rounded border border-purple-200 cursor-pointer hover:bg-purple-50 transition flex items-center">
                                            <input type="radio" name="category" class="form-radio h-4 w-4 text-purple-700 mr-2">
                                            <span>Education</span>
                                        </div>
                                        <div class="bg-white p-3 rounded border border-purple-200 cursor-pointer hover:bg-purple-50 transition flex items-center">
                                            <input type="radio" name="category" class="form-radio h-4 w-4 text-purple-700 mr-2" checked>
                                            <span>Environment</span>
                                        </div>
                                        <div class="bg-white p-3 rounded border border-purple-200 cursor-pointer hover:bg-purple-50 transition flex items-center">
                                            <input type="radio" name="category" class="form-radio h-4 w-4 text-purple-700 mr-2">
                                            <span>Healthcare</span>
                                        </div>
                                    </div>
                                </div>
                                <div>
                                    <label class="block text-gray-700 text-sm font-medium mb-2">Add Tags</label>
                                    <div class="mb-2">
                                        <input class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-purple-500" type="text" placeholder="Type and press Enter to add tags">
                                    </div>
                                    <div class="flex flex-wrap gap-2">
                                        <span class="px-3 py-1 bg-purple-100 text-purple-800 rounded-full text-sm flex items-center">
                                            Recycling
                                            <button class="ml-1 focus:outline-none">
                                                <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 20 20">
                                                    <path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path>
                                                </svg>
                                            </button>
                                        </span>
                                        <span class="px-3 py-1 bg-purple-100 text-purple-800 rounded-full text-sm flex items-center">
                                            Waste Management
                                            <button class="ml-1 focus:outline-none">
                                                <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 20 20">
                                                    <path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path>
                                                </svg>
                                            </button>
                                        </span>
                                        <span class="px-3 py-1 bg-purple-100 text-purple-800 rounded-full text-sm flex items-center">
                                            Community
                                            <button class="ml-1 focus:outline-none">
                                                <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 20 20">
                                                    <path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path>
                                                </svg>
                                            </button>
                                        </span>
                                    </div>
                                </div>
                            </div>
                            <div class="mt-6">
                                <label class="block text-gray-700 text-sm font-medium mb-2">Relevant Department</label>
                                <div class="bg-purple-50 p-4 rounded border border-purple-100">
                                    <div class="flex items-center">
                                        <svg class="w-5 h-5 text-purple-700 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                        </svg>
                                        <span class="text-sm">Based on your selection, your submission will be routed to:</span>
                                    </div>
                                    <div class="mt-2 flex items-center">
                                        <div class="w-10 h-10 bg-white rounded-full flex items-center justify-center mr-3 border border-purple-200">
                                            <svg class="w-5 h-5 text-purple-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"></path>
                                            </svg>
                                        </div>
                                        <div>
                                            <h5 class="font-medium">Ministry of Climate Change & Environment</h5>
                                            <p class="text-sm text-gray-600">Waste Management & Recycling Division</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="flex flex-col sm:flex-row sm:items-center justify-between">
                            <div class="mb-4 sm:mb-0">
                                <span class="text-sm font-medium text-gray-700">Key Benefits:</span>
                                <div class="flex flex-wrap gap-2 mt-2">
                                    <span class="px-2 py-1 bg-purple-50 text-purple-700 rounded text-xs">Efficient Routing</span>
                                    <span class="px-2 py-1 bg-purple-50 text-purple-700 rounded text-xs">Faster Response</span>
                                    <span class="px-2 py-1 bg-purple-50 text-purple-700 rounded text-xs">Better Organization</span>
                                </div>
                            </div>
                            <button class="px-4 py-2 bg-purple-700 text-white rounded-md hover:bg-purple-800 transition">
                                Learn More
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Follow My Concern Tracker Section -->
    <section id="tracking" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="max-w-5xl mx-auto">
                <div class="text-center mb-12 animate-fadeIn opacity-0">
                    <span class="inline-block px-4 py-1 bg-yellow-100 text-yellow-800 rounded-full text-sm font-medium mb-4">Transparency</span>
                    <h2 class="text-3xl font-bold mb-4">Follow My Concern Tracker</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">
                        Track the status of your submitted issues or ideas in real-time, receiving notifications on progress at every step.
                    </p>
                </div>
                
                <div class="bg-white rounded-xl shadow-md overflow-hidden animate-fadeIn opacity-0 delay-100">
                    <div class="p-6">
                        <!-- Tracker Demo -->
                        <div class="bg-gray-50 rounded-lg p-6 mb-6 border border-gray-200">
                            <div class="flex flex-col md:flex-row md:items-center justify-between mb-6">
                                <div>
                                    <h4 class="font-medium text-gray-800">My Submissions</h4>
                                    <p class="text-sm text-gray-600">Track the status of your concerns and ideas</p>
                                </div>
                                <div class="mt-4 md:mt-0">
                                    <div class="relative">
                                        <input type="text" class="pl-10 pr-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-yellow-500 w-full" placeholder="Search submissions...">
                                        <div class="absolute left-3 top-2.5">
                                            <svg class="h-5 w-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path>
                                            </svg>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <div class="overflow-x-auto">
                                <table class="min-w-full divide-y divide-gray-200">
                                    <thead class="bg-gray-100">
                                        <tr>
                                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">ID</th>
                                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Subject</th>
                                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Category</th>
                                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Submitted</th>
                                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Status</th>
                                            <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider">Action</th>
                                        </tr>
                                    </thead>
                                    <tbody class="bg-white divide-y divide-gray-200">
                                        <tr class="hover:bg-gray-50">
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-900">#2453</td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-900">Infrastructure proposal</td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">Infrastructure</td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">2 days ago</td>
                                            <td class="px-6 py-4 whitespace-nowrap">
                                                <span class="px-2 py-1 inline-flex text-xs leading-5 font-semibold rounded-full bg-yellow-100 text-yellow-800">
                                                    In Progress
                                                </span>
                                            </td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
                                                <button class="text-yellow-700 hover:text-yellow-900">View Details</button>
                                            </td>
                                        </tr>
                                        <tr class="hover:bg-gray-50">
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-900">#1872</td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-900">Community feedback</td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">Community Services</td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">1 week ago</td>
                                            <td class="px-6 py-4 whitespace-nowrap">
                                                <span class="px-2 py-1 inline-flex text-xs leading-5 font-semibold rounded-full bg-green-100 text-green-800">
                                                    Resolved
                                                </span>
                                            </td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
                                                <button class="text-yellow-700 hover:text-yellow-900">View Details</button>
                                            </td>
                                        </tr>
                                        <tr class="hover:bg-gray-50">
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-900">#1654</td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-900">Education initiative</td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">Education</td>
                                            <td class="px-6 py-4 whitespace-nowrap">
                                                <span class="px-2 py-1 inline-flex text-xs leading-5 font-semibold rounded-full bg-blue-100 text-blue-800">
                                                    Under Review
                                                </span>
                                            </td>
                                            <td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500">
                                                <button class="text-yellow-700 hover:text-yellow-900">View Details</button>
                                            </td>
                                        </tr>
                                    </tbody>
                                </table>
                            </div>
                        </div>
                        
                        <!-- Detailed Tracker View -->
                        <div class="bg-yellow-50 rounded-lg p-6 border border-yellow-100">
                            <div class="flex items-center justify-between mb-6">
                                <div class="flex items-center">
                                    <div class="w-10 h-10 bg-yellow-100 rounded-full flex items-center justify-center mr-4">
                                        <svg class="w-5 h-5 text-yellow-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="font-medium text-gray-800">Infrastructure Proposal #2453</h4>
                                        <p class="text-sm text-gray-600">Submitted 2 days ago</p>
                                    </div>
                                </div>
                                <span class="px-3 py-1 bg-yellow-200 text-yellow-800 rounded-full text-sm font-medium">In Progress</span>
                            </div>
                            
                            <div class="relative">
                                <!-- Progress Timeline -->
                                <div class="ml-6 border-l-2 border-yellow-300 pl-6 pb-6">
                                    <div class="absolute -left-1 mt-2">
                                        <div class="w-6 h-6 bg-green-500 rounded-full border-4 border-white"></div>
                                    </div>
                                    <div class="mb-6">
                                        <h5 class="font-medium text-gray-800">Submission Received</h5>
                                        <p class="text-sm text-gray-600 mb-2">Your proposal has been successfully submitted to our system.</p>
                                        <span class="text-xs text-gray-500">May 15, 2023 - 10:23 AM</span>
                                    </div>
                                </div>
                                
                                <div class="ml-6 border-l-2 border-yellow-300 pl-6 pb-6">
                                    <div class="absolute -left-1 mt-2">
                                        <div class="w-6 h-6 bg-green-500 rounded-full border-4 border-white"></div>
                                    </div>
                                    <div class="mb-6">
                                        <h5 class="font-medium text-gray-800">Initial Review</h5>
                                        <p class="text-sm text-gray-600 mb-2">Your proposal has been reviewed by our team and categorized appropriately.</p>
                                        <span class="text-xs text-gray-500">May 15, 2023 - 2:45 PM</span>
                                    </div>
                                </div>
                                
                                <div class="ml-6 border-l-2 border-yellow-300 pl-6 pb-6">
                                    <div class="absolute -left-1 mt-2">
                                        <div class="w-6 h-6 bg-green-500 rounded-full border-4 border-white"></div>
                                    </div>
                                    <div class="mb-6">
                                        <h5 class="font-medium text-gray-800">Forwarded to Department</h5>
                                        <p class="text-sm text-gray-600 mb-2">Your proposal has been forwarded to the Roads & Infrastructure Authority for further assessment.</p>
                                        <span class="text-xs text-gray-500">May 16, 2023 - 9:30 AM</span>
                                    </div>
                                </div>
                                
                                <div class="ml-6 border-l-2 border-gray-200 pl-6 pb-6">
                                    <div class="absolute -left-1 mt-2">
                                        <div class="w-6 h-6 bg-yellow-400 rounded-full border-4 border-white animate-pulse"></div>
                                    </div>
                                    <div class="mb-6">
                                        <h5 class="font-medium text-gray-800">Under Assessment</h5>
                                        <p class="text-sm text-gray-600 mb-2">Your proposal is currently being assessed by the relevant department.</p>
                                        <span class="text-xs text-gray-500">In Progress</span>
                                    </div>
                                </div>
                                
                                <div class="ml-6 border-l-2 border-gray-200 pl-6 pb-6">
                                    <div class="absolute -left-1 mt-2">
                                        <div class="w-6 h-6 bg-gray-300 rounded-full border-4 border-white"></div>
                                    </div>
                                    <div class="mb-6">
                                        <h5 class="font-medium text-gray-400">Decision</h5>
                                        <p class="text-sm text-gray-400 mb-2">Awaiting decision from the relevant department.</p>
                                    </div>
                                </div>
                                
                                <div class="ml-6 pl-6">
                                    <div class="absolute -left-1 mt-2">
                                        <div class="w-6 h-6 bg-gray-300 rounded-full border-4 border-white"></div>
                                    </div>
                                    <div>
                                        <h5 class="font-medium text-gray-400">Implementation</h5>
                                        <p class="text-sm text-gray-400 mb-2">If approved, your proposal will enter the implementation phase.</p>
                                    </div>
                                </div>
                            </div>
                            
                            <div class="mt-6 pt-6 border-t border-yellow-200">
                                <h5 class="font-medium text-gray-800 mb-3">Updates & Comments</h5>
                                <div class="bg-white p-4 rounded border border-gray-200 mb-4">
                                    <div class="flex items-start">
                                        <div class="w-8 h-8 bg-blue-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                            <svg class="w-4 h-4 text-blue-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"></path>
                                            </svg>
                                        </div>
                                        <div>
                                            <div class="flex items-center mb-1">
                                                <h6 class="font-medium text-gray-800 mr-2">Ahmed Al Mansouri</h6>
                                                <span class="text-xs text-gray-500">Roads & Infrastructure Authority</span>
                                            </div>
                                            <p class="text-sm text-gray-600 mb-1">
                                                Thank you for your detailed proposal. We are currently assessing the feasibility and budget requirements. We may need additional information about the specific location.
                                            </p>
                                            <span class="text-xs text-gray-500">May 16, 2023 - 11:45 AM</span>
                                        </div>
                                    </div>
                                </div>
                                
                                <div class="flex">
                                    <div class="w-8 h-8 bg-yellow-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-4 h-4 text-yellow-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z"></path>
                                        </svg>
                                    </div>
                                    <div class="flex-1">
                                        <textarea class="w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-yellow-500" rows="2" placeholder="Add a comment or additional information..."></textarea>
                                        <div class="flex justify-end mt-2">
                                            <button class="px-4 py-2 bg-yellow-700 text-white rounded-md hover:bg-yellow-800 transition">
                                                Submit Comment
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-6 flex flex-col sm:flex-row sm:items-center justify-between">
                            <div class="mb-4 sm:mb-0">
                                <span class="text-sm font-medium text-gray-700">Key Benefits:</span>
                                <div class="flex flex-wrap gap-2 mt-2">
                                    <span class="px-2 py-1 bg-yellow-50 text-yellow-700 rounded text-xs">Real-time Updates</span>
                                    <span class="px-2 py-1 bg-yellow-50 text-yellow-700 rounded text-xs">Transparency</span>
                                    <span class="px-2 py-1 bg-yellow-50 text-yellow-700 rounded text-xs">Two-way Communication</span>
                                </div>
                            </div>
                            <button class="px-4 py-2 bg-yellow-700 text-white rounded-md hover:bg-yellow-800 transition">
                                View All Submissions
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Announcements & Consultations Section -->
    <section id="announcements" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="max-w-5xl mx-auto">
                <div class="text-center mb-12 animate-fadeIn opacity-0">
                    <span class="inline-block px-4 py-1 bg-red-100 text-red-800 rounded-full text-sm font-medium mb-4">Stay Informed</span>
                    <h2 class="text-3xl font-bold mb-4">Announcements & Consultations</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">
                        Stay updated with official government announcements, public consultation periods for new policies, and upcoming Majlis sessions.
                    </p>
                </div>
                
                <div class="bg-white rounded-xl shadow-md overflow-hidden animate-fadeIn opacity-0 delay-100">
                    <div class="p-6">
                        <!-- Announcements Tabs -->
                        <div class="border-b border-gray-200 mb-6">
                            <div class="flex flex-wrap -mb-px">
                                <button class="feature-tab active mr-2 inline-block py-2 px-4 text-sm font-medium focus:outline-none border-b-2 border-transparent rounded-t-lg" data-tab="announcements">
                                    Announcements
                                </button>
                                <button class="feature-tab mr-2 inline-block py-2 px-4 text-sm font-medium focus:outline-none border-b-2 border-transparent rounded-t-lg" data-tab="consultations">
                                    Public Consultations
                                </button>
                                <button class="feature-tab mr-2 inline-block py-2 px-4 text-sm font-medium focus:outline-none border-b-2 border-transparent rounded-t-lg" data-tab="majlis">
                                    Upcoming Majlis Sessions
                                </button>
                            </div>
                        </div>
                        
                        <!-- Announcements Content -->
                        <div id="announcements-content" class="feature-content active">
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                                <div class="bg-gray-50 rounded-lg p-6 border border-gray-200 bg-cover bg-center" style="background-image: url('https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/2da5f391-a34a-4b6e-953e-83b4cc48f71e.png'); background-blend-mode: overlay;">
                                    <div class="flex items-center mb-4">
                                        <div class="w-10 h-10 bg-red-100 rounded-full flex items-center justify-center mr-3">
                                            <svg class="w-5 h-5 text-red-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 5.882V19.24a1.76 1.76 0 01-3.417.592l-2.147-6.15M18 13a3 3 0 100-6M5.436 13.683A4.001 4.001 0 017 6h1.832c4.1 0 7.625-1.234 9.168-3v14c-1.543-1.766-5.067-3-9.168-3H7a3.988 3.988 0 01-1.564-.317z"></path>
                                            </svg>
                                        </div>
                                        <div>
                                            <h4 class="font-medium text-gray-800">Latest Announcements</h4>
                                            <p class="text-sm text-gray-600">Official updates from government entities</p>
                                        </div>
                                    </div>
                                    
                                    <div class="space-y-4">
                                        <div class="bg-white p-4 rounded border border-gray-200">
                                            <span class="text-xs bg-blue-100 text-blue-800 px-2 py-1 rounded mb-2 inline-block">Infrastructure</span>
                                            <h5 class="font-medium text-gray-800 mb-1">New Road Development Project</h5>
                                            <p class="text-sm text-gray-600 mb-2">
                                                The Roads & Transport Authority announces the commencement of a new road development project in Al Barsha South area.
                                            </p>
                                            <div class="flex justify-between items-center">
                                                <span class="text-xs text-gray-500">May 14, 2023</span>
                                                <a href="#" class="text-sm text-red-700 hover:text-red-800" onclick="showAnnouncement('road-dev-2023')">Read More</a>
                                            </div>
                                        </div>
                                        
                                        <div class="bg-white p-4 rounded border border-gray-200">
                                            <span class="text-xs bg-green-100 text-green-800 px-2 py-1 rounded mb-2 inline-block">Environment</span>
                                            <h5 class="font-medium text-gray-800 mb-1">Sustainable Energy Initiative</h5>
                                            <p class="text-sm text-gray-600 mb-2">
                                                The Ministry of Energy announces new incentives for residential solar panel installation.
                                            </p>
                                            <div class="flex justify-between items-center">
                                                <span class="text-xs text-gray-500">May 10, 2023</span>
                                                <a href="#" class="text-sm text-red-700 hover:text-red-800" onclick="showAnnouncement('solar-incentives-2023')">Read More</a>
                                            </div>
                                        </div>
                                        
                                        <div class="bg-white p-4 rounded border border-gray-200">
                                            <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded mb-2 inline-block">Education</span>
                                            <h5 class="font-medium text-gray-800 mb-1">New Scholarship Program</h5>
                                            <p class="text-sm text-gray-600 mb-2">
                                                The Ministry of Education announces scholarships for advanced technology studies abroad.
                                            </p>
                                            <div class="flex justify-between items-center">
                                                <span class="text-xs text-gray-500">May 5, 2023</span>
                                                <a href="#" class="text-sm text-red-700 hover:text-red-800" onclick="showAnnouncement('scholarship-2023')">Read More</a>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                
                                <div class="bg-red-50 rounded-lg p-6 border border-red-100">
                                    <div class="flex items-center mb-4">
                                        <div class="w-10 h-10 bg-red-100 rounded-full flex items-center justify-center mr-3">
                                            <svg class="w-5 h-5 text-red-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"></path>
                                            </svg>
                                        </div>
                                        <div>
                                            <h4 class="font-medium text-gray-800">Featured Announcement</h4>
                                            <p class="text-sm text-gray-600">Important update for all citizens</p>
                                        </div>
                                    </div>
                                    
                                    <div class="bg-white p-6 rounded border border-red-100 mb-4">
                                        <div class="flex items-center justify-between mb-4">
                                            <span class="px-3 py-1 bg-red-100 text-red-800 rounded-full text-sm font-medium">Important</span>
                                            <span class="text-sm text-gray-500">May 18, 2023</span>
                                        </div>
                                        <h4 class="text-xl font-bold text-gray-800 mb-3">National Digital Identity Update</h4>
                                        <p class="text-gray-600 mb-4">
                                            The Federal Authority for Identity and Citizenship announces important updates to the National Digital Identity system. All citizens and residents are required to update their information through the official app by June 30, 2023.
                                        </p>
                                        <div class="bg-red-50 p-4 rounded mb-4 flex items-start">
                                            <svg class="w-5 h-5 text-red-700 mr-2 mt-0.5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                                            </svg>
                                            <p class="text-sm text-red-700">
                                                This update is mandatory and will ensure continued access to government services.
                                            </p>
                                        </div>
                                        <div class="flex justify-between items-center">
                                            <a href="#" class="text-red-700 hover:text-red-800 font-medium flex items-center" onclick="showAnnouncement('digital-id-2023')">
                                                Read Full Announcement
                                                <svg class="w-4 h-4 ml-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
                                                </svg>
                                            </a>
                                            <button class="px-4 py-2 bg-red-700 text-white rounded-md hover:bg-red-800 transition">
                                                View All Announcements
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        
                        <!-- Public Consultations Content -->
                        <div id="consultations-content" class="feature-content">
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                                <div class="bg-gray-50 rounded-lg p-6 border border-gray-200">
                                    <div class="flex items-center mb-4">
                                        <div class="w-10 h-10 bg-red-100 rounded-full flex items-center justify-center mr-3">
                                            <svg class="w-5 h-5 text-red-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z"></path>
                                            </svg>
                                        </div>
                                        <div>
                                            <h4 class="font-medium text-gray-800">Open Public Consultations</h4>
                                            <p class="text-sm text-gray-600">Provide your input on upcoming policies</p>
                                        </div>
                                    </div>
                                    
                                    <div class="space-y-4">
                                        <div class="bg-white p-4 rounded border border-gray-200">
                                            <span class="text-xs bg-yellow-100 text-yellow-800 px-2 py-1 rounded mb-2 inline-block">Open until June 30</span>
                                            <h5 class="font-medium text-gray-800 mb-1">Environmental Protection Act Amendments</h5>
                                            <p class="text-sm text-gray-600 mb-2">
                                                Seeking public feedback on proposed amendments to the Environmental Protection Act to enhance sustainability efforts.
                                            </p>
                                            <div class="flex justify-between items-center">
                                                <span class="text-xs text-gray-500">Ministry of Climate Change</span>
                                                <a href="#" class="text-sm text-red-700 hover:text-red-800">Participate</a>
                                            </div>
                                        </div>
                                        
                                        <div class="bg-white p-4 rounded border border-gray-200">
                                            <span class="text-xs bg-yellow-100 text-yellow-800 px-2 py-1 rounded mb-2 inline-block">Open until July 15</span>
                                            <h5 class="font-medium text-gray-800 mb-1">Digital Economy Strategy 2030</h5>
                                            <p class="text-sm text-gray-600 mb-2">
                                                Consultation on the national strategy to accelerate digital transformation and foster innovation.
                                            </p>
                                            <div class="flex justify-between items-center">
                                                <span class="text-xs text-gray-500">Ministry of Economy</span>
                                                <a href="#" class="text-sm text-red-700 hover:text-red-800">Participate</a>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                
                                <div class="bg-red-50 rounded-lg p-6 border border-red-100">
                                    <div class="flex items-center mb-4">
                                        <div class="w-10 h-10 bg-red-100 rounded-full flex items-center justify-center mr-3">
                                            <svg class="w-5 h-5 text-red-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01"></path>
                                            </svg>
                                        </div>
                                        <div>
                                            <h4 class="font-medium text-gray-800">How Public Consultations Work</h4>
                                            <p class="text-sm text-gray-600">Your voice shapes policy</p>
                                        </div>
                                    </div>
                                    <p class="text-gray-700 mb-4">
                                        Public consultations are an essential part of our democratic process. They allow citizens and stakeholders to provide valuable input on proposed laws, policies, and strategies before they are finalized. Your feedback helps us create more effective and inclusive governance.
                                    </p>
                                    <ul class="list-disc list-inside text-gray-600 space-y-2">
                                        <li>Review consultation documents and proposals.</li>
                                        <li>Submit your comments, suggestions, and concerns.</li>
                                        <li>Your feedback is analyzed and considered by policymakers.</li>
                                        <li>Final policies are published, often with a summary of public feedback.</li>
                                    </ul>
                                    <button class="mt-6 px-4 py-2 bg-red-700 text-white rounded-md hover:bg-red-800 transition">
                                        View All Consultations
                                    </button>
                                </div>
                            </div>
                        </div>
                        
                        <!-- Upcoming Majlis Sessions Content -->
                        <div id="majlis-content" class="feature-content">
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                                <div class="bg-gray-50 rounded-lg p-6 border border-gray-200">
                                    <div class="flex items-center mb-4">
                                        <div class="w-10 h-10 bg-red-100 rounded-full flex items-center justify-center mr-3">
                                            <svg class="w-5 h-5 text-red-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2zm3-7h.01M12 15h.01M15 15h.01"></path>
                                            </svg>
                                        </div>
                                        <div>
                                            <h4 class="font-medium text-gray-800">Upcoming Majlis Sessions</h4>
                                            <p class="text-sm text-gray-600">Schedule of traditional consultative gatherings</p>
                                        </div>
                                    </div>
                                    
                                    <div class="space-y-4">
                                        <div class="bg-white p-4 rounded border border-gray-200">
                                            <h5 class="font-medium text-gray-800 mb-1">Community Majlis - Al Wasl</h5>
                                            <p class="text-sm text-gray-600 mb-2">
                                                A session for residents of Al Wasl to discuss local community issues and initiatives.
                                            </p>
                                            <div class="flex justify-between items-center text-sm text-gray-600">
                                                <span><strong class="text-gray-800">Date:</strong> June 5, 2023</span>
                                                <span><strong class="text-gray-800">Time:</strong> 7:00 PM - 9:00 PM</span>
                                            </div>
                                            <div class="text-sm text-gray-600 mt-1">
                                                <span><strong class="text-gray-800">Location:</strong> Al Wasl Community Hall</span>
                                            </div>
                                            <a href="#" class="text-sm text-red-700 hover:text-red-800 mt-2 inline-block">Register to Attend</a>
                                        </div>
                                        
                                        <div class="bg-white p-4 rounded border border-gray-200">
                                            <h5 class="font-medium text-gray-800 mb-1">Youth Majlis - Future of Technology</h5>
                                            <p class="text-sm text-gray-600 mb-2">
                                                A special Majlis for young Emiratis to share their visions on technology and innovation.
                                            </p>
                                            <div class="flex justify-between items-center text-sm text-gray-600">
                                                <span><strong class="text-gray-800">Date:</strong> June 12, 2023</span>
                                                <span><strong class="text-gray-800">Time:</strong> 6:00 PM - 8:00 PM</span>
                                            </div>
                                            <div class="text-sm text-gray-600 mt-1">
                                                <span><strong class="text-gray-800">Location:</strong> Dubai Future Foundation</span>
                                            </div>
                                            <a href="#" class="text-sm text-red-700 hover:text-red-800 mt-2 inline-block">Register to Attend</a>
                                        </div>
                                    </div>
                                </div>
                                
                                <div class="bg-red-50 rounded-lg p-6 border border-red-100">
                                    <div class="flex items-center mb-4">
                                        <div class="w-10 h-10 bg-red-100 rounded-full flex items-center justify-center mr-3">
                                            <svg class="w-5 h-5 text-red-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2H6a2 2 0 01-2-2V6zM14 6a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2V6zM4 16a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2H6a2 2 0 01-2-2v-2zM14 16a2 2 0 012-2h2a2 2 0 012 2v2a2 2 0 01-2 2h-2a2 2 0 01-2-2v-2z"></path>
                                            </svg>
                                        </div>
                                        <div>
                                            <h4 class="font-medium text-gray-800">About Majlis Sessions</h4>
                                            <p class="text-sm text-gray-600">The heart of Emirati tradition</p>
                                        </div>
                                    </div>
                                    <p class="text-gray-700 mb-4">
                                        The Majlis is a traditional gathering place where community members meet to discuss local issues, share news, and seek advice. It embodies the spirit of open dialogue, consultation, and direct communication between leaders and citizens. These sessions are crucial for fostering community cohesion and ensuring that government decisions reflect the needs and aspirations of the people.
                                    </p>
                                    <button class="mt-6 px-4 py-2 bg-red-700 text-white rounded-md hover:bg-red-800 transition">
                                        Learn More About Majlis
                                    </button>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-6 flex flex-col sm:flex-row sm:items-center justify-between">
                            <div class="mb-4 sm:mb-0">
                                <span class="text-sm font-medium text-gray-700">Key Benefits:</span>
                                <div class="flex flex-wrap gap-2 mt-2">
                                    <span class="px-2 py-1 bg-red-50 text-red-700 rounded text-xs">Direct Engagement</span>
                                    <span class="px-2 py-1 bg-red-50 text-red-700 rounded text-xs">Community Building</span>
                                    <span class="px-2 py-1 bg-red-50 text-red-700 rounded text-xs">Cultural Preservation</span>
                                </div>
                            </div>
                            <button class="px-4 py-2 bg-red-700 text-white rounded-md hover:bg-red-800 transition">
                                View All Announcements
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Representative Directory Section -->
    <section id="directory" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="max-w-5xl mx-auto">
                <div class="text-center mb-12 animate-fadeIn opacity-0">
                    <span class="inline-block px-4 py-1 bg-blue-100 text-blue-800 rounded-full text-sm font-medium mb-4">Connect</span>
                    <h2 class="text-3xl font-bold mb-4">Representative Directory</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">
                        Find and connect with your local government representatives and officials.
                    </p>
                </div>
                
                <div class="bg-white rounded-xl shadow-md overflow-hidden animate-fadeIn opacity-0 delay-100">
                    <div class="p-6">
                        <!-- Search and Filter -->
                        <div class="flex flex-col md:flex-row justify-between items-center mb-6 space-y-4 md:space-y-0 md:space-x-4">
                            <div class="relative w-full md:w-1/2">
                                <input type="text" class="pl-10 pr-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500 w-full" placeholder="Search by name, department, or role...">
                                <div class="absolute left-3 top-2.5">
                                    <svg class="h-5 w-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path>
                                    </svg>
                                </div>
                            </div>
                            <div class="flex space-x-4 w-full md:w-auto">
                                <select class="px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500 w-full">
                                    <option>All Departments</option>
                                    <option>Ministry of Infrastructure</option>
                                    <option>Ministry of Education</option>
                                    <option>Ministry of Health</option>
                                    <option>Ministry of Climate Change</option>
                                </select>
                                <select class="px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500 w-full">
                                    <option>All Roles</option>
                                    <option>Minister</option>
                                    <option>Director General</option>
                                    <option>Department Head</option>
                                    <option>Advisor</option>
                                </select>
                            </div>
                        </div>
                        
                        <!-- Representative Cards -->
                        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200 text-center">
                                <img class="w-24 h-24 rounded-full mx-auto mb-4 object-cover" src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/68265b5f-486b-4e29-ae2a-e1ca2b036d27.png" alt="UAE Government Official">
                                <h4 class="font-bold text-lg text-gray-800">H.E. Dr. Sultan Al Jaber</h4>
                                <p class="text-blue-700 font-medium mb-2">Minister of Industry and Advanced Technology</p>
                                <p class="text-gray-600 text-sm mb-4">Oversees industrial development and technological innovation.</p>
                                <button class="px-4 py-2 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                    Contact
                                </button>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200 text-center">
                                <img class="w-24 h-24 rounded-full mx-auto mb-4 object-cover" src="https://via.placeholder.com/150/00732f/FFFFFF?text=Rep2" alt="Representative Photo">
                                <h4 class="font-bold text-lg text-gray-800">H.E. Sarah Al Amiri</h4>
                                <p class="text-blue-700 font-medium mb-2">Minister of State for Public Education and Advanced Technology</p>
                                <p class="text-gray-600 text-sm mb-4">Leads initiatives in education and space science.</p>
                                <button class="px-4 py-2 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                    Contact
                                </button>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200 text-center">
                                <img class="w-24 h-24 rounded-full mx-auto mb-4 object-cover" src="https://via.placeholder.com/150/00732f/FFFFFF?text=Rep3" alt="Representative Photo">
                                <h4 class="font-bold text-lg text-gray-800">H.E. Mariam Al Mheiri</h4>
                                <p class="text-blue-700 font-medium mb-2">Minister of Climate Change and Environment</p>
                                <p class="text-gray-600 text-sm mb-4">Focuses on environmental sustainability and food security.</p>
                                <button class="px-4 py-2 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                    Contact
                                </button>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200 text-center">
                                <img class="w-24 h-24 rounded-full mx-auto mb-4 object-cover" src="https://via.placeholder.com/150/00732f/FFFFFF?text=Rep4" alt="Representative Photo">
                                <h4 class="font-bold text-lg text-gray-800">H.E. Abdullah Al Nuaimi</h4>
                                <p class="text-blue-700 font-medium mb-2">Undersecretary of Ministry of Infrastructure Development</p>
                                <p class="text-gray-600 text-sm mb-4">Manages national infrastructure projects and planning.</p>
                                <button class="px-4 py-2 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                    Contact
                                </button>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200 text-center">
                                <img class="w-24 h-24 rounded-full mx-auto mb-4 object-cover" src="https://via.placeholder.com/150/00732f/FFFFFF?text=Rep5" alt="Representative Photo">
                                <h4 class="font-bold text-lg text-gray-800">H.E. Omar Al Olama</h4>
                                <p class="text-blue-700 font-medium mb-2">Minister of State for Artificial Intelligence, Digital Economy and Remote Work Applications</p>
                                <p class="text-gray-600 text-sm mb-4">Drives AI adoption and digital economy growth.</p>
                                <button class="px-4 py-2 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                    Contact
                                </button>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200 text-center">
                                <img class="w-24 h-24 rounded-full mx-auto mb-4 object-cover" src="https://via.placeholder.com/150/00732f/FFFFFF?text=Rep6" alt="Representative Photo">
                                <h4 class="font-bold text-lg text-gray-800">H.E. Hessa Buhumaid</h4>
                                <p class="text-blue-700 font-medium mb-2">Director General of Community Development Authority</p>
                                <p class="text-gray-600 text-sm mb-4">Oversees social services and community welfare programs.</p>
                                <button class="px-4 py-2 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                    Contact
                                </button>
                            </div>
                        </div>
                        
                        <div class="mt-8 text-center">
                            <button class="px-6 py-3 bg-blue-700 text-white rounded-md hover:bg-blue-800 transition">
                                View All Representatives
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Knowledge Hub Section -->
    <section id="knowledge" class="py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="max-w-5xl mx-auto">
                <div class="text-center mb-12 animate-fadeIn opacity-0">
                    <span class="inline-block px-4 py-1 bg-purple-100 text-purple-800 rounded-full text-sm font-medium mb-4">Educate</span>
                    <h2 class="text-3xl font-bold mb-4">Knowledge Hub</h2>
                    <p class="text-gray-600 max-w-2xl mx-auto">
                        Access a comprehensive library of government policies, laws, and public service information.
                    </p>
                </div>
                
                <div class="bg-white rounded-xl shadow-md overflow-hidden animate-fadeIn opacity-0 delay-100">
                    <div class="p-6">
                        <!-- Search and Filter -->
                        <div class="flex flex-col md:flex-row justify-between items-center mb-6 space-y-4 md:space-y-0 md:space-x-4">
                            <div class="relative w-full md:w-1/2">
                                <input type="text" class="pl-10 pr-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-purple-500 w-full" placeholder="Search documents, policies, laws...">
                                <div class="absolute left-3 top-2.5">
                                    <svg class="h-5 w-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path>
                                    </svg>
                                </div>
                            </div>
                            <div class="flex space-x-4 w-full md:w-auto">
                                <select class="px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-purple-500 w-full">
                                    <option>All Categories</option>
                                    <option>Laws & Regulations</option>
                                    <option>Government Policies</option>
                                    <option>Public Services Guides</option>
                                    <option>Reports & Publications</option>
                                </select>
                                <select class="px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-purple-500 w-full">
                                    <option>All Departments</option>
                                    <option>Ministry of Justice</option>
                                    <option>Ministry of Finance</option>
                                    <option>Federal Tax Authority</option>
                                    <option>Dubai Municipality</option>
                                </select>
                            </div>
                        </div>
                        
                        <!-- Document Cards -->
                        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200">
                                <div class="flex items-center mb-3">
                                    <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-purple-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="font-medium text-gray-800">Federal Law No. (1) of 2023</h4>
                                        <p class="text-sm text-gray-600">Digital Transactions Law</p>
                                    </div>
                                </div>
                                <p class="text-gray-600 text-sm mb-4">
                                    Regulates digital transactions, electronic signatures, and data protection in the UAE.
                                </p>
                                <div class="flex justify-between items-center">
                                    <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded">Laws & Regulations</span>
                                    <a href="#" class="text-sm text-purple-700 hover:text-purple-800">View Document</a>
                                </div>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200">
                                <div class="flex items-center mb-3">
                                    <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-purple-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="font-medium text-gray-800">UAE National Agenda 2030</h4>
                                        <p class="text-sm text-gray-600">Vision for a sustainable future</p>
                                    </div>
                                </div>
                                <p class="text-gray-600 text-sm mb-4">
                                    Outlines strategic objectives for economic, social, and environmental development.
                                </p>
                                <div class="flex justify-between items-center">
                                    <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded">Government Policies</span>
                                    <a href="#" class="text-sm text-purple-700 hover:text-purple-800">View Document</a>
                                </div>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200">
                                <div class="flex items-center mb-3">
                                    <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-purple-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H2v-2a3 3 0 015.356-1.857M17 20v-2c0-.185-.015-.368-.043-.546L16.5 16.5M2 17V6a2 2 0 012-2h16a2 2 0 012 2v11M10 10h.01M12 10h.01M14 10h.01M10 14h.01M12 14h.01M14 14h.01"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="font-medium text-gray-800">Guide to Starting a Business in UAE</h4>
                                        <p class="text-sm text-gray-600">Step-by-step guide for entrepreneurs</p>
                                    </div>
                                </div>
                                <p class="text-gray-600 text-sm mb-4">
                                    Comprehensive guide covering licensing, legal structures, and business regulations.
                                </p>
                                <div class="flex justify-between items-center">
                                    <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded">Public Services Guides</span>
                                    <a href="#" class="text-sm text-purple-700 hover:text-purple-800">View Document</a>
                                </div>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200">
                                <div class="flex items-center mb-3">
                                    <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-purple-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 17v-2m3 2v-4m3 4v-6m2 10H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="font-medium text-gray-800">Annual Economic Report 2022</h4>
                                        <p class="text-sm text-gray-600">Overview of UAE's economic performance</p>
                                    </div>
                                </div>
                                <p class="text-gray-600 text-sm mb-4">
                                    Detailed analysis of key economic indicators, sector performance, and future outlook.
                                </p>
                                <div class="flex justify-between items-center">
                                    <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded">Reports & Publications</span>
                                    <a href="#" class="text-sm text-purple-700 hover:text-purple-800">View Document</a>
                                </div>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200">
                                <div class="flex items-center mb-3">
                                    <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-purple-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.746 0 3.332.477 4.5 1.253v13C19.832 18.477 18.246 18 16.5 18s-3.332.477-4.5 1.253"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="font-medium text-gray-800">UAE Education Strategy 2030</h4>
                                        <p class="text-sm text-gray-600">Future of learning and development</p>
                                    </div>
                                </div>
                                <p class="text-gray-600 text-sm mb-4">
                                    Strategic framework for enhancing the quality and accessibility of education.
                                </p>
                                <div class="flex justify-between items-center">
                                    <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded">Government Policies</span>
                                    <a href="#" class="text-sm text-purple-700 hover:text-purple-800">View Document</a>
                                </div>
                            </div>
                            
                            <div class="bg-gray-50 rounded-lg p-6 border border-gray-200">
                                <div class="flex items-center mb-3">
                                    <div class="w-10 h-10 bg-purple-100 rounded-full flex items-center justify-center mr-3 flex-shrink-0">
                                        <svg class="w-5 h-5 text-purple-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3-.895 3-2-1.343-2-3-2zM21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z"></path>
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="font-medium text-gray-800">Public Health Guidelines</h4>
                                        <p class="text-sm text-gray-600">Health and safety protocols</p>
                                    </div>
                                </div>
                                <p class="text-gray-600 text-sm mb-4">
                                    Official guidelines and recommendations for maintaining public health and safety.
                                </p>
                                <div class="flex justify-between items-center">
                                    <span class="text-xs bg-purple-100 text-purple-800 px-2 py-1 rounded">Public Services Guides</span>
                                    <a href="#" class="text-sm text-purple-700 hover:text-purple-800">View Document</a>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-8 text-center">
                            <button class="px-6 py-3 bg-purple-700 text-white rounded-md hover:bg-purple-800 transition">
                                View All Documents
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-10">
        <div class="container mx-auto px-4 grid grid-cols-1 md:grid-cols-4 gap-8">
            <div>
                <h3 class="text-xl font-bold mb-4">Al-Majlis Al-Raqami</h3>
                <p class="text-gray-400 text-sm">
                    Bridging tradition with technology for a more engaged and connected community.
                </p>
                <div class="flex space-x-4 mt-4">
                    <a href="#" class="text-gray-400 hover:text-white">
                        <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.07 1.646.07 4.85s-.012 3.584-.07 4.85c-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.646.07-4.85.07s-3.584-.012-4.85-.07c-3.251-.148-4.77-1.691-4.919-4.919-.058-1.265-.07-1.646-.07-4.85s.012-3.584.07-4.85c.149-3.227 1.664-4.771 4.919-4.919 1.266-.058 1.646-.07 4.85-.07zm0-2.163c-3.259 0-3.667.014-4.947.072C2.79 0 0 2.79 0 7.057c0 1.28.014 1.688.072 4.947.058 3.259 2.849 5.04 4.947 5.04 1.28.058 1.688.072 4.947.072s3.667-.014 4.947-.072c2.098 0 4.889-1.781 4.947-5.04.058-1.28.072-1.688.072-4.947s-.014-3.667-.072-4.947C22.09 2.79 19.3 0 15.043 0c-1.28-.058-1.688-.072-4.947-.072zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.162 6.162 6.162 6.162-2.759 6.162-6.162-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4s1.791-4 4-4 4 1.79 4 4-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.44-.645 1.44-1.44s-.645-1.44-1.44-1.44z"></path>
                        </svg>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white">
                        <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M22.675 0H1.325C.593 0 0 .593 0 1.325v21.351C0 23.407.593 24 1.325 24h21.351c.732 0 1.325-.593 1.325-1.325V1.325C24 .593 23.407 0 22.675 0zM8.099 20.844H4.97V9.426h3.129v11.418zM6.534 8.11c-1.03 0-1.867-.837-1.867-1.867s.837-1.867 1.867-1.867 1.867.837 1.867 1.867-.837 1.867-1.867 1.867zM20.844 20.844h-3.129v-5.616c0-1.338-.024-3.064-1.867-3.064-1.868 0-2.155-1.458-2.155-2.984v-2.598h-3.129v11.418h3.129v-4.91c0-.32.006-.64.012-.96.024-.64.528-1.386 1.146-1.386.618 0 1.092.474 1.092 1.164v6.092h3.129z"></path>
                        </svg>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-white">
                        <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                            <path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.403 0-6.162 2.759-6.162 6.162 0 .483.055.953.15 1.404-5.133-.253-9.661-2.724-12.704-6.475-.526.9-.837 1.94-.837 3.062 0 2.134 1.086 4.021 2.74 5.125-.804-.025-1.56-.247-2.228-.616v.079c0 2.98 2.127 5.472 4.94 6.044-.52.139-1.06.214-1.61.214-.395 0-.778-.038-1.15-.109.782 2.443 3.06 4.222 5.796 4.262-2.09 1.64-4.724 2.625-7.59 2.625-.493 0-.978-.029-1.45-.085 2.704 1.737 5.929 2.752 9.39 2.752 11.26 0 17.41-9.353 17.41-17.41 0-.266-.006-.53-.015-.795.94-.679 1.758-1.537 2.413-2.517z"></path>
                        </svg>
                    </a>
                </div>
            </div>
            <div>
                <h3 class="text-lg font-bold mb-4">Quick Links</h3>
                <ul class="space-y-2 text-gray-400 text-sm">
                    <li><a href="#" class="hover:text-white">Home</a></li>
                    <li><a href="#" class="hover:text-white">Features</a></li>
                    <li><a href="#" class="hover:text-white">About Us</a></li>
                    <li><a href="#" class="hover:text-white">Contact Us</a></li>
                    <li><a href="#" class="hover:text-white">Privacy Policy</a></li>
                </ul>
            </div>
            <div>
                <h3 class="text-lg font-bold mb-4">Support</h3>
                <ul class="space-y-2 text-gray-400 text-sm">
                    <li><a href="#" class="hover:text-white">FAQ</a></li>
                    <li><a href="#" class="hover:text-white">Help Center</a></li>
                    <li><a href="#" class="hover:text-white">Terms of Service</a></li>
                    <li><a href="#" class="hover:text-white">Accessibility</a></li>
                </ul>
            </div>
            <div>
                <h3 class="text-lg font-bold mb-4">Contact Us</h3>
                <p class="text-gray-400 text-sm">
                    Sheikh Zayed Road, Dubai, UAE<br>
                    Email: info@almajlis.ae<br>
                    Phone: +971 4 123 4567
                </p>
            </div>
        </div>
        <div class="container mx-auto px-4 text-center text-gray-500 text-sm mt-10 border-t border-gray-700 pt-6">
            &copy; 2023 Al-Majlis Al-Raqami. All rights reserved.
        </div>
    </footer>

    <script>
        // Function to show announcement details
        function showAnnouncement(id) {
            alert(`Showing details for announcement ${id}. In a real application, this would fetch the full announcement from a server.`);
            // Example: window.location.href = `/announcements/${id}`;
        }

        // App download functionality
        document.getElementById('download-app').addEventListener('click', function() {
            alert('Thank you for downloading Al-Majlis Al-Raqami! You will be redirected to the app store.');
            // In a real implementation, you would redirect to actual app store links
            // window.location.href = 'https://play.google.com/store/apps/details?id=com.almajlis.raqami';
        });

        document.getElementById('download-app-mobile').addEventListener('click', function() {
            alert('Thank you for downloading Al-Majlis Al-Raqami! You will be redirected to the app store.');
            // window.location.href = 'https://play.google.com/store/apps/details?id=com.almajlis.raqami';
        });

        // Mobile menu toggle
        document.getElementById('menu-toggle').addEventListener('click', function() {
            document.getElementById('mobile-menu').classList.toggle('hidden');
        });

        // Feature tabs functionality
        document.querySelectorAll('.feature-tab').forEach(button => {
            button.addEventListener('click', () => {
                // Remove active class from all tabs and hide all content
                document.querySelectorAll('.feature-tab').forEach(btn => {
                    btn.classList.remove('active', 'bg-red-700', 'text-white', 'border-red-700');
                    btn.classList.add('text-gray-700', 'hover:text-red-700', 'border-transparent');
                });
                document.querySelectorAll('.feature-content').forEach(content => {
                    content.classList.remove('active');
                });

                // Add active class to clicked tab and show its content
                button.classList.add('active', 'bg-red-700', 'text-white', 'border-red-700');
                button.classList.remove('text-gray-700', 'hover:text-red-700', 'border-transparent');
                document.getElementById(button.dataset.tab + '-content').classList.add('active');
            });
        });

        // Voice Recording Functionality
        const startRecordingButton = document.getElementById('start-recording');
        const stopRecordingButton = document.getElementById('stop-recording');
        const playRecordingButton = document.getElementById('play-recording');
        const audioPlayback = document.getElementById('audio-playback');
        const voiceTimer = document.getElementById('voice-timer');
        const voiceProgressBar = document.getElementById('voice-progress-bar');
        const submitVoiceMajlisButton = document.getElementById('submit-voice-majlis');

        let mediaRecorder;
        let audioChunks = [];
        let audioBlob;
        let timerInterval;
        let startTime;

        startRecordingButton.addEventListener('click', async () => {
            try {
                const stream = await navigator.mediaDevices.getUserMedia({ audio: true });
                mediaRecorder = new MediaRecorder(stream);
                audioChunks = [];
                audioPlayback.classList.add('hidden'); // Hide playback during new recording
                audioPlayback.src = ''; // Clear previous recording

                mediaRecorder.ondataavailable = event => {
                    audioChunks.push(event.data);
                };

                mediaRecorder.onstop = () => {
                    audioBlob = new Blob(audioChunks, { type: 'audio/webm' });
                    const audioUrl = URL.createObjectURL(audioBlob);
                    audioPlayback.src = audioUrl;
                    audioPlayback.classList.remove('hidden');
                    playRecordingButton.disabled = false;
                    stopTimer();
                };

                mediaRecorder.start();
                startRecordingButton.disabled = true;
                stopRecordingButton.disabled = false;
                playRecordingButton.disabled = true; // Disable play while recording
                startTimer();
                voiceProgressBar.style.width = '0%'; // Reset progress bar
            } catch (err) {
                console.error('Error accessing microphone:', err);
                alert('Could not access microphone. Please ensure it is connected and permissions are granted.');
            }
        });

        stopRecordingButton.addEventListener('click', () => {
            if (mediaRecorder && mediaRecorder.state === 'recording') {
                mediaRecorder.stop();
                mediaRecorder.stream.getTracks().forEach(track => track.stop()); // Stop microphone access
                startRecordingButton.disabled = false;
                stopRecordingButton.disabled = true;
            }
        });

        playRecordingButton.addEventListener('click', () => {
            if (audioPlayback.src) {
                audioPlayback.play();
            }
        });

        submitVoiceMajlisButton.addEventListener('click', () => {
            if (audioBlob) {
                alert('Voice Majlis submitted successfully!');
                // Here you would typically send audioBlob to a server
                console.log('Submitting voice recording:', audioBlob);
                // Reset UI after submission
                audioPlayback.classList.add('hidden');
                audioPlayback.src = '';
                playRecordingButton.disabled = true;
                voiceTimer.textContent = '00:00';
                voiceProgressBar.style.width = '0%';
            } else {
                alert('Please record a voice message before submitting.');
            }
        });

        function startTimer() {
            startTime = Date.now();
            timerInterval = setInterval(() => {
                const elapsedTime = Date.now() - startTime;
                const seconds = Math.floor(elapsedTime / 1000);
                const minutes = Math.floor(seconds / 60);
                const remainingSeconds = seconds % 60;

                const formattedTime = `${String(minutes).padStart(2, '0')}:${String(remainingSeconds).padStart(2, '0')}`;
                voiceTimer.textContent = formattedTime;

                // Update progress bar (max 120 seconds for 2 minutes)
                const progress = (seconds / 120) * 100;
                voiceProgressBar.style.width = `${Math.min(progress, 100)}%`;

                if (seconds >= 120) {
                    stopRecordingButton.click(); // Automatically stop after 2 minutes
                }
            }, 1000);
        }

        function stopTimer() {
            clearInterval(timerInterval);
        }

        // Text Majlis Submission Alert
        document.getElementById('submit-text-majlis').addEventListener('click', () => {
            const subject = document.getElementById('subject').value;
            const message = document.getElementById('message').value;

            if (subject.trim() === '' || message.trim() === '') {
                alert('Please fill in both subject and message fields before submitting.');
            } else {
                alert('Text Majlis submitted successfully!');
                // Here you would typically send the text data to a server
                console.log('Submitting text:', { subject, message });
                // Optionally clear the form
                document.getElementById('subject').value = '';
                document.getElementById('message').value = '';
                document.querySelector('#text-majlis .form-checkbox').checked = true; // Reset anonymous checkbox
            }
        });
    </script>
</body>
</html>
