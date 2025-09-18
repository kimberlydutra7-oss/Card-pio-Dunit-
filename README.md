<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cardápio - Dunitê Sorvetes e Açaí</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lobster&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #1a1a1a;
        }
        .font-lobster {
            font-family: 'Lobster', cursive;
        }
        .card {
            background-color: rgba(30, 30, 30, 0.8);
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.4);
        }
        .flavor-item {
            transition: color 0.3s ease, transform 0.3s ease;
            cursor: default; /* Mudei para default, já que não é clicável */
        }
        .flavor-item:hover {
            color: #f472b6; /* Pink-400 */
            transform: translateX(5px);
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .fade-in {
            animation: fadeIn 0.8s ease-out forwards;
        }
    </style>
</head>
<body class="text-gray-200">
    <div class="relative min-h-screen bg-cover bg-center bg-fixed" style="background-image: url('https://images.unsplash.com/photo-1563805042-762955214838?q=80&w=2574&auto=format&fit=crop');">
        
        <div class="absolute inset-0 bg-black/70"></div>
        
        <div class="relative container mx-auto p-4 sm:p-8">
            <header class="text-center py-12 fade-in">
                <h1 class="font-lobster text-6xl md:text-8xl text-white tracking-wider" style="text-shadow: 0 0 15px rgba(255,105,180,0.7), 0 0 5px rgba(255,255,255,0.7);">Dunitê</h1>
                <p class="text-xl md:text-2xl mt-4 text-pink-300 font-light">Sorvetes e Açaí</p>
                <p class="text-lg md:text-xl mt-2 text-gray-300 font-light">Onde cada colherada é uma celebração!</p>
            </header>

            <main class="max-w-4xl mx-auto space-y-12">
                <section class="card rounded-2xl shadow-xl p-6 md:p-8 fade-in" style="animation-delay: 0.2s;">
                    <h2 class="font-lobster text-4xl text-center text-pink-400 mb-4">Nossas Obras de Arte Geladas</h2>
                    <p class="text-center text-gray-400 mb-8 max-w-2xl mx-auto">Uma seleção exclusiva de sabores, criados para transformar seu dia. Mergulhe nesta experiência cremosa!</p>
                    
                    <ul class="grid grid-cols-2 md:grid-cols-3 gap-x-8 gap-y-4 text-lg mb-10">
                        <li class="flavor-item">Charge</li>
                        <li class="flavor-item">Flocos</li>
                        <li class="flavor-item">Kalaque</li>
                        <li class="flavor-item">Cookies</li>
                        <li class="flavor-item">Kit Kat</li>
                        <li class="flavor-item">Chiclete</li>
                        <li class="flavor-item">Blue Ice</li>
                        <li class="flavor-item">Crocante</li>
                        <li class="flavor-item">Baunilha</li>
                        <li class="flavor-item">Mocacino</li>
                        <li class="flavor-item">Tentação</li>
                        <li class="flavor-item">Chocolate</li>
                        <li class="flavor-item">Kinder Ovo</li>
                        <li class="flavor-item">Milho Verde</li>
                        <li class="flavor-item">Ovomaltine</li>
                        <li class="flavor-item">Chocomenta</li>
                        <li class="flavor-item">Café Trufado</li>
                        <li class="flavor-item">Dois Amores</li>
                        <li class="flavor-item">Torta Alemã</li>
                        <li class="flavor-item">Torta de Limão</li>
                        <li class="flavor-item">Diamante Negro</li>
                        <li class="flavor-item">Floresta Negra</li>
                        <li class="flavor-item">Abacaxi Francês</li>
                        <li class="flavor-item">Maracujá</li>
                        <li class="flavor-item">Pavê Creme de Valsa</li>
                        <li class="flavor-item">Grego Frutas Vermelhas</li>
                        <li class="flavor-item">Brigadeiro com Beijinho</li>
                        <li class="flavor-item">Morango com Leite Cond.</li>
                    </ul>

                    <h3 class="text-2xl font-semibold text-white border-b-2 border-pink-400/50 pb-2 mb-6">Finalize com Coberturas Especiais:</h3>
                    <p class="text-center text-gray-400 mb-6 -mt-4">Um toque extra de sabor para o seu sorvete ou açaí!</p>
                    <ul class="grid grid-cols-2 md:grid-cols-4 gap-x-8 gap-y-4 text-lg">
                        <li class="flavor-item">Morango</li>
                        <li class="flavor-item">Menta</li>
                        <li class="flavor-item">Frutas Vermelhas</li>
                        <li class="flavor-item">Chocolate</li>
                        <li class="flavor-item">Cereja</li>
                        <li class="flavor-item">Caramelo</li>
                        <li class="flavor-item">Limão</li>
                        <li class="flavor-item">Tuttifruti</li>
                    </ul>
                </section>

                <section class="card rounded-2xl shadow-xl p-6 md:p-8 fade-in" style="animation-delay: 0.4s;">
                     <h2 class="font-lobster text-4xl text-center text-purple-400 mb-4">Cremes & Sonhos no Canudo</h2>
                     <p class="text-center text-gray-400 mb-6 max-w-2xl mx-auto">Seu sabor de sorvete favorito, transformado em um milk shake incrivelmente cremoso e irresistível. Qual vai ser a sua mistura hoje?</p>
                     <div class="text-center">
                         <p class="text-xl font-semibold">Todos os sabores de sorvete estão disponíveis!</p>
                         <p class="text-gray-300 mt-1">Da ousadia do <span class="text-purple-300 font-medium">Kinder Ovo</span> à nostalgia do <span class="text-purple-300 font-medium">Chiclete</span>.</p>
                     </div>
                </section>

                <section class="card rounded-2xl shadow-xl p-6 md:p-8 fade-in" style="animation-delay: 0.6s;">
                    <h2 class="font-lobster text-4xl text-center text-indigo-400 mb-4">Monte seu Açaí da Felicidade</h2>
                    <p class="text-center text-gray-400 mb-8 max-w-2xl mx-auto">Comece com a energia contagiante do nosso açaí puro e finalize com seus acompanhamentos preferidos. A arte é toda sua!</p>
                    
                    <div class="max-w-md mx-auto space-y-3 text-lg mb-8">
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2">
                            <span class="font-semibold">Copo 330ml</span>
                            <span class="font-semibold text-indigo-300">R$ 15,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2">
                            <span class="font-semibold">Copo 400ml</span>
                            <span class="font-semibold text-indigo-300">R$ 18,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2">
                            <span class="font-semibold">Copo 500ml</span>
                            <span class="font-semibold text-indigo-300">R$ 20,00</span>
                        </div>
                    </div>

                    <h3 class="text-2xl font-semibold text-white border-b-2 border-indigo-400/50 pb-2 mb-6">Turbine com Adicionais:</h3>
                    <div class="space-y-6">
                        <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Frutas</h4>
                            <ul class="grid grid-cols-2 md:grid-cols-4 gap-x-8 gap-y-3 text-lg">
                                <li class="flavor-item">Uva</li>
                                <li class="flavor-item">Morango</li>
                                <li class="flavor-item">Maçã</li>
                                <li class="flavor-item">Banana</li>
                                <li class="flavor-item">Kiwi</li>
                            </ul>
                        </div>
                        <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Cremes & Caldas</h4>
                            <ul class="grid grid-cols-2 md:grid-cols-3 gap-x-8 gap-y-3 text-lg">
                                <li class="flavor-item">Nutella</li>
                                <li class="flavor-item">Leite Condensado</li>
                                <li class="flavor-item">Creme de Leite Ninho</li>
                                <li class="flavor-item">Creme de Pistache</li>
                                <li class="flavor-item">Creme de Ovomaltine</li>
                            </ul>
                        </div>
                         <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Doces & Chocolates</h4>
                            <ul class="grid grid-cols-2 md:grid-cols-3 gap-x-8 gap-y-3 text-lg">
                                <li class="flavor-item">Cookie</li>
                                <li class="flavor-item">Bis</li>
                                <li class="flavor-item">Confete</li>
                                <li class="flavor-item">Bombom</li>
                                <li class="flavor-item">Suflair</li>
                                <li class="flavor-item">KitKat</li>
                                <li class="flavor-item">Gotas de Chocolate</li>
                                <li class="flavor-item">Raspas de Chocolate</li>
                                <li class="flavor-item">Chocoballs (Misto)</li>
                            </ul>
                        </div>
                         <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Secos & Pós</h4>
                            <ul class="grid grid-cols-2 md:grid-cols-4 gap-x-8 gap-y-3 text-lg">
                                <li class="flavor-item">Leite Ninho</li>
                                <li class="flavor-item">Paçoca</li>
                                <li class="flavor-item">Granola</li>
                                <li class="flavor-item">Castanha</li>
                                <li class="flavor-item">Kibbles</li>
                                <li class="flavor-item">Granulado</li>
                            </ul>
                        </div>
                        <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Guloseimas</h4>
                            <ul class="grid grid-cols-2 md:grid-cols-4 gap-x-8 gap-y-3 text-lg">
                                <li class="flavor-item">Fini Banana</li>
                                <li class="flavor-item">Fini Amora</li>
                                <li class="flavor-item">Fini Dentadura</li>
                                <li class="flavor-item">Fini Jujuba</li>
                            </ul>
                        </div>
                    </div>
                </section>
            </main>

            <footer class="text-center mt-16 pb-8 fade-in" style="animation-delay: 0.8s;">
                <p class="text-gray-400 text-sm">Dunitê Sorvetes e Açaí - Criando momentos doces desde sempre.</p>
                <p class="text-xs text-gray-500 mt-2">Osvaldo Cruz, SP - 2025</p>
            </footer>
        </div>
    </div>
</body>
</html>
