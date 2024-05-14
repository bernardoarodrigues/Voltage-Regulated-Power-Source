# Projeto Fonte Reguladora De Tensão

## Descrição
Fonte retificadora de tensão que transforma corrente alternada com tensão eficaz de 127V em corrente contínua com tensão ajustável entre 3V e 12V.

## Grupo
 - [Bernardo Alexandre Alves Rodrigues](mailto:bernardorodrigues@usp.br)
 - [Gabriel Phelippe Prado](mailto:gabriel.phelippe@usp.br)
 - [Gabriel Campanelli Iamato](mailto:gabriel.c.iamato@usp.br)
 - [Henrique Vieira Lima](mailto:vieira.henrique@usp.br)

## Informações
 - **Disciplina:** Eletrônica para Computação
 - **Professor:** Eduardo do Valle Simões
 - **Curso:** Bacharelado em Ciência da Computação
 - **Turma:** BCC-A / 2024 

## Vídeo do projeto
Adicionar link do vídeo no Youtube

## Lista de Componentes
| Quantidade | Componentes        | Valor (R$) |
|----|---------------|------------|
| 1x | Fusível              | [R$0,32](https://www.baudaeletronica.com.br/produto/fusivel-de-vidro-5x20-01a-250v.html) |
| 1x | Varistor             | [R$2,29](https://www.baudaeletronica.com.br/produto/varistor-s20k241-150vac.html) |
| 1x | Transformador 24V 1A | [R$53,46](https://www.baudaeletronica.com.br/produto/transformador-trafo-24v-1a-110220vac.html) |
| 5x | Diodo 1N4001         | [R$0,14 x 5 = R$0,70](https://www.baudaeletronica.com.br/produto/diodo-1n4001.html) |
| 1x | Capacitor 470µF 35V  | [R$0,77](https://www.baudaeletronica.com.br/produto/capacitor-eletrolitico-470uf-35v-105c.html) |
| 1x | Led Vermelho 5mm     | [R$0,24](https://www.baudaeletronica.com.br/produto/led-difuso-5mm-vermelho) |
| 1x | Resistor 2.2k        | [R$0,38](https://www.baudaeletronica.com.br/produto/resistor-2k2-5-2w.html) |
| 2x | Resistor 1k          | [R$0,05](https://www.baudaeletronica.com.br/produto/resistor-1k-5-14w.html) |
| 1x | Resistor 120         | [R$0,14](https://www.baudaeletronica.com.br/produto/resistor-120r-5-12w.html) |
| 1x | Resistor 82          | [R$0,14](https://www.baudaeletronica.com.br/produto/resistor-82r-5-12w.html) |
| 1x | Diodo Zener 13V 0.5W | [R$0,08](https://www.baudaeletronica.com.br/produto/diodo-zener-bzx55c-13v-05w.html) |
| 1x | Potenciômetro 5k     | [R$1,99](https://www.baudaeletronica.com.br/produto/potenciometro-linear-de-5k-5000.html) |
| 1x | Transistor NPN BC548 | [R$0,27](https://www.baudaeletronica.com.br/produto/transistor-npn-bc548.html) |
| 1x | Chave                | [R$1,35](https://www.baudaeletronica.com.br/produto/chave-hh-ss12f46-3-terminais.html) |
| **Total** |               | **R$62,18** |

## Funcionamento dos Componentes
 - **Fusível:** dispositivo de segurança que interrompe a passagem de corrente elétrica num circuito quando esta ultrapassa o limite permitido, de modo a proteger o circuito quando há picos de corrente.
 - **Varistor:** componente eletrônico que varia a sua resistência elétrica de acordo com a tensão aplicada aos seus terminais. Na medida em que a tensão aumenta, a resistência diminui. Os varistores são utilizados para proteger os aparelhos eletrônicos de picos de tensões.
 - **Transformador:** dispositivo que utiliza a indução eletromagnética para aumentar ou diminuir a tensão elétrica enquanto mantém a potência. Os transformadores funcionam exclusivamente com correntes alternadas. No circuito da fonte retificadora, o transformador reduz a tensão de 127V (proveniente da tomada) para 24V.
 - **Ponte de Diodo:** permite a conversão de corrente alternada (AC) em corrente contínua (DC). Ela é composta por quatro diodos retificadores conectados em uma configuração específica que permitem que a corrente flua em uma única direção.
 - **Capacitor:** é usado para armazenar carga elétrica. Na fonte reguladora, durante os ciclos da corrente alternada, libera corrente quando a tensão interna é maior do que a tensão advinda da ponte de diodo. Ele descarrega quando ocorre uma inversão de ciclo. O capacitor foi escolhido com um ripple desejado de 10%. Após os cálculos, foi-se obtido uma capacitância de 416,7uF. Assim, escolhemos o valor comercial de 470uF.
 - **Led:** diodo que converte eletricidade em luz. Nesse circuito, possui a função de indicar quando a fonte está ligada.
 - **Resistores:** componente eletrônico que regula a quantidade de eletricidade que flui por um circuito. O resistor diminui a intensidade da corrente elétrica e reduz o potencial elétrico ao longo de um fio.
 - **Diodo Zener:** componente que regula a tensão máxima. Ele irá conduzir corrente somente quando a tensão de entrada alcança a sua tensão nominal, que, no caso deste projeto, é de 12v. Caso a tensão seja menor do que 12V, não haverá corrente passando pelo diodo Zener; assim, ele não interferirá no circuito.  
 - **Potenciômetro:** componente eletrónico com resistência elétrica ajustável. Ele permitirá a escolha da tensão de saída, entre 3V e 12V.
 - **Transistor NPN:** dispositivo semicondutor que pode amplificar correntes elétricas, gerar oscilações elétricas e outros. Nesse projeto, possui a funcionalidade de permitir a passagem da corrente elétrica de forma ajustável.
 - **Chave:** uma chave elétrica pode estar num dos dois estados: fechado ou aberto. Quando a chave está fechada, a corrente elétrica passa pelo circuito; quando está aberta, a corrente elétrica não passa. Assim, podemos ativar ou desativar o funcionamento da fonte.

## Simulação do Circuito - Falstad
 - Acesse o simulador [Falstad](https://falstad.com/circuit/circuitjs.html)
 - No menu `File > Import from Text`, acesse o arquivo `./circuitoFonteFalstad.txt` do repositório
 - Adicionar Imagem

## Esquemático do Circuito - Eagle
 - Acesse o software [Eagle](https://www.autodesk.com/products/eagle/overview)
 - No menu `File > Open > Schematic...`, acesse o arquivo `./esquematicoEagle.sch` do repositório
 - Adicionar Imagem

## PCB do Circuito - Eagle
 - Acesse o software [Eagle](https://www.autodesk.com/products/eagle/overview)
 - No menu `File > Open > Schematic...`, acesse o arquivo `./pcbEagle.brd` do repositório
 - Adicionar Imagem

## Licença
Esse projeto está licenciado sobre a GNU General Public License V3.0, publicada pela Free Software Foundation.
