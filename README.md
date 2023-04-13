# Trabalho 1 - Fundamentos de Sistemas Computacionais

<h2>Integrantes</h2>

- Adrielle Dewes
- Arthur Turcati 
- Nicholas Luz

<br />

<h2 align="center">Desenvolvimento de um multiplicador serial com operandos de 8 bits</h2>

<div align="center">
  <img width="700" alt="image" src="https://user-images.githubusercontent.com/101582254/231624664-111670d1-dc84-4af3-8b7c-8ddfc636c4ad.png">
</div>

<br />

<h2> Operando o multiplicador:</h2>

<p align="justify"> 
Para começar a operar o multiplicador serial é necessário selecionar o valor do multiplicando representado pelos 8 pinos de A0 a A7 em sequência na parte superior do circuito, e o valor do multiplicador, representado pelos 8 flip-flops de B0 a B7 na parte inferior direita do circuito. A seleção destes valores é feita a partir da definição entre 1 e 0 nos respectivos pinos e flip-flops. Selecionados os valores, utiliza-se o clock situado a esquerda do circuito para dar início a operação. O clock deve ser clicado 16 vezes, que é o mesmo que realizar 8 pulsos de clock, para que a multiplicação seja feita e o resultado exibido no circuito. O resultado da operação pode ser visualizado na sequência de 16 flip-flops localizados na parte inferior do circuito, onde os 8 flip-flops da esquerda, ou registrador paralelo, correspondem a parte mais significativa (8 bits), e os 8 flip-flops da direita, ou registrador de deslocamento, correspondem a parte menos significativa (8 bits).
</p>
  
<h2>Exemplos de multiplicações</h2>
A seguir mostraremos exemplos de multiplicações com prints da tela do programa Logisim, onde o primeiro print se refere ao "antes", com o multiplicando e o multiplicador, e o segundo print é o resultado após os 8 pulsos de clock, com o número armazenado nos 16 flip-flops.

<br />
<br />

<p align="center"> Binário 00000101 x 00000110 = 0000000000011110</p>
<p align="center"> Decimal 5 x 6 = 30</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231625945-129ad5a3-00c5-4160-824b-49f7fe358b0c.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231626041-47b3dcdd-178b-4d62-9869-8e095560a9f9.png">
</div>

<br />

<p align="center"> Binário 10000001 x 00000010 = 0000000100000010</p>
<p align="center"> Decimal 129 x 2 = 258</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231626388-e0c712bb-949e-4ea1-9812-67177da5103d.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231626463-cae73429-7df3-4222-bf40-2f1f6efeacff.png">
</div>

<br />

<p align="center"> Binário 11111111 x 00000000 = 0000000000000000</p>
<p align="center"> Decimal 255 x 0 = 0</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231627380-6c67f139-0548-41a8-95d1-2608953ab22a.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231627430-8ab62f6e-b7c6-401d-806f-67f753fa63b6.png">
</div>

<br />

<p align="center"> Binário 11111111 x 11111111 = 1111111000000001</p>
<p align="center"> Decimal 255 x 255 = 65025</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231627670-d8cd8ffb-f9a0-4e96-8471-08c67bac2c91.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231627718-1d53a810-fdb2-4c63-8944-c56518993f6a.png">
</div>

<br />

<p align="center"> Binário 00000000 x 11111111 = 0000000000000000</p>
<p align="center"> Decimal 0 x 255 = 0</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231628107-3abd7184-0949-4605-bff8-1a4999181c1e.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231628155-ff38114d-502f-4c33-83ca-79abf14f3c6e.png">
</div>

<br />

<p align="center"> Binário 00001111 x 00000001 = 0000000000001111</p>
<p align="center"> Decimal 15 x 1 = 15</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231628600-c2a2b411-70de-4c13-bcd7-9f7e7473bbe8.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231628650-a17c4f54-6b45-4a54-861d-ede2b2fc441f.png">
</div>

<br />

<p align="center"> Binário 00000001 x 11110000 = 0000000011110000</p>
<p align="center"> Decimal 1 x 240 = 240</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231628905-70884cf4-d03d-416b-9b81-bcef99116052.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231628946-25afe165-2542-4e03-b688-4c70d02cda5b.png">
</div>

<br />

<p align="center"> Binário 00110011 x 11001100 = 0010100010100100</p>
<p align="center"> Decimal 51 x 204 = 10404</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231629226-05ed72a2-1986-49aa-a58a-8a72d80cc672.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231629258-f4b58721-91dd-4dcb-8342-5f53abb5b15a.png">
</div>

<br />

<p align="center"> Binário 01110111 x 00010001 = 0000011111100111</p>
<p align="center"> Decimal 119 x 17 = 2023</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231630212-beedc906-200d-4672-a970-3ae6a0873996.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231630242-e4713622-8810-4121-9ec2-1e42eac22b14.png">
</div>

<br />

<p align="center"> Binário 10101101 x 00001101 = 0000011101101111</p>
<p align="center"> Decimal 173 x 11 = 1903</p>
<div align="center" display="flex" >
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231630398-08676046-33b4-478c-bef5-514c58962d43.png">
  <img width="400" height="200" alt="image" src="https://user-images.githubusercontent.com/101582254/231630435-b5bbeb25-266e-4811-8c5c-91d2819eb7e0.png">
</div>
