<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Michael Terranova | Senior ML Systems & Infrastructure Engineer</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- MathJax for rendering equations -->
    <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
    <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f0fdf4',
                            500: '#22c55e',
                            900: '#14532d',
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-slate-950 text-slate-100 font-sans antialiased selection:bg-brand-500 selection:text-slate-950">

    <!-- Navigation -->
    <nav class="sticky top-0 z-50 backdrop-blur-md bg-slate-950/80 border-b border-slate-800">
        <div class="max-w-5xl mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-lg font-bold tracking-tight text-white hover:text-brand-500 transition-colors">Michael Terranova</a>
            <div class="space-x-6 text-sm font-medium text-slate-400">
                <a href="#research" class="hover:text-white transition-colors">Research</a>
                <a href="#systems" class="hover:text-white transition-colors">Systems & Infra</a>
                <a href="#experience" class="hover:text-white transition-colors">Experience</a>
                <a href="https://github.com/michael2893" target="_blank" class="text-brand-500 hover:underline">GitHub ↗</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="max-w-5xl mx-auto px-6 py-20">
        <div class="inline-block px-3 py-1 mb-6 text-xs font-semibold tracking-wider text-brand-500 uppercase bg-brand-500/10 border border-brand-500/20 rounded-full">
            Senior ML Systems & Infrastructure Engineer
        </div>
        <h1 class="text-4xl md:text-6xl font-extrabold tracking-tight text-white mb-6 leading-tight">
            Bridging high-throughput distributed systems with applied machine learning & statistics.
        </h1>
        <p class="text-lg md:text-xl text-slate-400 max-w-3xl mb-8 leading-relaxed">
            Specializing in real-time streaming platforms (5M+ events/sec), ML feature infrastructure, and Bayesian statistical modeling. Currently pursuing an M.S. in Computer Science (Machine Learning Specialization) at Georgia Tech.
        </p>
        <div class="flex flex-wrap gap-4 text-sm font-medium">
            <a href="mailto:amt2893@gmail.com" class="px-5 py-2.5 bg-brand-500 text-slate-950 font-semibold rounded-lg hover:bg-brand-400 transition-colors">Contact Me</a>
            <a href="https://github.com/michael2893" target="_blank" class="px-5 py-2.5 bg-slate-900 border border-slate-800 text-slate-200 rounded-lg hover:border-slate-700 transition-colors">GitHub Profile</a>
            <a href="https://doi.org/10.5281/zenodo.20368030" target="_blank" class="px-5 py-2.5 bg-slate-900 border border-slate-800 text-slate-200 rounded-lg hover:border-slate-700 transition-colors">CDC Research DOI ↗</a>
        </div>
    </section>

    <!-- Research & Statistical Science Section -->
    <section id="research" class="max-w-5xl mx-auto px-6 py-16 border-t border-slate-800">
        <h2 class="text-2xl font-bold text-white mb-2">Research & Applied Statistics</h2>
        <p class="text-slate-400 mb-10">Statistical modeling, Bayesian inference, and quantitative analysis.</p>

        <div class="grid md:grid-cols-2 gap-8">
            <!-- Project 1: CDC Wastewater -->
            <div class="bg-slate-900/50 border border-slate-800 rounded-xl p-6 flex flex-col justify-between hover:border-slate-700 transition-colors">
                <div>
                    <div class="flex items-center justify-between mb-4">
                        <span class="text-xs font-mono text-brand-500">PyMC / MCMC / Hierarchical</span>
                        <span class="text-xs text-slate-500">DOI: 10.5281/zenodo.20368030</span>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-3">CDC Wastewater Surveillance Analysis</h3>
                    <p class="text-slate-400 text-sm mb-4 leading-relaxed">
                        Formulated hierarchical linear and Dirichlet regression models in PyMC to analyze SARS-CoV-2, Influenza-A, and RSV concentration data across 1,200+ CDC NWSS monitoring sites.
                    </p>
                    <div class="bg-slate-950 p-3 rounded border border-slate-800 text-xs font-mono text-slate-300 mb-4">
                        $$\beta_1 \text{ HDI: } [0.028, 0.153]$$<br>
                        Between-site variance exceeds between-state variance.
                    </div>
                </div>
                <a href="https://doi.org/10.5281/zenodo.20368030" target="_blank" class="text-xs text-brand-500 font-semibold hover:underline flex items-center gap-1">View Publication ↗</a>
            </div>

            <!-- Project 2: Quantitative Neuro  -->
            <div class="bg-slate-900/50 border border-slate-800 rounded-xl p-6 flex flex-col justify-between hover:border-slate-700 transition-colors">
                <div>
                    <div class="flex items-center justify-between mb-4">
                        <span class="text-xs font-mono text-brand-500">ANCOVA / Multivariate / Longitudinal</span>
                        <span class="text-xs text-slate-500">Primary Author</span>
                    </div>
                    <h3 class="text-xl font-bold text-white mb-3">Clinical Longitudinal Evaluative Fears Study</h3>
                    <p class="text-slate-400 text-sm mb-4 leading-relaxed">
                        Evaluated interactions between Social Anxiety (SA), Fear of Negative Evaluation (FNE), and Fear of Positive Evaluation (FPE) in clinical eating pathology across longitudinal follow-ups using ANCOVA modeling with baseline covariates.
                    </p>
                </div>
                <a href="https://github.com/michael2893/QuantitativeNeuro" target="_blank" class="text-xs text-brand-500 font-semibold hover:underline flex items-center gap-1">View QuantitativeNeuro Repo ↗</a>
            </div>
        </div>
    </section>

    <!-- ML Systems & Infrastructure Section -->
    <section id="systems" class="max-w-5xl mx-auto px-6 py-16 border-t border-slate-800">
        <h2 class="text-2xl font-bold text-white mb-2">ML Infrastructure & Distributed Systems</h2>
        <p class="text-slate-400 mb-10">Scaling real-time compute, streaming data, and ML feature platforms.</p>

        <div class="space-y-6">
            <!-- Shopify Stream -->
            <div class="bg-slate-900/50 border border-slate-800 rounded-xl p-6">
                <div class="flex flex-wrap justify-between items-start mb-2">
                    <h3 class="text-lg font-bold text-white">5M+ Events/Sec Real-Time Streaming & ML Platform Backfills</h3>
                    <span class="text-xs text-slate-500 font-mono">Shopify</span>
                </div>
                <p class="text-slate-400 text-sm leading-relaxed mb-4">
                    Designed a full-state backfill algorithm utilizing LTP bin-packing, work-stealing protocols, and AIMD congestion control, speeding up platform backfills by 4000%. Prototyped and deployed probabilistic load balancing algorithms and LLM-driven synthetic data generation pipelines.
                </p>
                <div class="flex flex-wrap gap-2 text-xs font-mono text-slate-400">
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">Flink</span>
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">Kafka</span>
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">Debezium</span>
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">Yugabyte</span>
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">Agentic Workflows</span>
                </div>
            </div>

            <!-- Wayfair Graph ML -->
            <div class="bg-slate-900/50 border border-slate-800 rounded-xl p-6">
                <div class="flex flex-wrap justify-between items-start mb-2">
                    <h3 class="text-lg font-bold text-white">Probabilistic Device Graph & ML Training Data Infrastructure</h3>
                    <span class="text-xs text-slate-500 font-mono">Wayfair</span>
                </div>
                <p class="text-slate-400 text-sm leading-relaxed mb-4">
                    Architected data infrastructure supporting 100s of TBs/day of ML training data. Optimized weakly connected components graph algorithms to construct device-customer association networks, resulting in a $15M revenue increase via personalized recommendation models.
                </p>
                <div class="flex flex-wrap gap-2 text-xs font-mono text-slate-400">
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">TigerGraph</span>
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">Neo4j</span>
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">Graph Algorithms</span>
                    <span class="px-2 py-1 bg-slate-950 rounded border border-slate-800">ML Training Data Platforms</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Education -->
    <section class="max-w-5xl mx-auto px-6 py-16 border-t border-slate-800">
        <h2 class="text-2xl font-bold text-white mb-6">Education & Academic Background</h2>
        <div class="grid md:grid-cols-2 gap-6">
            <div class="bg-slate-900/30 border border-slate-800 p-6 rounded-xl">
                <h3 class="text-lg font-bold text-white">Georgia Institute of Technology</h3>
                <p class="text-brand-500 text-sm mb-2">M.S. in Computer Science (Machine Learning Specialization) • Expected 2027</p>
                <p class="text-slate-400 text-xs leading-relaxed">Focus on Bayesian Statistics, Machine Learning, and Quantum Computing.</p>
            </div>
            <div class="bg-slate-900/30 border border-slate-800 p-6 rounded-xl">
                <h3 class="text-lg font-bold text-white">The Ohio State University</h3>
                <p class="text-brand-500 text-sm mb-2">B.S. Computational Neuroscience • B.A. Music • CS Minor</p>
                <p class="text-slate-400 text-xs leading-relaxed">Focus on PCA, k-means clustering, biophysical mathematical modeling, and neuro-imaging statistical analysis.</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="border-t border-slate-800 py-8 text-center text-xs text-slate-500">
        <p>© 2026 Michael Terranova. Hosted on GitHub Pages.</p>
    </footer>

</body>
</html>
