# Novidades do Ondren

## 1.5.1 · Menor atividade em segundo plano — 15/09/2026
- A mesa passa a atualizar a interface com menor frequência em repouso e deixa de atualizar os pads e medidores quando está oculta na bandeja.
- O modo compacto atualiza seus próprios controles, sem redesenhar a mesa completa escondida. Textos e cores dos pads são reutilizados quando o estado não mudou.
- O estúdio de voz interrompe seu temporizador visual quando está oculto ou minimizado e reduz sua frequência fora de foco.
- Falhas de áudio, conclusão de prévias, limites de gravação e reconexão continuam sendo verificados em segundo plano. O processamento de áudio e os atalhos não dependem da frequência visual.
- O tempo da gravação agora exibe horas, minutos e segundos.
- As melhorias reduzem trabalho desnecessário da interface; não confirmam nem garantem resolver o carregamento de texturas de jogos.

## 1.5 · Editor, gravação em faixas e cenas completas — 14/09/2026
- Editor no menu de cada pad: corte por início/fim, remoção de silêncio inicial, entradas e saídas suaves e ajuste de pico para −1 dB. A forma de onda ajuda a visualizar o trecho.
- O editor aceita sons mono ou estéreo de até 30 minutos e salva uma nova cópia WAV de 48 kHz / 16 bits. Os arquivos originais e as cópias existentes são preservados. É possível ouvir a edição só no fone e usar a cópia no pad.
- O botão Gravar áudio oferece mistura final ou três faixas sincronizadas: mistura, voz tratada e soma dos pads enviados à chamada. As faixas individuais ficam antes do limiter final e preservam os volumes, mute/solo, tratamento e ducking aplicáveis.
- As gravações usam WAV estéreo de 48 kHz em ponto flutuante. Sons destinados só ao fone e prévias não entram nas faixas. Desligar a mesa, desconectar um dispositivo ou atingir 90 minutos finaliza a gravação.
- Arquivo → Exportar cena com áudios reúne os ajustes e os sons em um arquivo .ondren. Sons repetidos ocupam espaço uma única vez. O pacote comporta até 2 GB de áudio.
- Arquivo → Importar cena com áudios verifica o pacote e copia seus sons para uma pasta própria em Dados/CenasImportadas. A mesa fica desligada após carregar; confira os dispositivos antes de ligá-la. As cenas antigas continuam funcionando.
- Pacotes com caminhos indevidos, arquivos inesperados, áudios ausentes ou conteúdo inválido são rejeitados antes de trocar a cena atual.
- Corrigida a cópia dos buffers de áudio usados pelo Windows na gravação WAV, evitando erro de tipo de array.


## 1.4 · Destinos por pad, mesa compacta e reconexão — 14/09/2026
- Cada pad pode tocar na chamada, no fone ou nos dois, com volumes separados em Destino e volumes. O fader original continua controlando o volume geral do pad.
- Cenas e bancos guardam destinos e volumes. Configurações antigas mantêm o envio aos dois destinos. Sons enviados só ao fone não entram na gravação da mistura.
- Modo compacto com oito pads, controle de voz, volumes da chamada e do fone e silêncio geral. A troca de janela não reinicia o áudio.
- Ícone na bandeja do Windows para abrir a mesa, alternar para o modo compacto, silenciar o microfone e sair. Minimizar mantém o áudio ligado; fechar a janela principal ou escolher Sair encerra o app.
- O Ondren detecta dispositivos desconectados, preserva as escolhas e oferece Reconectar áudio quando os mesmos dispositivos voltam. A reconexão depende de um clique: a voz volta se estava habilitada, mas os pads ficam parados.
- Uma interrupção finaliza a gravação em andamento. A gravação não recomeça automaticamente após reconectar.
- Dispositivos salvos ausentes ficam identificados como indisponíveis, sem troca automática para outra saída.


## 1.3.1 · Correções dos pads, prévia e biblioteca — 14/09/2026
- Pads reiniciam no próximo clique após terminar o áudio, inclusive MP3 cuja duração estimada é maior que o som decodificado. Pausar continua retomando da mesma posição.
- Corrigido o erro que impedia a prévia de tocar no fone ao enviar o áudio para o Windows.
- A prévia termina depois que a saída conclui a reprodução, evitando cortar o final do som.
- Menu dos pads com fundo escuro e texto legível sem precisar passar o mouse. Prévia e remoção ficam indisponíveis em pads vazios.
- Espaçamento entre seleção de pad e carregamento, campos e botões dos bancos; folga junto à barra de rolagem da biblioteca.
- Falhas e conclusão da prévia também aparecem no painel da biblioteca. Campo de nome nos ajustes do canal acompanha o tema escuro.


## 1.3 · Biblioteca, atalhos e prévia — 13/09/2026
- Biblioteca de sons com busca por nome e categoria, favoritos e organização dos arquivos.
- Bancos para salvar e carregar os oito pads com seus nomes, volumes, equalização, panorama, mute, solo e loop. Ao carregar um banco, os pads anteriores param; a voz e a conexão são preservadas.
- Prévia independente no fone escolhido, com volume próprio. Ela não entra na mistura transmitida ou na gravação e não liga o microfone. Saídas virtuais reconhecidas e a saída da transmissão são bloqueadas para a prévia.
- Atalhos globais personalizáveis para pads, silêncio geral, mute do microfone, ativação de efeitos e personagens de voz. O editor avisa sobre combinações repetidas ou ocupadas.
- Histórico de atualizações disponível em Ajuda → Novidades da versão e neste arquivo.
- A biblioteca guarda referências aos arquivos originais. Renomear ou remover uma entrada não altera o áudio no disco. Mantenha os arquivos nas pastas originais.

## 1.2 · Menus e configurações — 13/09/2026
- Menus Arquivo, Áudio, Exibir e Ajuda; janela de Configurações com abas Áudio, Interface e Atalhos.
- Opções para ocultar painéis e manter o app sempre por cima, salvas separadamente das cenas.
- Dispositivos e buffer protegidos contra alterações enquanto a mesa está ligada.

## 1.1 · Supressão de ruído — 12/09/2026
- Limpeza local do microfone com RNNoise e intensidade ajustável, sem filtrar os pads.
- Comparação com o som original e persistência em cenas e perfis de voz.
- Aproximadamente 30 ms de atraso adicional quando a limpeza é ativada.

## 1.0.1 · Diagnóstico de voz e pads — 12/09/2026
- Teste da entrada virtual ampliado para verificar pad sozinho, voz com efeito e ambos juntos.
- Orientações sobre filtros do Discord e a diferença entre volume de transmissão e retorno.

## 1.0 · Identidade Ondren e conexão virtual — 12/09/2026
- Nome Ondren, novo símbolo e paleta de estúdio em grafite, verde e âmbar.
- Assistente para conectar a voz e os pads ao Discord usando VB-CABLE.
- Preservação das cenas anteriores, tratamento de voz, efeitos e gravação da mistura.

