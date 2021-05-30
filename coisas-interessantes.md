# Lista de coisas interessantes em Hardware

# FPGAs

## Toolchain open-source para FPGAs

### [Project Trellis](https://github.com/YosysHQ/prjtrellis)

É um projeto que permite utilizar um toolchain open-source pra FPGAs ECP5 da Lattice. Essa linha (ECP5) tem até 85k LUTs e modelos com interfaces SERDES de até 5Gbps, permitindo sintetizar interfaces de alta velocidade como PCI-Express, USB 3.0, SATA, HDMI entre outras.

### [Yosys](https://github.com/YosysHQ/yosys)

Framework open-source para sintetizar Verilog.

### [Nextpnr](https://github.com/YosysHQ/nextpnr)

Framework open-source para "_place and routing_" em FPGAs. Usa a saída do Yosys para gerar o bitstream pra várias famílias de FPGA.

### Tutoriais usando Yosys, nextpnr

[Esse repositório](https://github.com/BrunoLevy/learn-fpga) tem tutoriais de como desenvolver um processador RISC-V simples e sintetizar ele numa FPGA usando um toolchain open-source.

- [https://github.com/BrunoLevy/learn-fpga](https://github.com/BrunoLevy/learn-fpga)

### [nMigen](https://m-labs.hk/gateware/nmigen/)
Ferramenta open-source que permite desenvolver para FPGAs utilizando Python.

- [Tutorial](https://github.com/RobertBaruch/nmigen-tutorial/blob/master/README.md)

## FPGAs Interessantes

### iCE40
São FPGAs de baixo custo (a partir de $1) e baixo consumo de energia que podem ser usadas com um toolchain open-source para desenvolvimento de hardware. Possuem até 8k LUTs.
Esse [tweet](https://twitter.com/BrunoLevy01/status/1398541544118964225?s=20) mostra um chip FPGA de $5 com um processador RISC-V sintetizado controlando um display de LCD pelo barramento SPI.

- [Link busca Digikey](https://www.digikey.com/en/products/filter/embedded-fpgas-field-programmable-gate-array/696?s=N4IgTCBcDaIJYGMCmAWADCAugGhAVilAAcoBGXIkyMPAX1wDZD4ATKEAWlLVJAoBd2fEPwCeRJOwCGAZwQhatIA)
- [Placa barata](https://www.olimex.com/Products/FPGA/iCE40/iCE40HX1K-EVB/open-source-hardware)

### ECP5

São FPGAs de alta performance (a partir de $6) que podem ser usadas com um toolchain open-source para desenvolvimento de hardware. Possuem até 85k LUTs e alguns modelos possuem interface LVDS e SERDES de até 5Gb, pspermitindo sintetizar interfaces de alta velocidade como PCI-Express, USB 3.0, SATA, HDMI entre outras.

- [Link busca Digikey](https://www.digikey.com/en/products/filter/embedded-fpgas-field-programmable-gate-array/696?s=N4IgTCBcDaIKYGMAOBWEBdANCAbFUAlgCZQgC0AjAAwUjZIAupdIDAnknKQIYDOCIAL6CgA)
- [Placa barata](https://fr.aliexpress.com/item/1005001686175194.html?spm=a2g0o.productlist.0.0.f77b6dd22zXn2l&algo_pvid=ab7f7951-1ffc-4486-a318-1c3f348619fb&algo_expid=ab7f7951-1ffc-4486-a318-1c3f348619fb-2&btsid=2100bb5116223679590967467ed725&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)


--------------------------

# Ferramentas interessantes

## Software
### [KiCad](https://www.kicad.org)
Ferramenta open-source para o desenvolvimento de placas de circuito (PCBs).

## Hardware

### [J-Link (clone)](https://fr.aliexpress.com/item/4000182310208.html?spm=a2g0o.productlist.0.0.413d7a512sErmz&algo_pvid=f1c5e32b-3439-4a62-8ae9-d837fff054ca&algo_expid=f1c5e32b-3439-4a62-8ae9-d837fff054ca-0&btsid=2100bb5116223679993457668ed725&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)
Permite programar microcontroladores através de várias interfaces como JTAG e SWD. Pode ser usado com as ferramentas da Segger ou com OpenOCD.

### [Analizador Lógico](https://fr.aliexpress.com/item/1005001451709172.html?spm=a2g0o.productlist.0.0.167a679dDUBRzr&algo_pvid=336e6ef4-045e-43f3-ab6f-e295854f85eb&algo_expid=336e6ef4-045e-43f3-ab6f-e295854f85eb-0&btsid=2100bb5116223680823958157ed725&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603_)
Esse analizador lógico de 8 canais e 24MHz pode ser usado como um "osciloscópio de baixo custo" para ensinar desenvolvimento de hardware. Pode ser usado com ferramentas open-source como o [Sigrok](https://sigrok.org) ou proprietárias como o [Saleae Logic](https://www.saleae.com/downloads/). Permite visualizar e decodificar sinais digitais como I2C, SPI, I2S, CAN, RS232, etc, e também visualizar sinais analógicos.


--------------------------
# Microcontroladores

## [Projeto Zephyr](https://www.zephyrproject.org)

É um projeto da Linux foundation para um sistema operacional em tempo real (RTOS) para microcontroladores que usa abstrações de hardware parecidas com a do Linux (Device Tree). Suporta quase todas as famílias de microcontroladores e tem uma implementação open-source do Bluetooth Low Energy.


--------------------------
# Linux embarcado DIY

Esse [artigo](https://jaycarlson.net/embedded-linux/) do _Jay Carlson_ mostra um guia de como ele construiu 10 projetos de SBCs (single-board computers) diferentes rodando Linux usando processadores diferentes, em PCBs que ele mesmo projetou.

- [Artigo](https://jaycarlson.net/embedded-linux/)

--------------------------

# Cursos
### [Desenvolvendo drivers de hardware para Linux](https://www.udemy.com/course/linux-device-driver-programming-using-beaglebone-black/)

### [Zero to ASIC](https://www.zerotoasiccourse.com)
Curso (USD550) que ensina desenvolvimento de ASICs para pessoas que já tem experiência com desenvolvimento de FPGAs.

--------------------------

# ASICs

## [Projeto OpenShuttle](https://www.efabless.com/open_shuttle_program)
Projeto patrocinado pela Google que fornece a fabricação de ASICs gratuitamente para projetos de hardware open-source.

## [Efabless](https://efabless.com)
Empresa que produz ASICs por USD10k.
