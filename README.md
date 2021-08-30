# Regras udev


Pacote .tgz é destinado ao Slackware.


Mais hardware pode ser adicionados a regra, ser o kernel tiver suporte a eles. 

No Issue os usuários contribuem, reportam os problemas/bugs encontrados. Ficando assim mais fácil a correção do problema e a obtenção das informações para simulação dos problemas.

----------------------------------------------------------------------------

Padrão para criar novas regras:

1- Fornecer a saída do comando lsusb.

# lsusb
Bus 008 Device 005: ID 093a:2620 Pixart Imaging, Inc.

2- Informa qual o programa que abre esse dispositivo

guvcview

----------------------------------------------------------------------------


Seria algo de Plug and Play para Linux

Plug and Play, às vezes, PnP abreviado, é uma frase cativante usada para descrever dispositivos que funcionam com um sistema de computador assim que são conectados. O usuário não precisa instalar manualmente Drivers para o dispositivo ou até mesmo informar ao computador que um novo dispositivo foi adicionado. Em vez disso, o computador reconhece automaticamente o dispositivo, carrega novos drivers para o hardware, se necessário, e começa a trabalhar com o dispositivo recém-conectado.

Por exemplo, se você conectar um mouse Plug-and-Play ao USB porta do computador, ele começará a funcionar alguns segundos depois de ser conectado. Um dispositivo não plug-and-play exigiria que você seguisse várias etapas de instalação de drivers e configuração do dispositivo antes de funcionar.

Embora o Plug and Play geralmente se refira a dispositivos periféricos de computador, como teclados e mouses, também pode ser usado para descrever o hardware interno. Por exemplo, um placa de vídeo or disco rígido pode ser um dispositivo Plug and Play, o que significa que o computador o reconhecerá assim que for instalado. A única diferença é que os componentes internos geralmente exigem que o computador seja desligado quando estão instalados, enquanto dispositivos externos geralmente podem ser instalados enquanto o computador está em execução.




Regras para dispositivos USBs


* Plugou aquele pendrive cheio de virus na porta USB do computador
passa o antivirus Clamav.

Bus 002 Device 006: ID 1221:3234 Unknown manufacturer Disk (Thumb drive)



* Abre o Wicd para:

- Adaptador de rede sem fio MT7601U da Ralink

  Bus 001 Device 008: ID 148f:7601 Ralink Technology, Corp. MT7601U Wireless Adapter


- Adaptador de rede sem fio 'Intelbras WBN 900' usando o chip da Ralink

  Bus 002 Device 006: ID 148f:3070 Ralink Technology, Corp. RT2870/RT3070 Wireless Adapter



* Abre o Guvcview para:

- Webcam USB da C3Tech

  Bus 008 Device 005: ID 093a:2620 Pixart Imaging, Inc.

...

Leia o arquivo: /usr/doc/regras-udev-?/leia-me.txt
