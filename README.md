# cp500
Homenagem ao CP-500, um computador fabricado pela empresa brasileira Prológica durante a década de 1980

O CP-500 é um clone do TRS-80 americano, o que significa que todo o software desenvolvido para esta máquina também funciona na brasileira e vice-versa.

Há uma comunidade significativa de entusiastas do TRS-80 nos EUA e ao redor do mundo, e algumas dessas pessoas criaram emuladores quem permitem rodar aplicativos e jogos do TRS-80 em computadores modernos. Além disso, centenas de disquetes contendo software para essas máquinas foram disponibilizados na Internet de forma virtual, podendo ser usados diretamente nos emuladores. Alguns desses emuladores, como o TRS32 de Matthew Reed, são tão impressionantes, que imitam até mesmo o ruído dos drives quando acessam os disquetes, fazendo você se sentir como se estivesse diante de uma máquina de verdade.

http://www.cp500.com.br/
https://www.retrostic.com/
https://datassette.org/

Modelos
Quatro modelos de CP-500 foram produzidos no Brasil ao longo dos anos. Já nos EUA, o número de modelos de TRS-80 criados é bem maior. Há os TRS-80 Model I, II, III, 4, as versões portáteis 100/102, 200, 600, os CoCos 1, 2, 3, o MC-10 e também oito versões diferentes de Pocket Computers, para não falar nos clones internacionais dentre os quais o CP-500 é apenas um. Nem todos esses modelos são compatíveis entre si, portanto a tabela abaixo mostra os quatro modelos de CP-500 já criados e sua compatibilidade com os modelos de TRS-80.

Modelo	Ano	CPU	ROM	RAM	Texto	Gráficos	Compatibilidade
CP-500	1982	Z80 2MHz	16KB	48KB	64x16, 32x16	128x48	TRS-80 Model I/III
CP-500 M80	1985	Z80 2MHz	16KB or 2KB*	48KB or 64KB*	64x16, 32x16, 80x24	128x48	TRS-80 Model I/III/4
CP-500 M80C	1986	Z80 2MHz	16KB or 2KB*	48KB or 64KB*	64x16, 32x16, 80x24	128x48	TRS-80 Model I/III/4
CP-500 Turbo	1987	Z80 4MHz	16KB or 2KB*	48KB or 64KB*	64x16, 32x16, 80x24	128x48	TRS-80 Model I/III/4
*O CP-500 M80 e os modelos produzidos após esse eram equipados com uma placa que os permitia executar o sistema operacional CP/M . O CP/M deixa 64KB de memória RAM disponível para o sistema e reduz o endereçamento de ROM a apenas 2KB.

Emulação
Para emular um CP-500, você precisará de 3 coisas:

Um emulador de TRS-80 compatível com o seu sistema operacional
Um arquivo contendo uma imagem da ROM do CP-500 para usar no emulador
Um arquivo contendo uma imagem de disquete com um sistema operacional compatível com o CP-500
Opcionalmente, pode querer ter também:

Imagens adicionais de disquetes contendo jogos, aplicativos, utilitários etc.
Manuais de operação, livros de programação etc.
Nas seções seguintes são apresentadas as opções disponíveis em cada uma dessas categorias. Reserve um tempo para consultar também a seção de links, onde encontrará uma boa lista de referências para outras páginas sobre o TRS-80 ao redor do mundo.

Emuladores
A tabela abaixo lista os melhores emuladores que conheço. Se estiver usando Windows, não há alternativa melhor que o TRS32. Se estiver no Linux, vá de xtrs. Caso queira apenas ver um TRS-80 rodando online, veja a página do TRSEMU.

