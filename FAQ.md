# Perguntas frequentes

## Preciso criar uma conta?
Não para usar o aplicativo ou baixar a Release pública. Uma conta no GitHub é necessária para abrir relatos de problemas.

## Em quais computadores funciona?
O pacote é para Windows 64 bits (x64). Não há versões nativas para macOS, Linux ou Windows ARM. O .NET acompanha o app. Ainda não foi definida uma configuração mínima de hardware baseada em testes amplos.

## Por que não aparece um microfone chamado Ondren no Discord?
O Ondren envia a mistura a um dispositivo virtual instalado separadamente. Com o VB-CABLE padrão, escolha CABLE Input na saída do Ondren e CABLE Output na entrada do Discord.

## A voz chega, mas os pads são cortados.
Confira destino, volume, mute/solo e master. Depois revise a supressão de ruído e os filtros automáticos do Discord: eles podem interpretar música e efeitos como ruído. A supressão do Ondren trata apenas o microfone.

## Onde ficam os dados?
Configurações e biblioteca ficam em Dados, dentro da pasta do aplicativo. Áudios normalmente continuam nas pastas originais. Cenas completas importadas guardam cópias em Dados/CenasImportadas. Preserve Dados e seus áudios ao atualizar.

## A atualização é automática?
Ainda não. Feche o Ondren e execute o novo instalador na mesma pasta que contém seu Ondren.exe. Isso também funciona para atualizar uma cópia portátil. Se preferir o ZIP, extraia e copie os arquivos para a pasta atual, preservando Dados e seus áudios. Instalar em outra pasta não transfere configurações automaticamente. Leia as notas antes de atualizar.

## O editor modifica o original?
Não. Ele salva uma nova cópia WAV estéreo, 48 kHz / 16 bits. Aceita sons mono ou estéreo de até 30 minutos. A normalização ajusta o pico a −1 dB; não é normalização de volume percebido/LUFS.

## Como funcionam as faixas separadas?
São três WAVs sincronizados: mistura final, voz tratada e soma dos pads enviados à chamada. Voz e pads ficam antes do limiter final. Sons só no fone e prévias não entram. A gravação termina ao desligar ou desconectar a mesa, ou aos 90 minutos.

## O Ondren resolve travamentos ou texturas de jogos?
Não há essa garantia. A versão 1.5.1 reduz o trabalho visual em repouso e suspende a atualização dos controles na bandeja. O efeito em um jogo precisa ser medido no próprio computador.

## O Windows mostra um aviso.
O executável ainda não possui assinatura digital de editor. Baixe pela Release deste repositório e compare o SHA-256 com SHA256SUMS.txt da mesma versão. Não desative o antivírus. Se houver detecção de ameaça, interrompa a instalação e informe o nome da detecção, sem dados pessoais.

## Quais são os limites desta beta?
- WAV, MP3 e AAC/M4A foram testados. Outros formatos dependem dos decodificadores do Windows.
- As saídas usam 48 kHz estéreo. Buffers de 40/80/120 ms são configurações, não a latência total medida.
- A reconexão depende de um clique; pads e gravação não retomam automaticamente.
- O dispositivo virtual é instalado separadamente.
- Instalador e ZIP portátil disponíveis; sem assinatura digital ou atualização automática nesta etapa.

## O desinstalador apaga meus áudios e configurações?
Não. Ele remove os arquivos instalados do aplicativo e mantém os dados pessoais na pasta escolhida. Por isso, a pasta pode continuar existindo após desinstalar.

## Como entro em contato?
Abra **Ajuda → Contato e comunidade** para escrever ou copiar o e-mail, enviar sugestões, relatar problemas e acessar os canais oficiais. O endereço é ondren.audio@gmail.com.
