# Laboratório de circuitos - Codificação e Simulações

---

**Integrantes:** [Leonardo Castro](https://github.com/thetwelvedev) e [Álefe Alves](https://github.com/AlefeAlvesC)

**Descrição:** Essa a atividade tem como finalidade a construção de 17 componentes, onde sua construção total é feita com apenas o uso de pinos de entrada, pino des saída, portas OR, portas AND, portas NOT, Clock, Contante e Distribuidor. Onde tem como objeto o entendendimento de componentes da arquitetura de um computador. Cada componente está em uma pasta onde tem sua descrição, imagens, testes e arquivo gerado pelo **Logisim**.

---

## Índice
- [Laboratório de circuitos - Codificação e Simulações](#laboratório-de-circuitos---codificação-e-simulações)
  - [Índice](#índice)
  - [Relatório](#relatório)
  - [Componentes](#componentes)
    - [Componente 1 - Registrador Flip-Flop do tipo D e do tipo JK.](#componente-1---registrador-flip-flop-do-tipo-d-e-do-tipo-jk)
      - [Registrador Flip-flop tipo D:](#registrador-flip-flop-tipo-d)
      - [Registrador Flip-flop tipo D com PRESET e CLEAR:](#registrador-flip-flop-tipo-d-com-preset-e-clear)
      - [Registrador Flip-flop tipo JK:](#registrador-flip-flop-tipo-jk)
    - [Componente 2 - Multiplexador de 4 entradas.](#componente-2---multiplexador-de-4-entradas)
    - [Componente 3 - Porta lógica XOR.](#componente-3---porta-lógica-xor)
    - [Componente 4 - Somador de 8 bits mais 4.](#componente-4---somador-de-8-bits-mais-4)
    - [Componente 5 - Memória ROM de 8 bits.](#componente-5---memória-rom-de-8-bits)
    - [Componente 6 - Memória RAM de 8 bits.](#componente-6---memória-ram-de-8-bits)
    - [Componente 7 - Banco de Registradores de 8 bits.](#componente-7---banco-de-registradores-de-8-bits)
    - [Componente 8 - Somador de 8 bits.](#componente-8---somador-de-8-bits)
    - [Componente 9 - Detector de Sequência Binária 101.](#componente-9---detector-de-sequência-binária-101)
    - [Componente 10 - Unidade Lógica Aritmética de 8 Bits.](#componente-10---unidade-lógica-aritmética-de-8-bits)
    - [Componente 11 - Extensor de 4 bits para 8 bits.](#componente-11---extensor-de-4-bits-para-8-bits)
    - [Componente 15 - Extensor de 4 bits para 8 bits.](#componente-15---extensor-de-4-bits-para-8-bits)
      - [Circuito sem otimização:](#circuito-sem-otimização)
      - [Circuito otimizado com Mapa de Karnaugh:](#circuito-otimizado-com-mapa-de-karnaugh)
    - [Componente 16 - Decodificador de 7 Segmentos.](#componente-16---decodificador-de-7-segmentos)
    - [Componente 17 - Detector de Número Primo de 4 entradas com Mapa de Karnaugh.](#componente-17---detector-de-número-primo-de-4-entradas-com-mapa-de-karnaugh)
  - [Referências](#referências)

---
## Relatório
> Teve como finalidade a documentação do processo de construção dos 17 componentes, informando como foi realizada a construção, disponibilizando as imagens dos circuitos e seus componentes para melhor entendendimento, e a realização de teste para confirmar o funcionamento.

[Acesse o relatório]()<!--Colocar o endereço do relatório por pasta exeemplo: ./docs/relatório.pdf-->

---

## Componentes

### Componente 1 - Registrador Flip-Flop do tipo D e do tipo JK. 
> **Descrição:** Os Flip-Flops tipo D e JK são circuitos sequenciais usados para armazenar bits. O Flip-Flop D captura o valor presente na entrada D na borda ativa do clock, armazenando-o até a próxima borda, sendo ideal para registradores e sincronização. Já o Flip-Flop JK é mais versátil, eliminando estados inválidos do tipo SR; suas entradas J e K permitem configurar, resetar ou alternar o estado, sendo útil em contadores e divisores de frequência. Ambos são essenciais em circuitos digitais para armazenamento e controle de dados.
#### Registrador Flip-flop tipo D:
![Imagem Flip-Flop D](./Componente%201/Imagens/flip-flop-d.png)

#### Registrador Flip-flop tipo D com PRESET e CLEAR:
![Imagem Flip-Flop D](./Componente%201/Imagens/flip-flop-d-preset-clear.png)

#### Registrador Flip-flop tipo JK:
![Imagem Flip-Flop D](./Componente%201/Imagens/flip-flop-jk.png)

- [Arquivo do Circuito](./Componente%201/1-FLIP_FLOP_D_E_JK.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%201/Imagens)

### Componente 2 - Multiplexador de 4 entradas. 
> **Descrição:** O multiplexador é um dispositivo digital que seleciona uma entre várias linhas de entrada e a direciona para uma única linha de saída. Ele é controlado por sinais chamados de linhas de seleção. No caso do multiplexador de 4 entradas, ele seleciona uma entre as 4 entradas e tem 2 linhas de seleção, a quantidade de linhas de seleção é dada pela fórmula m= log2⁡(n), onde n é número de entradas.

![Multiplexador 4 entradas](./Componente%202/Imagens/mux-4-1.png)

- [Arquivo do Circuito](./Componente%202/2-MUX_4_X_1.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%202/Imagens)

### Componente 3 - Porta lógica XOR. 
> **Descrição:** A porta lógica XOR é uma porta digital que realiza a operação lógica de disjunção exclusiva. Ela tem a propriedade de retornar um valor 1 apenas quando suas entradas são diferentes, e 0 quando as entradas são iguais.

![Porta lógica XOR](./Componente%203/Imagens/xor.png)

- [Arquivo do Circuito](./Componente%203/3-XOR.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%203/Imagens)

### Componente 4 - Somador de 8 bits mais 4. 
> **Descrição:** Um somador de 8 bits é um circuito digital que realiza a soma de dois números binários de 8 bits (A e B) e, opcionalmente, considera um bit de transporte de entrada (Cin), gerando como resultado número binário de 8 bits representado pela saída S e em caso de “estouro” de bits vai 1 para o Cout ocorrendo um overflow. Mas nesse caso o valor de B é contante sendo sempre 4, assim os 8 somadores de bit em paralelo recebem 0 menos o terceiro pois ele fica na posição que resulta no valor 4, como pode ser visto na imagem a abaixo.

![Somador de 8 bits mais 4](./Componente%204/Imagens/somador-8-bits-mais-4.png)

- [Arquivo do Circuito](./Componente%204/4-SOMADOR_8_BITS_MAIS_4.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%204/Imagens)

### Componente 5 - Memória ROM de 8 bits. 
> **Descrição:** A memória apenas de leitura, mais conhecida como memória ROM, é uma memória normalmente projetada para fazer leitura de dados permanentes ou que raramente são alterados. Outras características desta que podem ser citadas são que esta é uma memória semicondutora e não-volátil. 

![Memória ROM de 8 bits](./)

- [Arquivo do Circuito](./)
- [Imagens]()

### Componente 6 - Memória RAM de 8 bits. 
> **Descrição:** Memória RAM é um termo empregado para se referir às memórias cujo tempo de acesso em qualquer endereço da memória é igual. Existem diversos tipos de memórias que podem receber esta alcunha, um exemplo é a própria memória ROM apresentada no componente anterior. Quando se trata de RAM em memórias semicondutoras, normalmente se refere às memórias do tipo RWM (Read-Write-Memory) que são aquelas em que é possível realizar as operações de leitura e escrita de dados. 

![Memória RAM de 8 bits](./)

- [Arquivo do Circuito](./)
- [Imagens]()

### Componente 7 - Banco de Registradores de 8 bits. 
> **Descrição:** O banco de registradores é um componente digital essencial no funcionamento de um processador, responsável por armazenar temporariamente as informações que estão sendo processadas em um dado momento. Ele consiste em um conjunto organizado de registradores, permitindo a execução de operações de leitura e de escrita sendo otimizado para acesso extremamente rápido às informações diretamente utilizadas pelo processador.

![Banco de Registradores de 8 bits](./)

- [Arquivo do Circuito](./)
- [Imagens]()

### Componente 8 - Somador de 8 bits. 
> **Descrição:** Um somador de 8 bits é um circuito digital que realiza a soma de dois números binários de 8 bits (A e B) e, opcionalmente, considera um bit de transporte de entrada (Cin), gerando como resultado número binário de 8 bits representado pela saída SOMA e em caso de “estouro” de bits vai 1 para o Cout ocorrendo um overflow. A soma ocorre por conta dos 8 somadores de bit em paralelo e as suas entradas recebem os bits correspondentes a suas posições, como pode ser visto na imagem a abaixo.

![Somador de 8 bits](./Componente%208/Imagens/somador-8bits.png)

- [Arquivo do Circuito](./Componente%208/8-SOMADOR_8_BITS.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%208/Imagens)

### Componente 9 - Detector de Sequência Binária 101. 
> **Descrição:** Um detector de sequência binária é um circuito capaz de detectar uma sequência de sinais de entrada em um conjunto de dados binários. Ou seja, é um circuito capaz de determinar se um conjunto de bits recebidos correspondem a uma sequência pré-estabelecida. Esse tipo de circuito é amplamente usando em sistemas de comunicação, processamento de dados e processamento de sinais digitais.

![Detector de Sequência Binária 101](./)

- [Arquivo do Circuito](./)
- [Imagens]()

### Componente 10 - Unidade Lógica Aritmética de 8 Bits. 
> **Descrição:** Uma Unidade Lógica e Aritmética (ULA) é um componente fundamental em sistemas digitais, responsável por realizar operações lógicas e aritméticas sobre números representados em circuitos lógicos. Geralmente, uma ULA recebe dois operandos como entradas e possui uma entrada de controle adicional, que especifica qual operação deve ser executada. Essas operações podem incluir somas, subtrações, multiplicações, divisões, além de operações lógicas como AND, OR, XOR, entre outras. A ULA desempenha um papel crucial no processamento de dados, sendo utilizada em processadores, controladores e outros dispositivos eletrônicos.

![Unidade Lógica Aritmética de 8 Bits](./)

- [Arquivo do Circuito](./)
- [Imagens]()

### Componente 11 - Extensor de 4 bits para 8 bits. 
> **Descrição:** Um extensor de sinal é um circuito digital utilizado para ampliar o número de bits de um valor binário, mantendo a precisão do número em termos de sinal (positivo ou negativo). O extensor de sinal de 4 bits para 8 bits é um circuito que transforma um número de 4 bits em um número de 8 bits, replicando o bit mais significativo (o bit de sinal) para os 4 bits mais significativos da saída, garantindo que o número continue com o mesmo valor.

![Extensor de 4 bits para 8 bits](./Componente%2011/Imagens/extensor-4-to-8.png)

- [Arquivo do Circuito](./Componente%2011/11-EXTENSOR_4_PARA_8_BITS.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%2011/Imagens)

### Componente 15 - Extensor de 4 bits para 8 bits. 
> **Descrição:** Um extensor de sinal é um circuito digital utilizado para ampliar o número de bits de um valor binário, mantendo a precisão do número em termos de sinal (positivo ou negativo). O extensor de sinal de 4 bits para 8 bits é um circuito que transforma um número de 4 bits em um número de 8 bits, replicando o bit mais significativo (o bit de sinal) para os 4 bits mais significativos da saída, garantindo que o número continue com o mesmo valor.

#### Circuito sem otimização:
![Circuito otimizado](./Componente%2015/Imagens/circuito-normal.png)
#### Circuito otimizado com Mapa de Karnaugh:
![Circuito otimizado](./Componente%2015/Imagens/circuito-otimizado.png)

- [Arquivo do Circuito](./Componente%2015/15-CIRCUITO_OTIMIZADO_COM_MAPA_DE_KARNAUGH.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%2015/Imagens)

### Componente 16 - Decodificador de 7 Segmentos. 
> **Descrição:** O decodificador de 7 segmentos de 4 entradas é um dispositivo eletrônico utilizado para converter um número binário em sinais que acionam um display de 7 segmentos, representando visualmente números em formato hexadecimal (0-9 e A-F). O display é composto por sete LEDs dispostos de forma a formar os números de 0 a 9 e as letras A à F, com cada segmento do display sendo controlado por um sinal individual, tendo suas posições representadas por letras (a, b, c, d, e, f e g).

![Decodificador de 7 Segmentos](./Componente%2016/Imagens/decodificador-de-7-segmentos-caso1.png)
- [Arquivo do Circuito](./Componente%2016/16-DECODIFICADOR_DE_7_SEGMENTOS_FORM_HEX.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%2016/Imagens)

### Componente 17 - Detector de Número Primo de 4 entradas com Mapa de Karnaugh. 
> **Descrição:** Um Detector de Número Primo de 4 entradas utilizando mapa de Karnaugh é um circuito lógico que identifica se um número de 4 bits (representado pelas entradas (A, B, C, D) é primo. Números primos são aqueles que possuem exatamente dois divisores 1 e ele mesmo. Onde nesse intervalo os números primos são 2, 3, 5, 7, 11 e 13. Quando há uma entrada em binário de um desses números primos a saída S = 1, caso contrário S = 0.

![Detector de Número Primo](./Componente%2017/Imagens/detector-de-numero-primo.png)
- [Arquivo do Circuito](./Componente%2017/17-DETECTOR_NUMERO_PRIMO_COM_MAPA_DE_KARNAUGH.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%2017/Imagens)

---

## Referências
<!--1. Link para vídeos YouTube: 
2. Documentação: 
3. Site:-->
