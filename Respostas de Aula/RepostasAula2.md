# Repostas Aula 2

**data 15/03/2017**

**Thássio Gabriel Farias dos Santos 14/0163697**

**Q1. Quais as diferenças entre os barramentos de dados e de endereços?**
R: O Barramento de dados faz a transferencia entre os dados e o Barramento de endereço seleciona a origem ou o destino dos dados.

**Q2. Quais são as diferenças entre as memórias RAM e ROM?**
R: A memória ROM armazena dados e tem sua leitura lenta, já a memória RAM não consegue armazenar dados e tem sua leitura rápida.

**Q3. Considere o código abaixo, de 12 linhas:**

1.   #include <stdio.h>
    2.   int main(void)
    3.   {
    4.      int i;
    5.      printf("Insira um número inteiro: ");
    6.      scanf("%d", &i);
    7.      if(i%2)
    8.         printf("%d eh impar.\n");
    9.      else
   10.         printf("%d eh par.\n");
   11.      return 0;
   12.   }

**Para este código, responda:**
**(a) A variável 'i' é armazenada na memória RAM ou ROM? Por quê?**
  R:Na memória RAM pois essa é uma tarefa para uma memória volatil que nao armazena informação permanentemente.
  
**(b) O programa compilado a partir deste código é armazenado na memória RAM ou ROM? Por quê?**
  R:Na memória ROM pois essa é uma tarefa para uma memória não volátil que armazena a informação de forma permanente.
  
**Q4. Quais são as diferenças, vantagens e desvantagens das arquiteturas Harvard e Von Neumann?**
R:As arquiteturas são a Harvard Architecture e a Von Neumann Architecture. A arquitetura Von Neumann é mais simples e menos eficiente pois a arquitetura Harvard consegue ler e escrever informações ao mesmo tempo e a arquitetura Von Neumann ou lê ou escreve informações.

**Q5. Considere a variável inteira 'i', armazenando o valor 0x8051ABCD. Se 'i' é armazenada na memória a partir do endereço 0x0200, como ficam este byte e os seguintes, considerando que a memória é:**

    (a) Little-endian?          (b) Big-endian?
     0xCD ----- 0x200           0x80 ----- 0x200
     0xAB ----- 0x201           0x51 ----- 0x201
     0x51 ----- 0x202           0xAB ----- 0x202
     0x80 ----- 0x203           0xCD ----- 0x203

**Q6. Sabendo que o processador do MSP430 tem registradores de 16 bits, como ele soma duas variáveis de 32 bits?**
R:Usando 4 registradores. 
 - Primeiro deve ser inserido a primeira metade dos bits de um numero (16 bits) em um registrador e depois a outra metade em outro registrador;
 - Repete-se o mesmo processo para o outro número;
 - Soma-se as primeiras metades dos numeros e armazena o resultado em um dos registradores;
 - Junto com o carry, soma-se a outra metade dos numeros e o resultado final guarda-se em um registrador;
 - Usando os resultados de dois registradores em conjunto forma-se a soma dos dois numeros de 32 bits;
