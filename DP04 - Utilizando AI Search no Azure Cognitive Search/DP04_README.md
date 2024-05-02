# Azure Cognitive Search: Utilizando AI Search para  Indexação e Consulta de Dados

## 1. Criando Recursos
### Criar um recurso de Azure AI Search:
<img src="DP04_imagens\01.png" /> <br>

Preencher os campos e selecionar a Camada de preços indicada:

<img src="DP04_imagens\02.png" /> <br>
<img src="DP04_imagens\03.png" /> <br>

Após sucesso na validação, clicar em "Criar":

<img src="DP04_imagens\04.png" /> <br>
<img src="DP04_imagens\05.png" /> <br>

---
### Criar um recurso de Serviços Cognitivos:
<img src="DP04_imagens\06.png" /> <br>
<img src="DP04_imagens\07.png" /> <br>

---
### Criar uma Storage Account
Na barra de pesquisa da página inicial do Azure, pesquisar "storage" e selecionar o indicado na imagem:

<img src="DP04_imagens\08.png" /> <br>

Clicar em algum dos campos indicados para poder criar a conta de armazenamento:

<img src="DP04_imagens\09.png" /> <br>

Preencher os campos:

<img src="DP04_imagens\10.png" /> <br>

Após criar, ir na "Configuração":
- Clicar em "Habilitado" no campo de "Permitir acesso anônimo ao Blob".

<img src="DP04_imagens\11.png" /> <br>

Na aba de "Contêineres", criar um novo e preencher conforme imagem:

<img src="DP04_imagens\12.png" /> <br>
<img src="DP04_imagens\13.png" /> <br>

Após clicar no "coffee-reviews", carregar arquivos modelo que podem ser achados <a href = "inputs\reviews.zip" >AQUI.</a>

<img src="DP04_imagens\14.png" /> <br>
<img src="DP04_imagens\15.png" /> <br>

Após carregamento, ir na barra de pesquisa para encontrar a ferramenta "Pesquisa de IA"

<img src="DP04_imagens\16.png" /> <br>

Clicar em "Importar dados":

<img src="DP04_imagens\17.png" /> <br>

Preencher campos e escolher a conexão existente no campo de "Cadeia de conexão":

<img src="DP04_imagens\18.png" /> <br>
<img src="DP04_imagens\19.png" /> <br>
<img src="DP04_imagens\20.png" /> <br>
<img src="DP04_imagens\21.png" /> <br>
<img src="DP04_imagens\22.png" /> <br>

Preencher conforme imagem:

<img src="DP04_imagens\23.png" /> <br>
<img src="DP04_imagens\24.png" /> <br>
<img src="DP04_imagens\25.png" /> <br>
<img src="DP04_imagens\26.png" /> <br>
<img src="DP04_imagens\27.png" /> <br>
<img src="DP04_imagens\28.png" /> <br>

Execução bem sucedida:

<img src="DP04_imagens\29.png" /> <br>

Clicar em "Gerenciador de pesquisa":

<img src="DP04_imagens\30.png" /> <br>

No primeiro teste, foi escrito "chicago" para a ferramenta encontrar onde estaria localizada a palavra:

<img src="DP04_imagens\31.png" /> <br>

No segundo teste, foi escrito "negative" para que a ferramenta encontre frases com base no sentimento negativo:

<img src="DP04_imagens\32.png" /> <br>