Emulador	Autor	SO	Descrição	Página
TRS32	Matthew Reed	Windows	Este programa emula o TRS-80 Model I, III, 4, e 4P. A emulação da CPU é extremamente precisa, suporta todas as intruções conhecidas e roda exatamente na mesma velocidade do TRS-80. Ele também é extremamente rápido, pois foi escrito em linguagem assembly, e pode exceder a velocidade real do TRS-80 em qualquer computador capaz de rodar Windows. A emulação do drive de disquete é incrivelmente precisa e funcionará muito bem até mesmo com discos de auto-boot ou protegidos, tal como o Super Utility.	www.trs-80emulators.com
xtrs	Tim Mann	Unix	O xtrs é um emulador do TRS-80 Model I/III/4/4P da Radio Shack para Unix e sistema X Window. Ele inclui minúsculas, relógio de tempo real, gráficos de alta resolução, porta serial, impressora paralela, mouse, gravador, saída de som e música (requer OSS), drives de disquete de 5"e 8" em densidade simples e dupla, e até mesmo discos rígidos.	tim-mann.org
SDLTRS	Mark Grebe	MacOS	O sdltrs é um emulador de TRS-80 Model I/III/4/4P da Radio Shack para Macintosh OSX, Windows e Linux. Ele foi portado a partir do excelente emulador xtrs para UNIX X-Windows de Tim Mann. Ao invés de usar o sistema X-Window para gráficos, ele usa a biblioteca portátil SDL.	sdltrs.sourceforge.net
TRSEMU	Peter Phillips	Web	Esta página web emula um TRS-80 Model III usando apenas Javascript. Este emulador é uma prova real da extrema velocidade dos computadores modernos e dos novos e impressionantes interpretadores Javascript. Esta combinação pode facilmente emular um TRS-80 rodando a 2MHz. Isto dá bem mais do que 100.000 instruções emuladas por segundo!	people.cs.ubc.ca/~pphillip
Outro	Outro	Outro	Se você precisa de um emulador para outros sistemas operacionais, eu sugiro que você pesquise o site trs-80.com. O Ira Goldklang mantém uma lista de todos os emuladores conhecidos juntamente com os links para baixá-los.	www.trs-80.com
Imagens da ROM
Graças ao Prof. Gustavo E. A. P. A. Batista, a comunidade do CP-500 teve acesso à primeira imagem de uma ROM de CP-500 extraída diretamente dos chips do computador com um leitor de EPROM. A ROM do CP-500 tem 16KB ao contrário dos 14KB encontrados no TRS-80. De acordo com uma análise feita por Matthew Reed, estes 2KB extras contém o monitor Z80 residente, que parece ser um recurso exclusivo do CP-500. Uma comparação também mostrou que apenas 90 bytes diferem entre as duas ROMs, a maioria deles devido a mensagens traduzidas do inglês para o português.

Como o monitor Z80 ocupa uma faixa de memória que conflita com os endereços de vídeo e teclado do TRS-80 original, este recurso não funciona no emulador TRS32. Por alguma razão desconhecida, para acessar a ROM do CP-500 (como quando você liga o computador sem disquetes nos drives) você deve primeiro iniciar o emulador com um disco do DOS500 e então reiniciá-lo novamente sem disquetes. Talvez haja algo no código do DOS que "habilite" a ROM.

Se você é o feliz proprietário de um CP-500 e quiser extrair uma imagem de sua ROM por conta própria, você pode usar o seguinte código escrito em Disk BASIC:

		10 OPEN "O",1,"CP500/ROM"
		20 FOR X=0 TO &H37FF:PRINT#1,CHR$(PEEK(X));:NEXT X
		30 CLOSE 1
		
Caso você não tenha uma máquina real para extrair uma imagem da ROM, pode baixá-la a partir daqui:

ROM
CP-500
ROM
CP-500 M80
ROM
TRS-80 Model I Level I
ROM
TRS-80 Model I Level II
ROM
TRS-80 Model III Level I
ROM
TRS-80 Model III Level II
ROM
TRS-80 Model 4
Sistemas Operacionais
Curiosamente, o CP-500 tinha à disposição pelo menos uma dúzia de sistemas operacionais de disco ("DOS") diferentes à escolha dos usuários. Os links abaixo permitem que você baixe algumas das principais opções nesta categoria:

Screenshot
DOS500
Screenshot
TRSDOS
Screenshot
NEWDOS/80
Screenshot
MultiDOS
Screenshot
RapidOS
Screenshot
DOSPLUS
Screenshot
LDOS
Jogos e Aplicativos
Apesar das limitações, sempre causa comoção observar a variedade de coisas úteis e interessantes que um computador equipado com apenas um processador de 8 bits e 2MHz era capaz de fazer. Dentre os muitos aplicativos e jogos disponíveis para o CP-500/TRS-80, você encontrará:

