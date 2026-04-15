<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --roxo: #662c92;
            --lilas: #bf0087;
            --magenta: #ec0089;
            --amarelo: #fde100;
        }
        body {
            background-color: transparent;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
        }
        .bg-roxo { background-color: var(--roxo); }
        .text-roxo { color: var(--roxo); }
        .card-shadow {
            box-shadow: 0 4px 12px rgba(102, 44, 146, 0.15);
        }
        .timeline-line {
            position: absolute;
            left: 10px;
            top: 0;
            bottom: 0;
            width: 2px;
            background-color: var(--roxo);
            opacity: 0.3;
        }
        .timeline-dot {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            position: absolute;
            left: 6px;
            top: 6px;
            z-index: 10;
        }
    </style>
</head>
<body class="p-2">

    <div class="max-w-2xl mx-auto bg-white rounded-xl overflow-hidden card-shadow border border-gray-100">
        <!-- Header Compacto -->
        <div class="bg-roxo px-4 py-3 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <i class="fas fa-bullhorn text-amarelo text-xl"></i>
                <h1 class="text-white text-lg font-bold uppercase tracking-tight">Próximas Datas</h1>
            </div>
            <span class="text-[10px] text-white opacity-70 font-mono">📅 Calendário Acadêmico</span>
        </div>

        <!-- Conteúdo Compacto -->
        <div class="p-4 relative">
            <div class="timeline-line"></div>
            
            <div class="space-y-4">
                <!-- 21/04 -->
                <div class="relative pl-7">
                    <div class="timeline-dot bg-amarelo border-2 border-roxo"></div>
                    <div class="flex flex-col">
                        <span class="text-xs font-black text-roxo uppercase">21/04 • Feriado</span>
                        <p class="text-sm text-gray-700 font-bold">Tiradentes: Sem atividades acadêmicas.</p>
                    </div>
                </div>

                <!-- 28/04 -->
                <div class="relative pl-7">
                    <div class="timeline-dot bg-magenta border-2 border-white"></div>
                    <div class="flex flex-col">
                        <span class="text-xs font-black text-roxo uppercase">28/04 • Atenção</span>
                        <p class="text-sm text-gray-700">Sem aula presencial (Antecipada para 07 e 14/04).</p>
                    </div>
                </div>

                <!-- 28/04 a 05/05 -->
                <div class="relative pl-7">
                    <div class="timeline-dot bg-lilas border-2 border-white"></div>
                    <div class="flex flex-col">
                        <span class="text-xs font-black text-lilas uppercase">28/04 a 05/05 • Prazo Crítico</span>
                        <p class="text-sm font-bold text-roxo">Envio da Documentação (Versão 1)</p>
                        <div class="mt-1 grid grid-cols-2 gap-x-2 gap-y-1 bg-gray-50 p-2 rounded-lg border-l-2 border-amarelo">
                            <span class="text-[11px] text-gray-600"><i class="fas fa-users text-magenta mr-1"></i>Equipe</span>
                            <span class="text-[11px] text-gray-600"><i class="fas fa-code text-magenta mr-1"></i>Código</span>
                            <span class="text-[11px] text-gray-600"><i class="fas fa-user-tag text-magenta mr-1"></i>Stories</span>
                            <span class="text-[11px] text-gray-600"><i class="fas fa-video text-magenta mr-1"></i>Vídeo</span>
                        </div>
                    </div>
                </div>

                <!-- 05/05 -->
                <div class="relative pl-7">
                    <div class="timeline-dot bg-roxo border-2 border-amarelo"></div>
                    <div class="flex flex-col">
                        <span class="text-xs font-black text-magenta uppercase">05/05 • Avaliação</span>
                        <p class="text-sm font-bold text-roxo italic">Prova Presencial - Padrão ENADE</p>
                        <p class="text-[10px] text-gray-500 mt-1">Estudo disponível na sala online em 28/04.</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Footer Minimalista -->
        <div class="bg-gray-50 py-2 text-center border-t border-gray-100">
            <p class="text-[10px] text-roxo font-bold uppercase tracking-widest">Confira os detalhes no Modelo do Projeto</p>
        </div>
    </div>

</body>
</html>
