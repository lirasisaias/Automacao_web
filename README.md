## Projeto de Automação Web

##### Esse projeto de Automação web se trada de uma pesquisa de preços no Google shop e Buscapé.

##### Onde o objetivo é se o valor dos produtos for abaixo de um preço limite definido por você, você vai descobrir os produtos mais baratos e atualizar isso em uma planilha.

##### E apos salvaremos a planilha com os dados e enviaremos essa planilha por e-mail.

### Comecei criando uma planilha "bucas.xlsx" onde possui as colunas:
 - Nome
  - Onde colocamos o nome do produto.
- Termos banidos
  - Os termos que não queremos que nossa automação web não puxe para nossa planilha de resultado.
- preços mínimos
  - O preço mínimo que o produto pode ter.
- Preços máximos
  - O preço máximo que o produto pode ter.

### Utilizei as seguintes bibliotecas para esse projeto
- Selenium
  - Biblioteca utilizada para a automação web.
- Smtplib
  - Biblioteca utilizada para o envio do e-mail.
- Mimetypes
  - Biblioteca auxiliar do Smtplib.
- Pathlib
  - Biblioteca utilizada para manipulação de pastas.
- Pandas
  - Biblioteca utilizada para manipulação de planilhas e dados.
- time
  - Biblioteca utilizada para manipular certas esperas para não ocorrer erros.

### Depois da instalação/importação das Bibliotecas começamos abrindo o nosso navegador com o selenium e exportamos a planilha "buscas.xlsx" com o pandas.

### Depois fiz 2 filtros:
- 1 - Ver se o produto possui uma das palavras que colocamos como "Termos banidos".
- 2 - ver se o produto possui o "Nome", "Preço mínimo", "Preço máximo".
### Agora só usar o selenium para buscar esses dados e salvarmos em 2 planilhas("tabela_google", "tabela_buscape"). Depois juntamos em um planilha que chamei de "tabela_ofertas".

### Agora só utilizar o Smtplib para enviar o e-mail.