Editores de texto, planilhas de cálculo e sistemas de gerenciamento de bancos de dados
Jogos e programas para a criação de gráficos e som variados
Compiladores para muitas linguagens de programação
Utilitários de backup, softwares de comunicação etc.
Apesar de toda essa variedade, há um punhado de programas que, por alguma razão, realmente me encantavam. Eis alguns deles:

Screenshot
Crazy Painter
Screenshot
Chicken
Screenshot
Dancing Demon
Screenshot
Clone-III
Screenshot
Music Box
Screenshot
Visicalc
Screenshot
Frogger
Screenshot
Scarfman
Screenshot
Galaxy Invasion
Screenshot
Corndog
Manuais de Operação
Dois manuais eram fornecidos com o CP-500, um orientado a sua operação e programação em BASIC e outro ao uso do sistema operacional DOS500. Também existem manuais técnicos para a manutenção do hardware do TRS-80, mas não sei até que ponto o hardware do TRS-80 e o do CP-500 são semelhantes.

Cover
CP-500 Operação e Linguagem Basic
Cover
DOS-500 Sistema de Operação de Disco
Cover
TRS-80 Model III Technical Reference Manual
Cover
TRS-80 Model III/4 Diagnostics Manual
Cover
TRS-80 Model III/4 Service Manual
Alguns outros livros
Houve uma época em que surgiram inúmeras revistas e livros de programação nas livrarias do país e era empolgante buscar em cada publicação por conteúdo que fosse compatível com sua máquina. Como se pode observar em alguns dos livros abaixo, era comum publicarem listagens de programas para linhas variadas de computadores.

Cover
Microcomputador Jogos
Cover
Programas de Jogos de Espionagem
Cover
Programas de Jogos de Horror
Cover
Programas de Jogos de Terror
Cover
O Manual de CP/M
Cover
BASIC Faster and Better & Other Mysteries
Cover
TRSDOS 2.3 Decoded & Other Mysteries
Cover
Machine Language Disk I/O & Other Mysteries
Cover
Introduction to TRS-80 Level II BASIC
Cover
TRS-80 Assembly Language
Referências Externas
Esta é uma coleção de links que formei ao longo de minhas pesquisas sobre o CP-500. Se você decidir clicar em apenas um deles, que seja no primeiro, pois trata-se do Google Group que criei para trocar mensagens com outros interessados por esse assunto. Inscreva-se e mantenha contato com seus pares.

Screenshot
CP-500 Google Groups
Screenshot
Ira Goldklang's website
Screenshot
Matthew Reed's website
Screenshot
Tim Mann's website
Screenshot
Jeff Vavasour's website
Screenshot
George Phillips' website
Screenshot
Peter Phillips' website
Screenshot
Matt Hamilton's website
Screenshot
Yves Lempereur's website
Screenshot
Lajos Kintli's website
Screenshot
Wade Finch's website
Screenshot
Luis Tedeschi's website
Screenshot
Knut Roll-Lund's website
Screenshot
Michael Clay's website
Screenshot
Michael Haardt's website
Screenshot
Nick Andrew's website
Screenshot
Nickolas Marentes' website
Screenshot
Chris Swoboda' website
Screenshot
TRS-80 Dutch Usergroup
Screenshot
TRS-80.org
Screenshot
TRS-80.org.uk
Screenshot
Dick Smith System 80
Screenshot
LNW80 Main Page
Screenshot
Home of the Z80 CPU
Screenshot
Planet Emulation
Screenshot
Data Cassete
Screenshot
TRS80Stuff.net
Screenshot
Old-Computers.com
Screenshot
1000Bit
Screenshot
8bit-micro
Screenshot
MCI
Screenshot
Clube Old Bits
Screenshot
TRS-80 Gaming Guide
Screenshot
The Space Invaders Project
Screenshot
nemesis.lonestar.org
Screenshot
The Unnoficial CP/M Web site
Screenshot
CP/M Kermit
Screenshot
TRS-80 to PC Transfer Notes
Screenshot
The Semi-Virtual Diskette
Screenshot
OmniFlop
Screenshot
BBS: The Documentary
Screenshot
Radio Shack Catalogs
Screenshot
comp.sys.tandy Google Groups
Screenshot
TRS-80 Yahoo Groups
Screenshot
TRS-80 Club Yahoo Groups
Sobre Mim
Author
Meu nome é Miguel Dutra e comecei a programar em um CP-500 aos treze anos de idade, usando a linguagem BASIC. Segui carreira na área de tecnologia e sou apaixonado por programação até hoje.

