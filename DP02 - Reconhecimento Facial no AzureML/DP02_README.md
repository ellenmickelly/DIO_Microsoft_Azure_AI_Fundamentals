# Reconhecimento Facial e Transformação de Imagens em Dados no Azure ML

## 1. Criando um Recurso
Para iniciar, vamos em:

- "Criar um recurso"
- Categoria: IA + Machine Learning
- Serviços Cognitivos > Criar

<img src="DP02_imagens\01.png" /> <br>

Preencher os campos indicados e criar o recurso:

<img src="DP02_imagens\02.png" /> <br>
<img src="DP02_imagens\03.png" /> <br>
<img src="DP02_imagens\04.png" /> <br>

Após o recurso ser criado, ir para o Vision Studio.

---
## 2. Vision Studio
No Vision Studio, precisaremos selecionar o recurso a ser usado. <br>
Clique em: "View all resources".

<img src="DP02_imagens\05.png" /> <br>

Selecione o recurso criado anteriormente.

<img src="DP02_imagens\06.png" /> <br>


### Detect Faces in an Image
O primeiro teste será para detectar rostos nas imagens:

- Na página inicial do Vision Studio, clique na aba "Face"
- Clique em "Detect faces in an image"

<img src="DP02_imagens\07.png" /> <br>

Clicar no checkbox indicado:

<img src="DP02_imagens\08.png" /> <br>

Neste teste, foi colocada a imagem do The Flash para que reconheça o rosto e este foi o resultado:

<img src="output\01.png" /> <br>

Para poder ver o resultado em JSON, clique <a href = "output\01.json" >AQUI.</a> 


### Extract Text from Images
No nosso próximo teste, usaremos o "Extract text from images".

<img src="DP02_imagens\09.png" /> <br>

Mesmo procedimento anterior para assinalar a checkbox:

<img src="DP02_imagens\10.png" /> <br>

Neste teste, foi colocada uma imagem aleatória de passaporte e este foi o resultado:

<img src="output\02.png" /> <br>

Para poder ver o resultado em JSON, clique <a href = "output\02.json" >AQUI.</a> 


### Add Captions to Images
Neste último teste, será utilizado o "Add captions to images.

<img src="DP02_imagens\11.png" /> <br>

Assinale a checkbox:

<img src="DP02_imagens\12.png" /> <br>

Foi colocada a imagem do Thanos e este foi o resultado:

<img src="output\03.png" /> <br>

Para poder ver o resultado em JSON, clique <a href = "output\03.json" >AQUI.</a> 



