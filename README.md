<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Samir Guenchi | Code Quantum</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/tailwindcss/2.2.19/tailwind.min.css" rel="stylesheet">
    <style>
        body {
            background-color: #0a192f;
            color: #64ffda;
            font-family: 'Courier New', monospace;
        }
        .quantum-container {
            perspective: 1000px;
            transform-style: preserve-3d;
        }
        .quantum-orbit {
            position: absolute;
            border-radius: 50%;
            border: 2px solid rgba(100, 255, 218, 0.2);
            animation: rotate-orbit 20s linear infinite;
        }
        .quantum-particle {
            position: absolute;
            width: 15px;
            height: 15px;
            border-radius: 50%;
            background-color: #64ffda;
            box-shadow: 0 0 10px #64ffda;
            animation: quantum-pulse 2s ease-in-out infinite alternate;
        }
        @keyframes rotate-orbit {
            from { transform: rotateZ(0deg); }
            to { transform: rotateZ(360deg); }
        }
        @keyframes quantum-pulse {
            from { transform: scale(0.7); opacity: 0.6; }
            to { transform: scale(1.3); opacity: 1; }
        }
        .skill-particle {
            transition: all 0.3s ease;
        }
        .skill-particle:hover {
            transform: scale(1.5);
            background-color: #ff6b6b;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col items-center justify-center">
    <div class="quantum-container relative w-full h-screen">
        <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 text-center z-10">
            <h1 class="text-5xl font-bold mb-4">Samir Guenchi</h1>
            <p class="text-xl">Quantum Code Architect | Digital Alchemist</p>
        </div>

        <!-- Quantum Orbit System -->
        <div class="quantum-orbit absolute top-1/2 left-1/2 w-96 h-96 transform -translate-x-1/2 -translate-y-1/2">
            <div class="quantum-particle skill-particle" style="top: 0; left: 50%; transform: translateX(-50%);" data-skill="C++"></div>
        </div>
        <div class="quantum-orbit absolute top-1/2 left-1/2 w-64 h-64 transform -translate-x-1/2 -translate-y-1/2">
            <div class="quantum-particle skill-particle" style="top: 0; left: 50%; transform: translateX(-50%);" data-skill="Python"></div>
        </div>
        <div class="quantum-orbit absolute top-1/2 left-1/2 w-96 h-96 transform -translate-x-1/2 -translate-y-1/2 rotate-45">
            <div class="quantum-particle skill-particle" style="top: 0; left: 50%; transform: translateX(-50%);" data-skill="JavaScript"></div>
        </div>
        <div class="quantum-orbit absolute top-1/2 left-1/2 w-64 h-64 transform -translate-x-1/2 -translate-y-1/2 rotate-90">
            <div class="quantum-particle skill-particle" style="top: 0; left: 50%; transform: translateX(-50%);" data-skill="Linux"></div>
        </div>
    </div>

    <div class="absolute bottom-10 w-full text-center">
        <div class="inline-block bg-opacity-50 bg-black p-4 rounded-lg">
            <p class="text-sm">Current Project: choghl | Learning: Flutter & Kotlin</p>
            <div class="mt-4">
                <a href="mailto:samir.guenchi@ensia.edu.dz" class="mx-2 text-white hover:text-green-400">Contact</a>
                <a href="https://linkedin.com/in/your-linkedin" class="mx-2 text-white hover:text-green-400">LinkedIn</a>
                <a href="https://github.com/samir2022y" class="mx-2 text-white hover:text-green-400">GitHub</a>
            </div>
        </div>
    </div>

    <script>
        // Interactive particle hover effects
        document.querySelectorAll('.skill-particle').forEach(particle => {
            particle.addEventListener('mouseover', (e) => {
                const skill = e.target.getAttribute('data-skill');
                const infoBox = document.createElement('div');
                infoBox.className = 'absolute bg-black bg-opacity-70 p-2 rounded-lg text-white';
                infoBox.style.top = `${e.pageY + 10}px`;
                infoBox.style.left = `${e.pageX + 10}px`;
                infoBox.textContent = skill;
                document.body.appendChild(infoBox);

                e.target.addEventListener('mouseout', () => {
                    document.body.removeChild(infoBox);
                });
            });
        });
    </script>
</body>
</html>