Em 1990, quando eu tinha 16 anos, publiquei um artigo na revista brasileira Micro Sistemas, que era popular entre os usuários de computadores da época. Os vírus eram um tema em alta e eu também estava fascinado por eles, então mandei para a revista um programa escrito em BASIC cujo objetivo era detectar o vírus Sexta-Feira 13 em arquivos do PC.

Alguns meses mais tarde, naquele mesmo ano, enviei um artigo mais elaborado que acabou por se tornar a matéria de capa e também assunto do editorial daquela edição. Fiquei orgulhoso, claro! Era uma vacina tríplice desenvolvida em Turbo Pascal para encontrar e remover os vírus mais comuns da época: Sexta-feira 13, Stoned e Ping Pong. Depois desses, criei vários outros programas interessantes, relacionados à área de segurança. Olhando para trás, me arrependo de não tê-los publicado.

Veja abaixo meus artigos publicados na Micro Sistemas:

Page
Page
Page
Page
Page
Page
Page
Page
Na época em comecei a criar esta página, senti uma baita saudade do CP-500 e resolvi criar um programa para ler disquetes virtuais, que batizei de VDK-80.

Sobre o VDK-80
Floppy
Disquetes de CP-500 têm sido preservados através de processos de conversão que criam imagens do disco. Essas imagens são armazenadas em arquivos de PC especialmente formatados que podem ser usados diretamente nos emuladores.

Em fevereiro de 2009 eu comecei a trabalhar em um programa que permite algumas manipulações de imagens de disquetes de CP-500 em nível de arquivo. Seu desenvolvimento foi abandonado cerca de 4 anos depois. Apesar disso, ele avançou bastante e é capaz de operar com quase todos os sistemas operacionais e formatos de disco conhecidos do CP-500.

Por que isso é útil? Nos anos 1980 havia um grande número de sistemas operacionais disponíveis no mercado e seus sistemas de arquivo eram geralmente incompatíveis entre si. Em alguns casos, até mesmo entre versões sucessivas do mesmo sistema operacional. A transferência de arquivos entre tais discos não era tarefa fácil.

O que ele faz?
O VDK-80 é um programa de linha de comando do Windows que não requer instalação alguma. Eis a lista das "features":

Mostra o diretório do disco, nome do disco, conteúdo dos arquivos e setores do disco
Suporta ler, gravar, renomear ou excluir arquivos individuais ou grupos de arquivos
Suporta todos os sistemas operacionais conhecidos dos TRS-80 Model I/III/4, exceto CP/M
Suporta todos os formatos conhecidos de imagem de disquetes: JV1, JV3 e DMK
Tecnicalidades
Quando comecei este projeto decidi escrever o software em assembler usando orientação a objetos para resolver um problema relativamente incomum, como ler discos de computador antigos. Meu primeiro impulso foi trabalhar com disquetes reais do CP-500, mas depois Ira Goldklang me convenceu de que um software para manipular imagens de disco teria mais utilidade.

O código foi construído em módulos, ou classes no jargão de Orientação a Objetos. Há dois grupos principais de módulos que compartilham as mesmas características: um é a Interface de Sistema Operacional e a outra é a Interface de Disco Virtual. Esta última é responsável por "decodificar" o formato do arquivo e apresentar os dados como setores padrão para a camada superior. O primeiro interpreta a forma como cada sistema operacional armazena seus arquivos e depois remonta os setores como arquivos quando solicitado pela Interface do Usuário.

A imagem abaixo ilustra a relação entre os módulos especializados e as interfaces do programa:

