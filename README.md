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
    - [Componente 8 - Somador de 8 bits.](#componente-8---somador-de-8-bits)
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

### Componente 8 - Somador de 8 bits. 
> **Descrição:** Um somador de 8 bits é um circuito digital que realiza a soma de dois números binários de 8 bits (A e B) e, opcionalmente, considera um bit de transporte de entrada (Cin), gerando como resultado número binário de 8 bits representado pela saída SOMA e em caso de “estouro” de bits vai 1 para o Cout ocorrendo um overflow. A soma ocorre por conta dos 8 somadores de bit em paralelo e as suas entradas recebem os bits correspondentes a suas posições, como pode ser visto na imagem a abaixo.

![Somador de 8 bits](./Componente%208/Imagens/somador-8bits.png)

- [Arquivo do Circuito](./Componente%208/8-SOMADOR_8_BITS.circ)
- [Imagens](https://github.com/thetwelvedev/AOC_LeonardoCastroAlefeAlves_UFRR_LabCircuitos_2024/tree/main/Componente%208/Imagens)
---

## Referências
<!--1. Link para vídeos YouTube: 
2. Documentação: 
3. Site:-->
