<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Visionary AI: Empowering Career Agency</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Chart.js -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

    <!-- Palette: Electric Indigo Future -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        primary: '#4338ca', // Indigo 700
                        secondary: '#06b6d4', // Cyan 500
                        accent: '#d946ef', // Fuchsia 500
                        dark: '#0f172a', // Slate 900
                        light: '#f8fafc', // Slate 50
                        surface: '#ffffff',
                    }
                }
            }
        }
    </script>

    <style>
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            height: 350px;
            max-height: 400px;
        }
        @media (max-width: 640px) {
            .chart-container { height: 300px; }
        }
        .glass-card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        /* Custom Scrollbar */
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #f1f1f1; }
        ::-webkit-scrollbar-thumb { background: #4338ca; border-radius: 4px; }
        ::-webkit-scrollbar-thumb:hover { background: #312e81; }
    </style>
</head>
<body class="bg-light text-dark font-sans leading-relaxed selection:bg-accent selection:text-white">

    <!-- Navigation -->
    <nav class="sticky top-0 z-50 bg-primary shadow-lg text-white py-3 px-6 flex justify-between items-center">
        <div class="font-bold text-xl tracking-tight"><i class="fa-solid fa-eye mr-2"></i> Visionary AI</div>
        <div class="hidden md:flex gap-6 text-sm font-medium">
            <a href="#problem" class="hover:text-cyan-300 transition">The Problem</a>
            <a href="#solution" class="hover:text-cyan-300 transition">The Solution</a>
            <a href="#impact" class="hover:text-cyan-300 transition">Impact</a>
            <a href="#budget" class="hover:text-cyan-300 transition">Budget</a>
        </div>
    </nav>

    <!-- Header -->
    <header class="relative bg-dark text-white py-20 px-6 text-center overflow-hidden">
        <div class="absolute inset-0 opacity-20 bg-[radial-gradient(ellipse_at_center,_var(--tw-gradient-stops))] from-secondary via-primary to-dark"></div>
        <div class="relative z-10 max-w-4xl mx-auto">
            <h1 class="text-5xl md:text-7xl font-extrabold mb-6 tracking-tight bg-clip-text text-transparent bg-gradient-to-r from-secondary to-accent">
                Empowering Career Agency
            </h1>
            <p class="text-xl md:text-2xl text-gray-300 mb-8 max-w-2xl mx-auto">
                A voice-driven intelligent companion transforming futures for visually impaired youth in Vietnam.
            </p>
            <div class="inline-flex items-center gap-2 bg-white/10 px-4 py-2 rounded-full text-sm font-semibold border border-white/20">
                <span class="w-3 h-3 bg-green-400 rounded-full animate-pulse"></span>
                Pilot Success: VAIEP 2024 (Tay Ninh)
            </div>
        </div>
    </header>

    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12 space-y-24">

        <!-- SECTION 1: THE PROBLEM -->
        <section id="problem">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-dark mb-4 border-b-4 border-secondary inline-block pb-2">The Paradox of Access</h2>
                <p class="text-gray-600 max-w-3xl mx-auto">
                    Despite global progress, employment rates for the visually impaired remain critically low due to systemic barriers in guidance and infrastructure.
                </p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <!-- Chart: Employment Gap -->
                <div class="bg-white rounded-xl shadow-lg p-6">
                    <h3 class="text-lg font-bold text-dark mb-4 flex items-center">
                        <i class="fa-solid fa-chart-simple text-secondary mr-2"></i> The Employment Gap (2023)
                    </h3>
                    <div class="chart-container">
                        <canvas id="employmentGapChart"></canvas>
                    </div>
                    <p class="text-xs text-center text-gray-400 mt-4 italic">Source: Vietnam Disability Survey & General Statistics Office</p>
                </div>
                
                <!-- Barriers Cards -->
                <div class="space-y-6">
                    <div class="flex items-start p-4 bg-white rounded-lg shadow-sm border-l-4 border-primary">
                        <div class="text-2xl text-primary mr-4"><i class="fa-solid fa-book-open"></i></div>
                        <div>
                            <h4 class="font-bold text-dark">Inaccessible Guidance</h4>
                            <p class="text-sm text-gray-600">Materials are visual-heavy. Lack of specialized tools forces student passivity.</p>
                        </div>
                    </div>
                    <div class="flex items-start p-4 bg-white rounded-lg shadow-sm border-l-4 border-secondary">
                        <div class="text-2xl text-secondary mr-4"><i class="fa-solid fa-users-slash"></i></div>
                        <div>
                            <h4 class="font-bold text-dark">Guidance Overload</h4>
                            <p class="text-sm text-gray-600">1:50 teacher-student ratio makes personalized counseling impossible.</p>
                        </div>
                    </div>
                    <div class="flex items-start p-4 bg-white rounded-lg shadow-sm border-l-4 border-accent">
                        <div class="text-2xl text-accent mr-4"><i class="fa-solid fa-link-slash"></i></div>
                        <div>
                            <h4 class="font-bold text-dark">Market Disconnect</h4>
                            <p class="text-sm text-gray-600">Lack of data on candidate potential creates an "invisible wall" for employers.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 2: THE SOLUTION -->
        <section id="solution" class="bg-dark text-white rounded-3xl p-8 md:p-12 relative overflow-hidden">
            <div class="absolute -top-24 -right-24 w-96 h-96 bg-primary opacity-20 rounded-full blur-3xl"></div>
            
            <div class="text-center mb-16 relative z-10">
                <h2 class="text-3xl md:text-4xl font-extrabold mb-4">A 4-Step Transformative Journey</h2>
                <p class="text-gray-300 max-w-2xl mx-auto">
                    Visionary AI acts as a technological springboard, guiding students from self-discovery to job readiness through a seamless voice interface.
                </p>
            </div>

            <!-- Process Flow -->
            <div class="grid grid-cols-1 md:grid-cols-4 gap-6 relative z-10">
                <div class="bg-white/10 p-6 rounded-xl border border-white/10 hover:bg-white/20 transition duration-300">
                    <div class="text-secondary font-bold text-xl mb-2">Step 1</div>
                    <h4 class="font-bold text-lg mb-2">Self-Discovery</h4>
                    <p class="text-sm text-gray-300">Holland Code voice tests to build a "Student Persona".</p>
                </div>
                <div class="bg-white/10 p-6 rounded-xl border border-white/10 hover:bg-white/20 transition duration-300">
                    <div class="text-accent font-bold text-xl mb-2">Step 2</div>
                    <h4 class="font-bold text-lg mb-2">Market Intel</h4>
                    <p class="text-sm text-gray-300">Explore 20+ career clusters, salaries & assistive tech.</p>
                </div>
                <div class="bg-white/10 p-6 rounded-xl border border-white/10 hover:bg-white/20 transition duration-300">
                    <div class="text-primary font-bold text-xl mb-2">Step 3</div>
                    <h4 class="font-bold text-lg mb-2">Action Planning</h4>
                    <p class="text-sm text-gray-300">AI synthesizes data for teachers to co-create IDPs.</p>
                </div>
                <div class="bg-white/10 p-6 rounded-xl border border-white/10 hover:bg-white/20 transition duration-300">
                    <div class="text-green-400 font-bold text-xl mb-2">Step 4</div>
                    <h4 class="font-bold text-lg mb-2">Job Readiness</h4>
                    <p class="text-sm text-gray-300">Mock Interviews (STAR method) & WCAG-compliant CVs.</p>
                </div>
            </div>
        </section>

        <!-- SECTION 3: IMPACT & OUTCOMES -->
        <section id="impact">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-dark mb-4">Measurable Impact</h2>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Efficiency Chart -->
                <div class="bg-white rounded-xl shadow-lg p-6 border-l-4 border-primary">
                    <h3 class="text-lg font-bold text-dark mb-2">Pedagogical Efficiency</h3>
                    <p class="text-sm text-gray-500 mb-6">Target: ≥ 85% reduction in administrative time (5 hours → 45 mins).</p>
                    <div class="chart-container">
                        <canvas id="efficiencyChart"></canvas>
                    </div>
                </div>

                <!-- Outcome Radar Chart -->
                <div class="bg-white rounded-xl shadow-lg p-6 border-l-4 border-accent">
                    <h3 class="text-lg font-bold text-dark mb-2">Student Competency Growth</h3>
                    <p class="text-sm text-gray-500 mb-6">Projected improvements across key readiness indicators.</p>
                    <div class="chart-container">
                        <canvas id="outcomeRadarChart"></canvas>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION 4: BUDGET & ROADMAP -->
        <section id="budget" class="grid grid-cols-1 lg:grid-cols-2 gap-12">
            <!-- Budget Breakdown -->
            <div class="bg-white rounded-2xl shadow-xl p-8">
                <h3 class="text-2xl font-bold text-dark mb-6 text-center">Total Project Value: $91,300</h3>
                <div class="chart-container mb-6">
                    <canvas id="budgetDonutChart"></canvas>
                </div>
                <div class="grid grid-cols-2 gap-4 text-xs text-gray-600">
                    <div class="flex items-center"><span class="w-3 h-3 rounded-full bg-indigo-700 mr-2"></span>Core Team (Shared): $30k</div>
                    <div class="flex items-center"><span class="w-3 h-3 rounded-full bg-cyan-500 mr-2"></span>Dev Agency: $18k</div>
                    <div class="flex items-center"><span class="w-3 h-3 rounded-full bg-fuchsia-500 mr-2"></span>Infra & AI: $8.5k</div>
                    <div class="flex items-center"><span class="w-3 h-3 rounded-full bg-orange-400 mr-2"></span>Hardware: $7.5k</div>
                    <div class="flex items-center"><span class="w-3 h-3 rounded-full bg-slate-400 mr-2"></span>Experts/Logistics: $27.3k</div>
                </div>
            </div>

            <!-- Roadmap -->
            <div class="bg-gray-50 rounded-2xl p-8 border border-gray-200">
                <h3 class="text-2xl font-bold text-dark mb-6">12-Month Roadmap</h3>
                <div class="space-y-8 relative before:absolute before:inset-0 before:ml-5 before:-translate-x-px md:before:mx-auto md:before:translate-x-0 before:h-full before:w-0.5 before:bg-gradient-to-b before:from-transparent before:via-slate-300 before:to-transparent">
                    <div class="relative flex items-center justify-between md:justify-normal md:odd:flex-row-reverse group is-active">
                        <div class="flex items-center justify-center w-10 h-10 rounded-full border border-white bg-slate-300 group-[.is-active]:bg-secondary text-slate-500 group-[.is-active]:text-white shadow shrink-0 md:order-1 md:group-odd:-translate-x-1/2 md:group-even:translate-x-1/2">
                            <i class="fa-solid fa-magnifying-glass text-xs"></i>
                        </div>
                        <div class="w-[calc(100%-4rem)] md:w-[calc(50%-2.5rem)] bg-white p-4 rounded border border-slate-200 shadow">
                            <div class="flex items-center justify-between space-x-2 mb-1">
                                <div class="font-bold text-slate-900">Phase 1 (Months 1-3)</div>
                            </div>
                            <div class="text-slate-500 text-xs">Empathy & Insight: Research, Success Profiles, DEI Consultations.</div>
                        </div>
                    </div>
                    <div class="relative flex items-center justify-between md:justify-normal md:odd:flex-row-reverse group is-active">
                        <div class="flex items-center justify-center w-10 h-10 rounded-full border border-white bg-slate-300 group-[.is-active]:bg-primary text-slate-500 group-[.is-active]:text-white shadow shrink-0 md:order-1 md:group-odd:-translate-x-1/2 md:group-even:translate-x-1/2">
                            <i class="fa-solid fa-code text-xs"></i>
                        </div>
                        <div class="w-[calc(100%-4rem)] md:w-[calc(50%-2.5rem)] bg-white p-4 rounded border border-slate-200 shadow">
                            <div class="flex items-center justify-between space-x-2 mb-1">
                                <div class="font-bold text-slate-900">Phase 2 (Months 4-9)</div>
                            </div>
                            <div class="text-slate-500 text-xs">Co-Design & Training: Prototyping, AI Fine-tuning, Pilot Testing (3 sites).</div>
                        </div>
                    </div>
                    <div class="relative flex items-center justify-between md:justify-normal md:odd:flex-row-reverse group is-active">
                        <div class="flex items-center justify-center w-10 h-10 rounded-full border border-white bg-slate-300 group-[.is-active]:bg-accent text-slate-500 group-[.is-active]:text-white shadow shrink-0 md:order-1 md:group-odd:-translate-x-1/2 md:group-even:translate-x-1/2">
                            <i class="fa-solid fa-rocket text-xs"></i>
                        </div>
                        <div class="w-[calc(100%-4rem)] md:w-[calc(50%-2.5rem)] bg-white p-4 rounded border border-slate-200 shadow">
                            <div class="flex items-center justify-between space-x-2 mb-1">
                                <div class="font-bold text-slate-900">Phase 3 (Months 10-12)</div>
                            </div>
                            <div class="text-slate-500 text-xs">Deployment & Scaling: Launch, Manual Packaging, Nationwide Expansion Plan.</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- CONCLUSION -->
        <section class="text-center py-16">
            <div class="max-w-3xl mx-auto p-10 border-2 border-dashed border-primary/30 rounded-3xl bg-indigo-50/50">
                <p class="text-xl md:text-2xl font-serif italic text-primary font-medium">
                    "When we empower a student to truly see their own potential, we finally help the world see it too."
                </p>
                <div class="mt-6 text-sm text-gray-500 uppercase tracking-widest font-bold">Visionary AI Team</div>
            </div>
        </section>

    </main>

    <!-- CHART.JS LOGIC -->
    <script>
        // Label Wrapping Utility
        function wrapLabel(label) {
            const words = label.split(' ');
            const lines = [];
            let currentLine = words[0];
            for (let i = 1; i < words.length; i++) {
                if (currentLine.length + 1 + words[i].length <= 16) {
                    currentLine += ' ' + words[i];
                } else {
                    lines.push(currentLine);
                    currentLine = words[i];
                }
            }
            lines.push(currentLine);
            return lines;
        }

        // Tooltip Config
        const tooltipConfig = {
            plugins: {
                tooltip: {
                    callbacks: {
                        title: function(tooltipItems) {
                            const item = tooltipItems[0];
                            let label = item.chart.data.labels[item.dataIndex];
                            return Array.isArray(label) ? label.join(' ') : label;
                        }
                    }
                }
            }
        };

        // 1. Employment Gap Chart
        const ctx1 = document.getElementById('employmentGapChart').getContext('2d');
        new Chart(ctx1, {
            type: 'bar',
            data: {
                labels: [wrapLabel('Visually Impaired'), wrapLabel('General Population')],
                datasets: [{
                    label: 'Employment Rate (%)',
                    data: [10, 76.3],
                    backgroundColor: ['#d946ef', '#4338ca'],
                    borderRadius: 8
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: { y: { beginAtZero: true, max: 100 } },
                ...tooltipConfig
            }
        });

        // 2. Efficiency Chart (Horizontal)
        const ctx2 = document.getElementById('efficiencyChart').getContext('2d');
        new Chart(ctx2, {
            type: 'bar',
            data: {
                labels: [['Traditional', 'Method'], ['With', 'Visionary AI']],
                datasets: [{
                    label: 'Minutes per Student',
                    data: [300, 45], // 5 hours vs 45 mins
                    backgroundColor: ['#94a3b8', '#06b6d4'],
                    borderRadius: 6
                }]
            },
            options: {
                indexAxis: 'y',
                responsive: true,
                maintainAspectRatio: false,
                ...tooltipConfig
            }
        });

        // 3. Outcome Radar
        const ctx3 = document.getElementById('outcomeRadarChart').getContext('2d');
        new Chart(ctx3, {
            type: 'radar',
            data: {
                labels: ['Confidence', 'Market Intel', 'Interview Skills', 'CV Quality', 'Tech Usage'],
                datasets: [{
                    label: 'Before',
                    data: [30, 20, 25, 30, 40],
                    fill: true,
                    backgroundColor: 'rgba(148, 163, 184, 0.2)',
                    borderColor: '#94a3b8',
                    pointBackgroundColor: '#94a3b8'
                }, {
                    label: 'After Pilot',
                    data: [80, 85, 80, 90, 85],
                    fill: true,
                    backgroundColor: 'rgba(67, 56, 202, 0.2)',
                    borderColor: '#4338ca',
                    pointBackgroundColor: '#4338ca'
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                ...tooltipConfig
            }
        });

        // 4. Budget Donut Chart (UPDATED)
        const ctx4 = document.getElementById('budgetDonutChart').getContext('2d');
        new Chart(ctx4, {
            type: 'doughnut',
            data: {
                labels: [
                    wrapLabel('Core Team (Shared)'),
                    wrapLabel('Development Agency'),
                    wrapLabel('Infra & AI'),
                    wrapLabel('Hardware'),
                    wrapLabel('Experts & Logistics')
                ],
                datasets: [{
                    data: [30000, 18000, 8500, 7500, 27300],
                    backgroundColor: ['#4338ca', '#06b6d4', '#d946ef', '#fb923c', '#94a3b8'],
                    borderWidth: 0
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: { position: 'bottom' },
                    ...tooltipConfig.plugins
                }
            }
        });
    </script>
</body>
</html>