Diagram
A interface de usuário é de linha de comando, mas o objetivo final era ter uma interface gráfica onde fosse possível trocar arquivos entre discos apenas arrastando e soltando-os de uma janela para outra.

Como usar
Nesta seção eu mostrarei como executar uma variedade de operações com o programa. Nos exemplos abaixo, eu assumo que você tenha colocado o arquivo executável do VDK-80 em um diretório do seu computador e que você tenha adicionado esse diretório à variável de ambiente PATH, permitindo que executemos o programa a partir de qualquer outro diretório.

Obtendo ajuda
O VDK-80 faz um bom trabalho identificando os formatos de disco e os sistemas operacionais automaticamente, mas há momentos em que um ajuste pode ser preciso. Se você precisar de ajuda para lembrar o que faz cada parâmetro, digite apenas:

C:\>v80
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

Syntax: V80 [switches]  [source_filespec] [target_filespec]

Commands:
	-l		List directory (default)
	-r		Read files
	-w		Write files
	-n		Rename files
	-k		Delete files
	-f		Dump file contents
	-d		Dump disk contents

Options:
	-s		Include system files
	-i		Include invisible files
	-x		Show extra information
	-p		Skip the disk parameters check
	-c		Skip the directory structure check
	-g		Skip the GAT auto-fix in TRSDOS system disks
	-b		Read as much as possible from bad files
	-ss		Force the disk as single-sided
	-ds		Force the disk as double-sided

Disk Interfaces:
	-dmk		Force the DMK disk interface
	-jv1		Force the JV1 disk interface
	-jv3		Force the JV3 disk interface

DOS Interfaces:
	-cpm		Force the CP/M system interface (INCOMPLETE)
	-dd		Force the DoubleDOS system interface
	-md		Force the MicroDOS/OS-80 III system interface
	-nd		Force the NewDOS/80 system interface
	-rd		Force the RapiDOS system interface
	-td1		Force the TRSDOS Model I system interface
	-td3		Force the TRSDOS Model III system interface
	-td4		Force the TRSDOS Model 4 system interface
			
Os comandos foram separados em grupos apenas por uma questão de organização, porque eles podem ser usados em qualquer ordem na linha de comando, seja antes, entre ou após os nomes de arquivo.

Listando o diretório do disco I
Se você digitar apenas o nome do programa e um nome de arquivo, o VDK-80 listará o diretório do disco excluindo arquivos de sistema e invisíveis. A listagem contém o nome e extensão do arquivo, o tamanho do arquivo em bytes, a data do arquivo formatada como yyyy/mm/dd e os atributos do arquivo como "SIMP", significando: Sistema, Invisível, Modificado, Proteção (0-7).

C:\>v80 td13.dmk
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

Listing directory contents:

Filename	    Size	Date		Attr
----------------------------------------------------
LPC/CMD     	     256	1981/05/00	---0
MEMTEST/CMD 	    2048	1981/05/00	---0
HERZ50/BLD  	      40	1981/05/00	---0

Total of 2344 bytes in 3 files listed.

The operation completed successfully.
			
Listando o diretório do disco II
Como mencionado anteriormente, você pode ajustar o comportamento do programa adicionando na linha de comando alguns dos argumentos acima listados. No exemplo a seguir, o VDK-80 é solicitado a mostrar o formato de disco e sistema operacional identificados (-x), e então listar somente os arquivos com extensão CMD (*/CMD), incluindo os arquivos de sistema (-s) e invisíveis (-i).

C:\>v80 td13.dmk */cmd -i -s -x
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

VDI: DMK (40:1:18,DD)
OSI: TD3 (TRSDOS,02/20/99,00)

Listing directory contents:

Filename	    Size	Date		Attr
----------------------------------------------------
BASIC/CMD   	    5120	1981/05/00	SI-6
CONVERT/CMD 	    2560	1981/05/00	SI-6
XFERSYS/CMD 	    1024	1981/05/00	SI-6
LPC/CMD     	     256	1981/05/00	---0
MEMTEST/CMD 	    2048	1981/05/00	---0

Total of 11008 bytes in 5 files listed.

