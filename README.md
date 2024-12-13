<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Samir Guenchi | Computational Science Professional</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/tailwindcss/2.2.19/tailwind.min.css" rel="stylesheet">
    <style>
        body {
            background-color: #0a192f;
            color: #64ffda;
            font-family: 'Courier New', monospace;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        .skill-bar {
            animation: fadeIn 1s ease-out;
        }
        .skill-icon {
            transition: all 0.3s ease;
        }
        .skill-icon:hover {
            transform: scale(1.2);
            filter: brightness(1.2);
        }
        .animated-text {
            animation: fadeIn 1.5s ease-out;
        }
        .pulse-effect {
            animation: pulse 2s infinite;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col items-center justify-center p-4">
    <div class="container mx-auto max-w-4xl">
        <div class="text-center animated-text">
            <h1 class="text-5xl font-bold mb-4 text-white">Samir Guenchi</h1>
            <p class="text-2xl mb-8">Computational Science | AI Research | Competitive Programming</p>
        </div>

        <div class="grid md:grid-cols-2 gap-8">
            <div class="bg-gray-800 p-6 rounded-lg animated-text">
                <h2 class="text-2xl font-semibold mb-4 text-white">Professional Profile</h2>
                <p class="text-gray-300">
                    Interdisciplinary researcher specializing in the intersection of applied mathematics, 
                    artificial intelligence, and computational physics. Demonstrated expertise in 
                    developing advanced algorithmic solutions.
                </p>
            </div>

            <div class="bg-gray-800 p-6 rounded-lg">
                <h2 class="text-2xl font-semibold mb-4 text-white">Skill Proficiency</h2>
                <div class="space-y-4">
                    <div class="skill-bar">
                        <div class="flex justify-between mb-1">
                            <span class="text-white">Competitive Programming</span>
                            <span class="text-white">90%</span>
                        </div>
                        <div class="w-full bg-gray-700 rounded-full h-2.5">
                            <div class="bg-green-500 h-2.5 rounded-full" style="width: 90%"></div>
                        </div>
                    </div>
                    <div class="skill-bar">
                        <div class="flex justify-between mb-1">
                            <span class="text-white">Machine Learning</span>
                            <span class="text-white">80%</span>
                        </div>
                        <div class="w-full bg-gray-700 rounded-full h-2.5">
                            <div class="bg-blue-500 h-2.5 rounded-full" style="width: 80%"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="mt-8 text-center">
            <h2 class="text-3xl font-bold mb-6 text-white">Technology Stack</h2>
            <div class="flex flex-wrap justify-center gap-6">
                <img src="https://skillicons.dev/icons?i=cpp,python,pytorch,tensorflow,matlab,linux,git" 
                     alt="Technology Stack" 
                     class="skill-icon w-16 h-16 transform hover:scale-125 transition-transform"/>
            </div>
        </div>

        <div class="mt-8 text-center">
            <h2 class="text-3xl font-bold mb-6 text-white">GitHub Statistics</h2>
            <div class="flex flex-wrap justify-center gap-4">
                <img src="https://github-readme-stats.vercel.app/api?username=samir2022y&theme=dark&show_icons=true" 
                     alt="GitHub Stats" 
                     class="pulse-effect max-w-full"/>
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=samir2022y&theme=dark&layout=compact" 
                     alt="Top Languages" 
                     class="pulse-effect max-w-full"/>
            </div>
        </div>

        <div class="mt-8 text-center">
            <h2 class="text-3xl font-bold mb-6 text-white">Connect With Me</h2>
            <div class="flex justify-center space-x-4">
                <a href="mailto:samir.guenchi@ensia.edu.dz" class="text-white hover:text-green-400 text-lg">
                    Email
                </a>
                <a href="https://linkedin.com/in/your-linkedin" class="text-white hover:text-green-400 text-lg">
                    LinkedIn
                </a>
                <a href="https://github.com/samir2022y" class="text-white hover:text-green-400 text-lg">
                    GitHub
                </a>
            </div>
        </div>
    </div>
</body>
</html>
