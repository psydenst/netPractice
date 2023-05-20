# netPractice

## Protocolo TCP/IP

  Um endereço IP é literalmente como um endereço. É um identificador de um computador no interior de uma rede, assim como um endereço identifica uma casa numa rua. Existem dois protocolos para regulamentar endereços IP: o IPv4 e IPv6. A atual versáo é a quarta, capaz de produzir mais de 4 bilhões de endereços. É constituída de 4 octetos - i.e., conjunto de 8 bits - os quais variam de 0 a 255. 
  Um endereço IP tem duas partes, Network Address e Host Addres, que podem ser lidas de acordo com a sub-máscara de rede que for ali empregada. Uma sub-máscara é justamente o delimitador entre a porção do endereço que identifica uma rede e a porção do endereço que identifica uma máquina - host - em particular. 
  Suponhamos uma sub-máscara de rede 255.255.240 e um endereço IP 192.168.1.100. Eis a descrição de ambos em binário:
 
      Sub-máscara: 11111111.11111111.11110000.00000000
      Endereço IP: 11000000.10101000.00000001.01100100
  
  Para realizar propriamente a descoberta de qual porção é host e qual é network, basta fazer uma operação de AND bit a bit. O resultado dessa operação AND será o endereço de rede: 11000000.10101000.00000000.00000000 em binário, ou 192.168.0.0, em decimal. Assim, podemos ver que, o host address será o resto dessa operação de AND. Nesse caso, 1.100.
  