The operation completed successfully.
			
VDI é a sigla de Virtual Disk Interface e DMK é um dos três formatos de disco suportados pelo programa (JV1, JV3, DMK). Os números entre parênteses estão formatados como TT:S:SS,DD, representando o número de trilhas, lados, setores por trilha e a densidade do disco (SD=Simples, DD=Dupla, MD=Mista).

OSI é a sigla de Operating System Interface e TD3 é o módulo que representa o TRSDOS Model III. Os dados entre parênteses são o nome do disco, data do disco e o byte de versão do DOS, conforme gravado na GAT.

Lendo arquivos do disco
Se você quiser copiar todos os arquivos do disco para a pasta atual, apenas digite:

C:\>v80 td13.dmk -r
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

Reading files from disk:

LPC/CMD      -> .\LPC.CMD   	     256 bytes	OK
MEMCHECK/CMD -> .\MEMCHECK.CMD	    2048 bytes	OK
HERZ50/BLD   -> .\HERZ50.BLD	      40 bytes	OK

Total of 2344 bytes read from 3 files.

The operation completed successfully.
			
Gravando arquivos no disco
Para copiar um arquivo da pasta atual para o disco, digite:

C:\>v80 td13.dmk -w readme.txt
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

Writing files to disk:

C:\README.TXT -> README/TXT     291 bytes OK

Total of 291 bytes written in 1 files.

The operation completed successfully.
			
Renomeando arquivos
Para renomear um arquivo, digite:

C:\>v80 td13.dmk -n memtest/cmd memcheck/cmd
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

Renaming files:

MEMTEST/CMD  -> MEMCHECK/CMD	OK

Total of 1 files renamed.

The operation completed successfully.
			
Excluindo arquivos
Suponha que você queira excluir todos os arquivos com a extensão BLD do disco. Neste caso, você digitaria:

C:\>v80 td13.dmk -k */bld
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

Deleting files:

HERZ50/BLD  	OK

Total of 1 files deleted.

The operation completed successfully.
			
Exibindo o conteúdo de um arquivo
O programa pode mostrar o conteúdo de um arquivo na forma de bytes hexa:

C:\>v80 td13.dmk -f lpc/cmd
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

Dumping file contents:

