#Repostas Aula 3

data 22/03/2017

Thássio Gabriel Farias dos Santos 14/0163697

1. Dada uma variável 'a' do tipo 'char' (um byte), escreva os trechos de código em C para:

	(a) Somente setar o bit menos significativo de 'a'.
  
  R: a = 0x0
  
	(b) Somente setar dois bits de 'a': o menos significativo e o segundo menos significativo.
  
  R:
  
	(c) Somente zerar o terceiro bit menos significativo de 'a'.
  
  R:      
     P1DIR = a && 0xFB;
  
	(d) Somente zerar o terceiro e o quarto bits menos significativo de 'a'.
  
  R: P1DIR = a && 0xF3
  
	(e) Somente inverter o bit mais significativo de 'a'.
  
  R: a^= 0x80;
  
	(f) Inverter o nibble mais significativo de 'a', e setar o nibble menos significativo de 'a'. 

2. Considerando a placa Launchpad do MSP430, escreva o código em C para piscar os dois LEDs ininterruptamente.

3. Considerando a placa Launchpad do MSP430, escreva o código em C para piscar duas vezes os dois LEDs sempre que o usuário pressionar o botão.

4. Considerando a placa Launchpad do MSP430, faça uma função em C que pisca os dois LEDs uma vez.

5. Reescreva o código da questão 2 usando a função da questão 4.

6. Reescreva o código da questão 3 usando a função da questão 4.
