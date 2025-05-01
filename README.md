<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VoltRenew | Engenharia Elétrica Sustentável</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#10B981',
                        secondary: '#3B82F6',
                        dark: '#1F2937',
                        light: '#F9FAFB'
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.1) 0%, rgba(59, 130, 246, 0.1) 100%);
        }
        
        .stat-card {
            transition: all 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .project-card {
            transition: all 0.3s ease;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .nav-link {
            position: relative;
        }
        
        .nav-link:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 0;
            background-color: #10B981;
            transition: width 0.3s ease;
        }
        
        .nav-link:hover:after {
            width: 100%;
        }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Header/Navigation -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
            <div class="flex items-center">
                <div class="w-12 h-12 rounded-full bg-primary flex items-center justify-center mr-3">
                    <i class="fas fa-bolt text-white text-xl"></i>
                </div>
                <a href="#" class="text-2xl font-bold text-dark">Volt<span class="text-primary">Renew</span></a>
            </div>
            
            <nav class="hidden md:flex space-x-8">
                <a href="#home" class="nav-link text-gray-600 hover:text-dark font-medium">Início</a>
                <a href="#services" class="nav-link text-gray-600 hover:text-dark font-medium">Serviços</a>
                <a href="#projects" class="nav-link text-gray-600 hover:text-dark font-medium">Projetos</a>
                <a href="#about" class="nav-link text-gray-600 hover:text-dark font-medium">Sobre</a>
                <a href="#contact" class="nav-link text-gray-600 hover:text-dark font-medium">Contato</a>
            </nav>
            
            <button class="md:hidden text-gray-600" id="menu-toggle">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>
        
        <!-- Mobile Menu -->
        <div class="md:hidden hidden bg-white w-full py-4 px-4 shadow-md" id="mobile-menu">
            <div class="flex flex-col space-y-4">
                <a href="#home" class="text-gray-600 hover:text-dark font-medium">Início</a>
                <a href="#services" class="text-gray-600 hover:text-dark font-medium">Serviços</a>
                <a href="#projects" class="text-gray-600 hover:text-dark font-medium">Projetos</a>
                <a href="#about" class="text-gray-600 hover:text-dark font-medium">Sobre</a>
                <a href="#contact" class="text-gray-600 hover:text-dark font-medium">Contato</a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero-gradient py-10 md:py-20">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-12 md:mb-0">
                    <h1 class="text-4xl md:text-5xl font-bold text-dark mb-6">Energia limpa para um <span class="text-primary">futuro sustentável</span></h1>
                    <p class="text-lg text-gray-600 mb-8">Soluções inovadoras em engenharia elétrica focadas em energias renováveis e eficiência energética para residências e empresas.</p>
                    <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                        <a href="#contact" class="bg-primary hover:bg-green-700 text-white font-medium py-3 px-6 rounded-lg transition duration-300 text-center">Solicitar Orçamento</a>
                        <a href="#services" class="border border-primary text-primary hover:bg-primary hover:text-white font-medium py-3 px-6 rounded-lg transition duration-300 text-center">Nossos Serviços</a>
                    </div>
                </div>
                <div class="md:w-1/2 flex justify-center">
                    <img src="https://pbs.twimg.com/profile_images/1912560276953591808/ptjJ1_ee_400x400.jpg" alt="Coleção de acessórios para cabelo" class="rounded-xl shadow-xl w-full max-w-lg">
                </div>
              </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-6">
                <div class="stat-card bg-white p-6 rounded-xl shadow-md border border-gray-100">
                    <div class="text-primary text-4xl mb-3">
                        <i class="fas fa-solar-panel"></i>
                    </div>
                    <h3 class="text-3xl font-bold text-dark mb-2">25+</h3>
                    <p class="text-gray-600">Sistemas solares instalados</p>
                </div>
                <div class="stat-card bg-white p-6 rounded-xl shadow-md border border-gray-100">
                    <div class="text-primary text-4xl mb-3">
                        <i class="fas fa-leaf"></i>
                    </div>
                    <h3 class="text-3xl font-bold text-dark mb-2">15,000+</h3>
                    <p class="text-gray-600">Toneladas de CO2 reduzidas</p>
                </div>
                <div class="stat-card bg-white p-6 rounded-xl shadow-md border border-gray-100">
                    <div class="text-primary text-4xl mb-3">
                        <i class="fas fa-lightbulb"></i>
                    </div>
                    <h3 class="text-3xl font-bold text-dark mb-2">80%</h3>
                    <p class="text-gray-600">Economia média de energia</p>
                </div>
                <div class="stat-card bg-white p-6 rounded-xl shadow-md border border-gray-100">
                    <div class="text-primary text-4xl mb-3">
                        <i class="fas fa-user-tie"></i>
                    </div>
                    <h3 class="text-3xl font-bold text-dark mb-2">50+</h3>
                    <p class="text-gray-600">Clientes satisfeitos</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <span class="text-primary font-medium">NOSSOS SERVIÇOS</span>
                <h2 class="text-3xl md:text-4xl font-bold text-dark mt-2 mb-4">Soluções em Energia Sustentável</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Oferecemos serviços especializados para tornar sua propriedade mais eficiente e sustentável energeticamente.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300">
                    <div class="w-16 h-16 bg-primary bg-opacity-10 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-solar-panel text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-dark mb-3">Micro e Mini Geração Distribuída</h3>
                    <p class="text-gray-600 mb-4">Projeto e instalação de sistemas solares residenciais, comerciais e industriais, alem de consultoria regulatória para acesso ao sistema de distribuição</p>
                    <ul class="space-y-2">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check-circle text-primary mr-2"></i>
                            <span>Dimensionamento personalizado</span>
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check-circle text-primary mr-2"></i>
                            <span>Instalação profissional</span>
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check-circle text-primary mr-2"></i>
                            <span>Consultoria regulatória para acesso ao sistema de distribuição</span>
                        </li>
                    </ul>
                </div>
                
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300">
                    <div class="w-16 h-16 bg-primary bg-opacity-10 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-chart-line text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-dark mb-3">Eficiência Energética</h3>
                    <p class="text-gray-600 mb-4">Auditorias e projetos para reduzir o consumo de energia sem comprometer o conforto ou produtividade.</p>
                    <ul class="space-y-2">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check-circle text-primary mr-2"></i>
                            <span>Análise de consumo detalhada</span>
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check-circle text-primary mr-2"></i>
                            <span>Estudos para otimização de consumo</span>
                        </li>
                    </ul>
                </div>
                <div class="bg-white p-8 rounded-xl shadow-md hover:shadow-lg transition duration-300">
                    <div class="w-16 h-16 bg-primary bg-opacity-10 rounded-full flex items-center justify-center mb-6">
                        <i class="fas fa-chart-line text-primary text-2xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-dark mb-3">Mercado Livre</h3>
                    <p class="text-gray-600 mb-4">Estudo de demanda para acesso ao mercado livre de energia</p>
                    <ul class="space-y-2">
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check-circle text-primary mr-2"></i>
                            <span>Consultoria para contratação de demanda</span>
                        </li>
                        <li class="flex items-center text-gray-600">
                            <i class="fas fa-check-circle text-primary mr-2"></i>
                            <span>Autoprodução e produção independente de energia</span>
                        </li>
                    </ul>
                </div>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <span class="text-primary font-medium">NOSSOS PROJETOS</span>
                <h2 class="text-3xl md:text-4xl font-bold text-dark mt-2 mb-4">Trabalhos Realizados</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Alguns dos nossos projetos mais recentes em energias renováveis e eficiência energética.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="project-card bg-white rounded-xl overflow-hidden shadow-md">
                    <div class="h-48 overflow-hidden">
                        <img src="C:\Users\wosou\Desktop\site\PROJETO ELETRON\image2.jpg" alt="Projeto Solar Residencial" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <span class="text-primary text-sm font-medium">Microgeração Distribuída</span>
                        <h3 class="text-xl font-bold text-dark my-2">Sistema Solar 5kW</h3>
                        <p class="text-gray-600 mb-4">Instalação completa de sistema fotovoltaico para residência em Maricá/RJ.</p>
                        <div class="flex justify-between text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> Junho 2023</span>
                            <span><i class="fas fa-chart-line mr-1"></i> 80% redução na conta</span>
                        </div>
                    </div>
                </div>
                
                <div class="project-card bg-white rounded-xl overflow-hidden shadow-md">
                    <div class="h-48 overflow-hidden">
                        <img src="C:\Users\wosou\Desktop\site\PROJETO ELETRON\image.jpg" alt="Projeto Comercial" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <span class="text-primary text-sm font-medium">Eficiência Energética</span>
                        <h3 class="text-xl font-bold text-dark my-2">Supermercado Eco</h3>
                        <p class="text-gray-600 mb-4">Modernização completa do sistema elétrico com eficiência energética para rede de supermercados.</p>
                        <div class="flex justify-between text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> Março 2023</span>
                            <span><i class="fas fa-chart-line mr-1"></i> 35% economia anual</span>
                        </div>
                    </div>
                </div>

                <div class="project-card bg-white rounded-xl overflow-hidden shadow-md">
                    <div class="h-48 overflow-hidden">
                        <img src="C:\Users\wosou\Desktop\site\PROJETO ELETRON\image3.jpg" alt="Projeto Comercial" class="w-full h-full object-cover">
                    </div>
                    <div class="p-6">
                        <span class="text-primary text-sm font-medium">Minigeração distribuída</span>
                        <h3 class="text-xl font-bold text-dark my-2">Usina Fotovoltaica Macacu 3.000 kW</h3>
                        <p class="text-gray-600 mb-4">Consultoria para conexão de uma usina fotovoltaica, otimizando os processos e cuidando de toda a parte burocrática do processo de conexão.</p>
                        <div class="flex justify-between text-sm text-gray-500">
                            <span><i class="fas fa-calendar-alt mr-1"></i> Agosto 2024</span>
                            <span><i class="fas fa-chart-line mr-1"></i> Processo otimizado </span>
                        </div>
                    </div>
                </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="flex flex-col lg:flex-row items-center">
                <div class="lg:w-1/2 mb-12 lg:mb-0 lg:pr-12">
                    <img src="https://pbs.twimg.com/profile_banners/1912554110542315520/1744825350/1500x500" alt="Equipe VoltRenew" class="rounded-xl shadow-lg w-full">
                </div>
                <div class="lg:w-1/2">
                    <span class="text-primary font-medium">SOBRE NÓS</span>
                    <h2 class="text-3xl md:text-4xl font-bold text-dark mt-2 mb-6">Energizando o Futuro com Inovação</h2>
                    <p class="text-gray-600 mb-6">A VoltRenew nasceu em 2020 com a missão de transformar o setor energético através de soluções sustentáveis e tecnológicas. Somos uma equipe de engenheiros eletricistas, especialistas em energia renovável e eficiência energética comprometidos com um futuro mais limpo.</p>
                    
                    <div class="mb-8">
                        <div class="flex items-start mb-4">
                            <div class="bg-primary bg-opacity-10 p-2 rounded-full mr-4">
                                <i class="fas fa-bullseye text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark mb-1">Nossa Missão</h4>
                                <p class="text-gray-600">Democratizar o acesso a energias renováveis e promover a eficiência energética em todos os setores da sociedade.</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start mb-4">
                            <div class="bg-primary bg-opacity-10 p-2 rounded-full mr-4">
                                <i class="fas fa-eye text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark mb-1">Nossa Visão</h4>
                                <p class="text-gray-600">Ser referência nacional em soluções energéticas sustentáveis até 2030, contribuindo para a descarbonização da economia.</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-primary bg-opacity-10 p-2 rounded-full mr-4">
                                <i class="fas fa-heart text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark mb-1">Nossos Valores</h4>
                                <p class="text-gray-600">Sustentabilidade, inovação, excelência técnica, transparência e compromisso com o cliente.</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="flex flex-wrap gap-4">
                        <div class="flex items-center">
                            <div class="bg-primary bg-opacity-10 p-3 rounded-full mr-3">
                                <i class="fas fa-award text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark">5+</h4>
                                <p class="text-gray-600 text-sm">Anos de experiência</p>
                            </div>
                        </div>
                        
                        <div class="flex items-center">
                            <div class="bg-primary bg-opacity-10 p-3 rounded-full mr-3">
                                <i class="fas fa-users text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark">25+</h4>
                                <p class="text-gray-600 text-sm">Profissionais qualificados</p>
                            </div>
                        </div>
                        
                        <div class="flex items-center">
                            <div class="bg-primary bg-opacity-10 p-3 rounded-full mr-3">
                                <i class="fas fa-certificate text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark">15+</h4>
                                <p class="text-gray-600 text-sm">Certificações</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <span class="text-primary font-medium">DEPOIMENTOS</span>
                <h2 class="text-3xl md:text-4xl font-bold text-dark mt-2 mb-4">O que nossos clientes dizem</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">A satisfação dos nossos clientes é nossa maior recompensa.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-ccols-2 lg:grid-cols-3 gap-8">
                <div class="bg-gray-50 p-8 rounded-xl">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 mb-6">"A VoltRenew transformou completamente o consumo energético da minha casa. Em 6 meses o investimento no sistema solar já se pagou com a economia na conta de luz. Profissionais extremamente competentes."</p>
                    <div class="flex items-center">
                        <img src="https://th.bing.com/th/id/R.a879aa11cae13b23af42c1beda5bb86c?rik=OuG25EtFzIvHPg&pid=ImgRaw&r=0" alt="Dandarah Maria" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold text-dark">Dandarah Maria</h4>
                            <p class="text-gray-600 text-sm">Residência em Três Rios</p>
                        </div>
                    </div>
                </div>
                
                <div class="bg-gray-50 p-8 rounded-xl">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 mb-6">"Contratamos a VoltRenew para otimizar o consumo elétrico da nossa rede de lojas. O projeto superou todas as expectativas, com redução de 40% nos custos energéticos. Recomendo sem dúvidas!"</p>
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Carlos Mendes" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold text-dark">Carlos Mendes</h4>
                            <p class="text-gray-600 text-sm">Diretor Comercial</p>
                        </div>
                    </div>
                </div>
                
                <div class="bg-gray-50 p-8 rounded-xl">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 mb-6">"O sistema híbrido solar-eólico que instalaram na nossa propriedade rural resolveu nosso problema de falta de energia. Agora temos autonomia total e ainda vendemos o excedente. Equipe altamente profissional."</p>
                    <div class="flex items-center">
                        <img src="https://randomuser.me/api/portraits/women/65.jpg" alt="Ana Oliveira" class="w-12 h-12 rounded-full mr-4">
                        <div>
                            <h4 class="font-bold text-dark">Ana Oliveira</h4>
                            <p class="text-gray-600 text-sm">Produtora Rural</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="py-20 bg-primary text-white">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-bold mb-6">Pronto para economizar com energia limpa?</h2>
            <p class="text-lg mb-8 max-w-2xl mx-auto">Entre em contato conosco para uma avaliação gratuita do seu potencial de economia e geração de energia renovável.</p>
            <a href="#contact" class="bg-white text-primary hover:bg-gray-100 font-medium py-3 px-8 rounded-lg transition duration-300 inline-block">Agendar Consultoria</a>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <div class="flex flex-col lg:flex-row">
                <div class="lg:w-1/2 mb-12 lg:mb-0 lg:pr-12">
                    <span class="text-primary font-medium">CONTATO</span>
                    <h2 class="text-3xl md:text-4xl font-bold text-dark mt-2 mb-6">Entre em contato conosco</h2>
                    <p class="text-gray-600 mb-8">Estamos prontos para responder suas dúvidas e elaborar um projeto personalizado para suas necessidades energéticas.</p>
                    
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="bg-primary bg-opacity-10 p-3 rounded-full mr-4">
                                <i class="fas fa-map-marker-alt text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark mb-1">Endereço</h4>
                                <p class="text-gray-600">Praça da Bandeira - Rio de Janeiro/RJ</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-primary bg-opacity-10 p-3 rounded-full mr-4">
                                <i class="fas fa-phone-alt text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark mb-1">Telefone</h4>
                                <p class="text-gray-600">(21) 99999-4960</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-primary bg-opacity-10 p-3 rounded-full mr-4">
                                <i class="fas fa-envelope text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark mb-1">Email</h4>
                                <p class="text-gray-600">comercial@voltrenew.com.br</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-primary bg-opacity-10 p-3 rounded-full mr-4">
                                <i class="fas fa-clock text-primary"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-dark mb-1">Horário de Atendimento</h4>
                                <p class="text-gray-600">Segunda a Sexta: 8h às 18h</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="mt-8">
                        <h4 class="font-bold text-dark mb-4">Siga-nos nas redes sociais</h4>
                        <div class="flex space-x-4">
                            <a href="#" class="bg-gray-100 hover:bg-primary hover:text-white w-10 h-10 rounded-full flex items-center justify-center text-gray-600 transition duration-300">
                                <i class="fab fa-facebook-f"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-primary hover:text-white w-10 h-10 rounded-full flex items-center justify-center text-gray-600 transition duration-300">
                                <i class="fab fa-instagram"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-primary hover:text-white w-10 h-10 rounded-full flex items-center justify-center text-gray-600 transition duration-300">
                                <i class="fab fa-linkedin-in"></i>
                            </a>
                            <a href="#" class="bg-gray-100 hover:bg-primary hover:text-white w-10 h-10 rounded-full flex items-center justify-center text-gray-600 transition duration-300">
                                <i class="fab fa-youtube"></i>
                            </a>
                        </div>
                    </div>
                </div>
                
                <div class="lg:w-1/2">
                    <form class="bg-gray-50 p-8 rounded-xl shadow-sm">
                        <div class="mb-6">
                            <label for="name" class="block text-gray-700 font-medium mb-2">Nome Completo</label>
                            <input type="text" id="name" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent" placeholder="Seu nome">
                        </div>
                        
                        <div class="mb-6">
                            <label for="email" class="block text-gray-700 font-medium mb-2">Email</label>
                            <input type="email" id="email" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent" placeholder="seu@email.com">
                        </div>
                        
                        <div class="mb-6">
                            <label for="phone" class="block text-gray-700 font-medium mb-2">Telefone</label>
                            <input type="tel" id="phone" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent" placeholder="(00) 00000-0000">
                        </div>
                        
                        <div class="mb-6">
                            <label for="subject" class="block text-gray-700 font-medium mb-2">Assunto</label>
                            <select id="subject" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent">
                                <option value="">Selecione um assunto</option>
                                <option value="solar">Energia Solar</option>
                                <option value="efficiency">Eficiência Energética</option>
                                <option value="wind">Energia Eólica</option>
                                <option value="other">Outro</option>
                            </select>
                        </div>
                        
                        <div class="mb-6">
                            <label for="message" class="block text-gray-700 font-medium mb-2">Mensagem</label>
                            <textarea id="message" rows="5" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary focus:border-transparent" placeholder="Descreva sua necessidade..."></textarea>
                        </div>
                        
                        <button type="submit" class="w-full bg-primary hover:bg-green-700 text-white font-medium py-3 px-6 rounded-lg transition duration-300">Enviar Mensagem</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <div class="flex items-center mb-4">
                        <div class="w-10 h-10 rounded-full bg-primary flex items-center justify-center mr-3">
                            <i class="fas fa-bolt text-white"></i>
                        </div>
                        <a href="#" class="text-xl font-bold">Volt<span class="text-primary">Renew</span></a>
                    </div>
                    <p class="text-gray-400 mb-4">Soluções inovadoras em engenharia elétrica focadas em energias renováveis e eficiência energética.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <i class="fab fa-youtube"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h3 class="text-lg font-bold mb-4">Serviços</h3>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Energia Solar</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Eficiência Energética</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Armazenamento de Energia</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Carregamento VE</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Energia Eólica</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-lg font-bold mb-4">Links Úteis</h3>
                    <ul class="space-y-2">
                        <li><a href="#home" class="text-gray-400 hover:text-white transition duration-300">Início</a></li>
                        <li><a href="#services" class="text-gray-400 hover:text-white transition duration-300">Serviços</a></li>
                        <li><a href="#projects" class="text-gray-400 hover:text-white transition duration-300">Projetos</a></li>
                        <li><a href="#about" class="text-gray-400 hover:text-white transition duration-300">Sobre</a></li>
                        <li><a href="#contact" class="text-gray-400 hover:text-white transition duration-300">Contato</a></li>
                    </ul>
                </div>
                
                <div>
                    <h3 class="text-lg font-bold mb-4">Newsletter</h3>
                    <p class="text-gray-400 mb-4">Assine nossa newsletter para receber novidades e dicas sobre eficiência energética.</p>
                    <form class="flex">
                        <input type="email" placeholder="Seu email" class="px-4 py-2 rounded-l-lg focus:outline-none text-dark w-full">
                        <button type="submit" class="bg-primary hover:bg-green-700 px-4 py-2 rounded-r-lg">
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </form>
                </div>
            </div>
            
            <div class="border-t border-gray-800 mt-12 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 mb-4 md:mb-0">© 2023 VoltRenew. Todos os direitos reservados.</p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Termos de Serviço</a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Política de Privacidade</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        document.getElementById('menu-toggle').addEventListener('click', function() {
            const mobileMenu = document.getElementById('mobile-menu');
            if (mobileMenu.classList.contains('hidden')) {
                mobileMenu.classList.remove('hidden');
            } else {
                mobileMenu.classList.add('hidden');
            }
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    const mobileMenu = document.getElementById('mobile-menu');
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                }
            });
        });
    </script>
</body>
</html
