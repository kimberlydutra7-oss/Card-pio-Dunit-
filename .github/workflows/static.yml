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
        .flavor-item-list,
        .price-item { /* Adicionamos price-item para ser clicável */
            transition: color 0.3s ease, transform 0.3s ease, background-color 0.3s ease;
            cursor: pointer; /* Mudar para cursor: pointer indica que o item é clicável */
        }
        .flavor-item-list:hover {
            color: #f472b6; /* Pink-400 */
            transform: translateX(5px);
        }
        .price-item:hover {
            background-color: rgba(255, 255, 255, 0.05);
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .fade-in {
            animation: fadeIn 0.8s ease-out forwards;
        }

        /* Estilos do Modal (Balão) */
        .modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            display: none; /* Inicia oculto */
            justify-content: center;
            align-items: center;
            z-index: 100; /* Garante que fique acima de tudo */
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        .modal.open {
            display: flex;
            opacity: 1;
        }
        .modal-content {
            background-color: #2a2a2a;
            padding: 1.5rem;
            border-radius: 1rem;
            max-width: 90%;
            max-height: 90%;
            overflow-y: auto;
            position: relative;
            transform: scale(0.8);
            transition: transform 0.3s ease;
        }
        .modal.open .modal-content {
            transform: scale(1);
        }
        .close-button {
            position: absolute;
            top: 10px;
            right: 15px;
            font-size: 2rem;
            color: #fff;
            cursor: pointer;
            transition: color 0.2s;
        }
        .close-button:hover {
            color: #f472b6;
        }
        .modal-image {
            max-width: 100%;
            height: auto;
            border-radius: 0.5rem;
        }
    </style>
</head>
<body class="text-gray-200">
    <div class="relative min-h-screen bg-cover bg-center bg-fixed" style="background-image: url('https://images.unsplash.com/photo-1563805042-762955214838?q=80&w=2574&auto=format&fit=crop');">
        
        <div class="absolute inset-0 bg-black/70"></div        <!-- Todo o conteúdo está em um container relativo para aparecer acima da camada -->
        <div class="relative container mx-auto p-4 sm:p-8">
            <header class="text-center py-12 fade-in">
                <h1 class="font-lobster text-6xl md:text-8xl text-white tracking-wider" style="text-shadow: 0 0 15px rgba(255,105,180,0.7), 0 0 5px rgba(255,255,255,0.7);">Dunitê</h1                <p class="text-xl md:text-2xl mt-4 text-pink-300 font-light">Sorvetes e Açaí</p>
                <p class="text-xl md:text-2xl mt-4 text-pink-300 font-light">Onde cada colherada é uma celebração!</p>
            </header>

            <main class="max-w-4xl mx-auto space-y-12">
            <main class="max-w-4xl mx-auto space-y-12">
                
                <section class="card rounded-2xl shadow-xl p-6 md:p-8 fade-in" style="animation-delay: 0.1s;">
                    <h2 class="font-lobster text-4xl text-center text-pink-400 mb-4">Nossas Obras de Arte Geladas</h2>
                    <p class="text-center text-gray-400 mb-8 max-w-2xl mx-auto">Uma seleção exclusiva de sabores, criados para transformar seu dia. Mergulhe nesta experiência cremosa!</p>
                    
                    <ul class="grid grid-cols-2 md:grid-cols-3 gap-x-8 gap-y-4 text-lg mb-10">
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Charge">Charge</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Flocos">Flocos</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Kalaque">Kalaque</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Cookies">Cookies</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Kit+Kat">Kit Kat</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Chiclete">Chiclete</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Blue+Ice">Blue Ice</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Crocante">Crocante</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Baunilha">Baunilha</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Mocacino">Mocacino</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Tentacao">Tentação</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Chocolate">Chocolate</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Kinder+Ovo">Kinder Ovo</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Milho+Verde">Milho Verde</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Ovomaltine">Ovomaltine</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Chocomenta">Chocomenta</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Cafe+Trufado">Café Trufado</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Dois+Amores">Dois Amores</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Torta+Alema">Torta Alemã</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Torta+de+Limão">Torta de Limão</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Diamante+Negro">Diamante Negro</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Floresta+Negra">Floresta Negra</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Abacaxi+Frances">Abacaxi Francês</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Maracuja">Maracujá</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Pave+Creme+de+Valsa">Pavê Creme de Valsa</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Brigadeiro+com+Beijinho">Brigadeiro com Beijinho</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Sorvete+Morango+com+Leite+Cond">Morango com Leite Cond.</li>
                    </ul>

                    <h3 class="text-2xl font-semibold text-white border-b-2 border-pink-400/50 pb-2 mb-6">Finalize com Coberturas Especiais:</h3>
                    <p class="text-center text-gray-400 mb-6 -mt-4">Um toque extra de sabor para o seu sorvete ou açaí!</p>
                    <ul class="grid grid-cols-2 md:grid-cols-4 gap-x-8 gap-y-4 text-lg">
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cobertura+Morango">Morango</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cobertura+Menta">Menta</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cobertura+Frutas+Vermelhas">Frutas Vermelhas</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cobertura+Chocolate">Chocolate</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cobertura+Cereja">Cereja</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cobertura+Caramelo">Caramelo</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cobertura+Limão">Limão</li>
                        <li class="flavor-item-list" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cobertura+Tuttifruti">Tuttifruti</li>
                    </ul>
                </section>
                
                <section class="card rounded-2xl shadow-xl p-6 md:p-8 fade-in" style="animation-delay: 0.2s;">
                    <h2 class="font-lobster text-4xl text-center text-yellow-400 mb-4">Nossas Casquinhas Crocantes</h2>
                    <p class="text-center text-gray-400 mb-8 max-w-2xl mx-auto">A forma mais clássica e crocante de saborear o seu sorvete. Escolha a sua!</p>
                    
                    <div class="max-w-md mx-auto space-y-3 text-lg">
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text= Casquinha Simples (1 Bola)">
                            <span class="font-semibold text-gray-300">Casquinha Simples (1 Bola)</span>
                            <span class="font-semibold text-yellow-300">R$ 8,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text= Cascão Uni (1 Bola e Cobertura)">
                            <span class="font-semibold text-gray-300">Cascão Uni (1 Bola e Cobertura)</span>
                            <span class="font-semibold text-yellow-300">R$10,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text= Cascão Duni (2 Bolas e Cobertura)">
                            <span class="font-semibold text-gray-300"> Cascão Duni (2 Bolas e Cobertura)</span>
                            <span class="font-semibold text-yellow-300">R$ 12,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text= Cestinha com 3 Bolas">
                            <span class="font-semibold text-gray-300">Cestinha com 3 Bolas</span>
                            <span class="font-semibold text-yellow-300">R$ 15,00</span>
                        </div>
                        <div class="flex justify-between items-center pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Cestinha com 4 Bolas">
                            <span class="font-semibold text-gray-300">Cestinha com 4 Bolas</span>
                            <span class="font-semibold text-yellow-300">R$ 16,00</span>
                        </div>
                    </div>
                </section>

                <section class="card rounded-2xl shadow-xl p-6 md:p-8 fade-in" style="animation-delay: 0.4s;">
                    <h2 class="font-lobster text-4xl text-center text-purple-400 mb-4">Cremes & Sonhos no Canudo</h2>
                    <p class="text-center text-gray-400 mb-6 max-w-2xl mx-auto">Seu sabor de sorvete favorito, transformado em um milk shake incrivelmente cremoso e irresistível.</p>
                    
                    <div class="text-center mb-8">
                        <p class="text-xl font-semibold">Disponível em todos os sabores de sorvete!</p>
                        <p class="text-gray-300 mt-1">Da ousadia do <span class="text-purple-300 font-medium">Kinder Ovo</span> à nostalgia do <span class="text-purple-300 font-medium">Chiclete</span>.</p>
                    </div>

                    <div class="max-w-md mx-auto space-y-3 text-lg">
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Milk+Shake+P">
                            <span class="font-semibold">Duni Shake P (300ml)</span>
                            <span class="font-semibold text-purple-300">R$ 18,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Milk+Shake+M">
                            <span class="font-semibold"> Duni Shake M (400ml)</span>
                            <span class="font-semibold text-purple-300">R$ 20,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Milk+Shake+G">
                            <span class="font-semibold"> Duni Shake G (500ml)</span>
                            <span class="font-semibold text-purple-300">R$ 22,00</span>
                        </div>
                        <div class="flex justify-between items-center pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Milk+Shake+GG">
                            <span class="font-semibold">Duni Shake Do Snowy</span>
                            <span class="font-semibold text-purple-300">R$ 40,00</span>
                        </div>
                    </div>
                </section>

                <section class="card rounded-2xl shadow-xl p-6 md:p-8 fade-in" style="animation-delay: 0.6s;">
                    <h2 class="font-lobster text-4xl text-center text-indigo-400 mb-4">Monte seu Açaí da Felicidade</h2>
                    <p class="text-center text-gray-400 mb-8 max-w-2xl mx-auto">Comece com a energia contagiante do nosso açaí puro e finalize com seus acompanhamentos preferidos. A arte é toda sua!</p>
                    
                    <h3 class="text-2xl font-semibold text-white border-b-2 border-indigo-400/50 pb-2 mb-6">Tamanhos Base Açaí:</h3>
                    <div class="max-w-md mx-auto space-y-3 text-lg mb-8">
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Açai+330ml">
                            <span class="font-semibold">Copo 330ml</span>
                            <span class="font-semibold text-indigo-300">R$ 15,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Açai+400ml">
                            <span class="font-semibold">Copo 440ml</span>
                            <span class="font-semibold text-indigo-300">R$ 18,00</span>
                        </div>
                        <div class="flex justify-between items-center border-b border-gray-700 pb-2 price-item" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Açai+500ml">
                            <span class="font-semibold">Copo 550ml</span>
                            <span class="font-semibold text-indigo-300">R$ 20,00</span>
                        </div>
                    </div>

                    <h3 class="text-2xl font-semibold text-white border-b-2 border-indigo-400/50 pb-2 mb-6">Turbine com Adicionais:</h3>
                    <div class="space-y-6">
                        
                        <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Frutas</h4>
                            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 gap-x-8 gap-y-3 text-lg">
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Uva">
                                    <span class="text-gray-300">Uva</span>
                                    <span class="text-indigo-300">R$ 3,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Morango">
                                    <span class="text-gray-300">Morango</span>
                                    <span class="text-indigo-300">R$ 4,50</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Maca">
                                    <span class="text-gray-300">Maçã</span>
                                    <span class="text-indigo-300">R$ 3,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Banana">
                                    <span class="text-gray-300">Banana</span>
                                    <span class="text-indigo-300">R$ 3,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Kiwi">
                                    <span class="text-gray-300">Kiwi</span>
                                    <span class="text-indigo-300">R$ 5,00</span>
                                </div>
                            </div>
                        </div>
                        
                        <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Cremes & Caldas</h4>
                            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 gap-x-8 gap-y-3 text-lg">
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Nutella">
                                    <span class="text-gray-300">Nutella</span>
                                    <span class="text-indigo-300">R$ 6,50</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Leite+Condensado">
                                    <span class="text-gray-300">Leite Condensado</span>
                                    <span class="text-indigo-300">R$ 3,50</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Creme+Ninho">
                                    <span class="text-gray-300">Creme de Leite Ninho</span>
                                    <span class="text-indigo-300">R$ 4,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Creme+Pistache">
                                    <span class="text-gray-300">Creme de Pistache</span>
                                    <span class="text-indigo-300">R$ 6,50</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Creme+Ovomaltine">
                                    <span class="text-gray-300">Creme de Ovomaltine</span>
                                    <span class="text-indigo-300">R$ 6,00</span>
                                </div>
                            </div>
                        </div>
                        
                        <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Doces & Chocolates</h4>
                            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 gap-x-8 gap-y-3 text-lg">
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Cookie">
                                    <span class="text-gray-300">Cookie</span>
                                    <span class="text-indigo-300">R$ 4,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Bis">
                                    <span class="text-gray-300">Bis</span>
                                    <span class="text-indigo-300">R$ 2,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Marshmellow">
                                    <span class="text-gray-300">Marshmellow</span>
                                    <span class="text-indigo-300">R$ 2,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Confete">
                                    <span class="text-gray-300">Confete</span>
                                    <span class="text-indigo-300">R$ 3,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Kit Kat">
                                    <span class="text-gray-300">Kit Kat</span>
                                    <span class="text-indigo-300">R$ 4,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Chocoball Misto">
                                    <span class="text-gray-300">Chocoball Misto</span>
                                    <span class="text-indigo-300">R$ 3,50</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Chocoball Chocolate">
                                    <span class="text-gray-300">Chocoball Chocolate</span>
                                    <span class="text-indigo-300">R$ 3,50</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+ Gotas de Chocolate">
                                    <span class="text-gray-300">Gotas de Chocolate</span>
                                    <span class="text-indigo-300">R$ 3,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Raspas+Chocolate">
                                    <span class="text-gray-300">Raspas de Chocolate</span>
                                    <span class="text-indigo-300">R$ 1,50</span>
                                </div>
                            </div>
                        </div>
                        
                        <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Secos & Pós</h4>
                            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 gap-x-8 gap-y-3 text-lg">
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Leite+Ninho">
                                    <span class="text-gray-300">Leite Ninho</span>
                                    <span class="text-indigo-300">R$ 4,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Paçoca">
                                    <span class="text-gray-300">Paçoca</span>
                                    <span class="text-indigo-300">R$ 3,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Granola">
                                    <span class="text-gray-300">Granola</span>
                                    <span class="text-indigo-300">R$ 3,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Granulado">
                                    <span class="text-gray-300">Granulado</span>
                                    <span class="text-indigo-300">R$ 1,50</span>
                                </div>
                            </div>
                        </div>
                        
                        <div>
                            <h4 class="text-xl font-semibold text-indigo-300 mb-3">Guloseimas</h4>
                            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-2 gap-x-8 gap-y-3 text-lg">
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Fini+Banana">
                                    <span class="text-gray-300">Fini Banana</span>
                                    <span class="text-indigo-300">R$ 4,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Fini+Amora">
                                    <span class="text-gray-300">Fini Amora</span>
                                    <span class="text-indigo-300">R$ 4,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Fini+Dentadura">
                                    <span class="text-gray-300">Fini Dentadura</span>
                                    <span class="text-indigo-300">R$ 4,00</span>
                                </div>
                                <div class="flex justify-between items-center price-item border-b border-gray-700 pb-1" data-modal-target="productModal" data-image-url="https://via.placeholder.com/600x400?text=Adicional+Fini+Jujuba">
                                    <span class="text-gray-300">Fini Jujuba</span>
                                    <span class="text-indigo-300">R$ 3,00</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>
                
            </main>

            <footer class="text-center mt-16 pb-8 fade-in" style="animation-delay: 0.8s;">
                <p class="text-gray-400 text-sm">Dunitê Sorvetes e Açaí - Criando momentos doces desde sempre.</p>
                <p class="text-xs text-gray-500 mt-2">Paranaíba, MS - 2025</p>
            </footer>
        </div>
    </div>

    <div id="productModal" class="modal">
        <div class="modal-content">
            <span class="close-button" onclick="closeModal('productModal')">&times;</span>
            <h3 id="modalTitle" class="text-3xl font-lobster text-pink-400 mb-4 text-center"></h3>
            <img id="modalImage" src="" alt="Imagem do Produto" class="modal-image mx-auto my-4 shadow-lg">
            <p id="modalDescription" class="text-gray-300 text-center"></p>
        </div>
    </div>


    <script>
        function openModal(itemId, itemText, imageUrl) {
            const modal = document.getElementById(itemId);
            const modalTitle = document.getElementById('modalTitle');
            const modalImage = document.getElementById('modalImage');
            const modalDescription = document.getElementById('modalDescription');
            
            // Define o título, a imagem e a descrição
            modalTitle.textContent = itemText;
            modalImage.src = imageUrl;
            // A descrição é opcional, deixei vazia, mas você pode adicionar se quiser
            // modalDescription.textContent = 'Experimente a delícia de ' + itemText + '!'; 

            // Abre o modal
            modal.classList.add('open');
            document.body.style.overflow = 'hidden'; // Evita rolagem da página principal
        }

        function closeModal(itemId) {
            const modal = document.getElementById(itemId);
            modal.classList.remove('open');
            document.body.style.overflow = 'auto'; // Restaura a rolagem
        }

        // Adiciona eventos de clique a todos os elementos com a classe 'flavor-item-list' ou 'price-item'
        document.addEventListener('DOMContentLoaded', () => {
            const clickableItems = document.querySelectorAll('.flavor-item-list, .price-item');

            clickableItems.forEach(item => {
                item.addEventListener('click', () => {
                    const modalId = item.getAttribute('data-modal-target');
                    const imageUrl = item.getAttribute('data-image-url');
                    
                    // Tenta obter o texto do item. Para .flavor-item-list é o texto interno.
                    // Para .price-item, pegamos o texto do primeiro <span> (o nome do produto).
                    let itemText = '';
                    if (item.classList.contains('flavor-item-list')) {
                        itemText = item.textContent.trim();
                    } else if (item.classList.contains('price-item')) {
                        const titleSpan = item.querySelector('span:first-child');
                        if (titleSpan) {
                            itemText = titleSpan.textContent.trim();
                        }
                    }

                    if (modalId && imageUrl && itemText) {
                        openModal(modalId, itemText, imageUrl);
                    }
                });
            });

            // Fecha o modal ao clicar fora dele
            const modal = document.getElementById('productModal');
            modal.addEventListener('click', (event) => {
                if (event.target === modal) {
                    closeModal('productModal');
                }
            });

            // Fecha o modal ao pressionar a tecla ESC
            document.addEventListener('keydown', (event) => {
                if (event.key === 'Escape' && modal.classList.contains('open')) {
                    closeModal('productModal');
                }
            });
        });
    </script>
</body>
</html>