01 5A 00 70 2A 26 40 01 C2 03 AF ED 42 C2 2D 40 .Z.p*&@.Â.¯íBÂ-@
2A 11 44 22 36 70 22 46 70 22 4D 70 01 2A 00 B7 *.D"6p"Fp"Mp.*.·
ED 42 22 11 44 23 22 26 40 11 2E 70 EB ED B0 C3 íB".D#"&@..pëí°Ã
2D 40 79 E6 7F 4F CA 4B 04 3A 57 70 FE 0C 28 0F -@yæOÊK.:Wpþ..(.
FE 0D 28 0B FE 0A 28 07 79 32 57 70 C3 C3 03 79 þ.(.þ.(.y2WpÃÃ.y
32 57 70 FE 0D CA 2A 04 C3 C3 03 0D 02 02 00 70 2Wpþ.Ê*.ÃÃ.....p
21 E6 47 CD B9 43 21 54 48 CD B9 43 E1 5C CD 9C !æGÍ¹C!THÍ¹Cá\Í
43 5D CD 9C 43 CD CA 43 11 00 30 3E 07 32 08 44 C]ÍCÍÊC..0>.2.D
CD FE 43 E5 21 19 48 CD B9 43 21 6D 48 CD B9 43 ÍþCå!.HÍ¹C!mHÍ¹C
E1 3A E8 37 4F A8 B7 ED 42 B7 ED 42 5C CD 9C 43 á:è7O¨·íB·íB\ÍC
5D CD 9C 43 CD C7 43 21 49 49 CD B9 43 C9 D5 F5 ]ÍCÍÇC!IIÍ¹CÉÕõ
7B 07 07 07 07 CD AD 43 7B CD AD 43 F1 D1 C9 E6 {....Í­C{Í­CñÑÉæ
0F C6 90 27 CE 40 27 CD CC 43 C9 F5 7E FE 03 28 .Æ'Î@'ÍÌCÉõ~þ..(
06 CD CC 43 23 18 F5 F1 C9 CD CA 43 3E 0D D5 FD .ÍÌC#.õñÉÍÊC>.Õý
E5 F5 FE 09 28 17 CD 33 00 FD 21 11 4A FD 34 00 åõþ.(.Í3.ý!.Jý4.
FE 0D 20 04 FD 36 00 00 F1 FD E1 D1 C9 C5 3A 11 þ. .ý6..ñýá;ÑÉÅ:.

Total of 256 bytes dumped.

The operation completed successfully.
			
Exibindo todos os setores do disco
Ver a estrutura de um disco, setor a setor, pode ser muito útil para diagnosticar vários tipos de problemas. Algumas vezes você encontra problemas no setor de boot, no diretório ou em outras áreas importantes, que podem estar causando erros de acesso.

C:\>v80 td13.dmk -d
VDK-80, The TRS-80 Virtual Disk Kit v1.5
Written by Miguel Dutra (www.mdutra.com)
Icon by Marco Martin (www.notmart.org)

Dumping disk contents:

[00:0:01]
FE 11 3E D0 D3 F0 21 02 00 22 EA 43 AF 32 EC 43 þ.>ÐÓð!.."êC¯2ìC
CD 3E 43 FE 01 28 0C FE 02 20 E7 CD 3E 43 CD 35 Í>Cþ.(.þ. çÍ>CÍ5
43 E9 FF CD 3E 43 D6 02 47 CD 35 43 CD 3E 43 77 CéÿÍ>CÖ.GÍ5CÍ>Cw
23 10 F9 18 DB CD 3E 43 6F CD 3E 43 67 C9 C5 E5 #.ù.ÛÍ>CoÍ>CgÉÅå
3A EC 43 B7 20 2E 06 09 C5 CD 7F 43 C1 E6 1D 28 :ìC· ...ÅÍCÁæ..(
13 3E D0 D3 F0 10 F1 3E 17 CD 33 00 21 ED 43 CD .>ÐÓð.ñ>.Í3.!íCÍ
1B 02 18 FE 2A EA 43 2C 7D FE 13 38 03 2E 01 24 ...þ*êC,}þ.8...$
22 EA 43 AF 6F 26 4D 3C 32 EC 43 7E E1 C1 C9 CD "êC¯o&M<2ìC~áÁÉÍ
C5 43 01 F3 00 3E 81 D3 F4 57 21 B7 43 22 4A 40 ÅC.ó.>ÓôW!·C"J@.
3E C3 32 49 40 F3 3E C0 D3 E4 1E 02 21 00 4D 3E >Ã2I@ó>ÀÓä..!.M>
84 D3 F0 CD E0 43 DB F0 A3 28 FB ED A2 7A F6 40 ÓðÍàCÛð£(ûí¢zö@
D3 F4 ED A2 C3 B0 43 E1 AF D3 E4 3E 81 D3 F4 CD Óôí¢Ã°Cá¯Óä>ÓôÍ.
E6 43 DB F0 C9 3E 81 D3 F4 2A EA 43 7C D3 F3 3E æCÛðÉ>Óô*êC|Óó>.
1C D3 F0 CD E6 43 DB F0 CB 47 20 FA 7D D3 F2 C9 .ÓðÍæCÛðËG ú}ÓòÉ
F5 F1 F5 F1 F5 F1 F5 F1 00 C9 02 00 00 17 45 52 õñõñõñõñ.É....ER
52 4F 52 0D 01 26 40 73 18 10 02 40 00 00 13 28 ROR..&@s...@...(

(...)

[39:0:18]
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 E5 åååååååååååååååå
28 63 29 20 31 39 38 30 20 54 61 6E 64 79 20 20 (c) 1980 Tandy  

Total of 720 sectors dumped.

The operation completed successfully.
			
Download
Este software é fornecido gratuitamente, no estado ("as is"), sem garantias de qualquer tipo. Comentários e sugestões são bem-vindos.

TRS-80 Virtual Disk Kit v1.6
Floppy
VDK-80_v1.6.zip
72.670 bytes
Código-Fonte C++
Floppy
