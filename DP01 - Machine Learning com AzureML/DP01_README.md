# Trabalhando com Machine Learning na Prática no Azure ML

## 1. Criando Workspace no Azure
Como passo inicial, é importante que seja criado um workspace no Azure, caso você não tenha um.

- O primeiro passo é clicar para "Criar um recurso".
- Após clicar, você será levado a página do Marketplace.
- Digite na barra de pesquisa "machine learning" e clique em "criar" após localizar o Azure Machine Learning.

<img src="DP01_imagens\01.png" /> <br>

Na próxima página terá algumas configurações a serem feitas.

- Colocar a Assinatura e Grupo de recursos (se não tiver um, apenas clicar em "criar novo")

<img src="DP01_imagens\02.png" /> <br>

Após esse passo, colocar as configurações como na imagem abaixo:

- A Região East US foi escolhida devido ao custo ser menor do que no Brasil.
- Os campos: "Conta de armazenamento", "Cofre de chaves" e "Application Insights" são preenchidos automaticamente após você preencher o primeiro campo "Nome".

<img src="DP01_imagens\03.png" /> <br>

A partir daí, poderá criar o workspace, será feita a validação primeiro como na imagem abaixo, e então poderá clicar em "criar":

<img src="DP01_imagens\04.png" /> <br>

Após ser concluída, poderá "ir para o recurso":

<img src="DP01_imagens\05.png" /> <br>

E iniciar o estúdio:

<img src="DP01_imagens\06.png" /> <br>

Já no estúdio, poderá ver os espaços de trabalho como na imagem abaixo e clicar neles para entrar:

<img src="DP01_imagens\07.png" /> <br>

E então podemos começar a próxima etapa na aba "ML Automatizado".

<img src="DP01_imagens\08.png" /> <br>
--

## 2. Criando ML Automatizado
Após clicar em "Novo trabalho de ML automatizado" como na imagem anterior, seguiremos o próximo passo de preencher os campos como está na imagem abaixo e clicar em "avançar":

<img src="DP01_imagens\09.png" /> <br>

Nesta tela selecionaremos o tipo de tarefa "Regressão" e criaremos um ativo de dados:

<img src="DP01_imagens\10.png" /> <br>

Preencher conforme imagem:

<img src="DP01_imagens\11.png" /> <br>

Agora será selecionado a opção "De arquivos da Web":

<img src="DP01_imagens\12.png" /> <br>

Nesta página, preencher com este link e clicar em "avançar":

<img src="DP01_imagens\13.png" /> <br>

Verificar se os campos estão iguais da imagem:

<img src="DP01_imagens\14.png" /> <br>

Seguir:

<img src="DP01_imagens\15.png" /> <br>

Clicar em "Criar":

<img src="DP01_imagens\16.png" /> <br>

Podemos ver que o ativo foi criado e agora podemos avançar:

<img src="DP01_imagens\17.png" /> <br>

Nesta tela, verificar a "Coluna de destino" e selecionar "rentals (Integer)" e clicar em "Exibir definições de configuração adicionais":

<img src="DP01_imagens\18.png" /> <br>

Selecionar e preencher conforme imagem:

<img src="DP01_imagens\19.png" /> <br>

Preencher conforme imagem:

<img src="DP01_imagens\20.png" /> <br>
<img src="DP01_imagens\21.png" /> <br>
<img src="DP01_imagens\22.png" /> <br>

Agora é só enviar o trabalho de treinamento:

<img src="DP01_imagens\23.png" /> <br>

Após envio do trabalho, irá passar pelo processo de configuração. Neste caso, espere até que termine o processamento.

<img src="DP01_imagens\24.png" /> <br>
<img src="DP01_imagens\25.png" /> <br>

Após processamento, na aba de "Jobs" poderá ver os resultados:

<img src="DP01_imagens\26.png" /> <br>
<img src="DP01_imagens\27.png" /> <br>
--

## 3. Teste do Modelo
Na página do modelo:
- Clique na aba "Pontos de extremidade" (também é possível acessar pelo menu lateral em "Pontos de extremidade"). 
- Clique no ponto correspondente ao modelo gerado. Em seguida, acesse a aba "Testar".

Para o teste, foi utilizado o JSON abaixo:

``` JASON
 {
   "Inputs": { 
     "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]    
   },   
   "GlobalParameters": 1.0
 }
```

A previsão gerada foi: 361.95

``` JASON
[
  361.95238671338427
]
```

