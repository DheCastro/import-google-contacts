# Import Google Contacts
Utilitário para importação dos contatos do Google Contatos para o Google Sheets

A ferramenta Google Contatos (onde se encontram informações de e-mail, telefone, cargo... dos contatos de quem utiliza os serviços do Google),
dispõe de funcionalidade de importação dos dados, mas a mesma só pode ser "baixada" no formato <b>CSV</b> ou <b>vCard</b>, dificultando para quem apenas necessita
de uma listagem simples em um arquivo <b>XLS</b> ou <b>XLSX</b>, por exemplo. Segue print da tela de importação:

<img src="https://uploaddeimagens.com.br/images/003/023/118/full/contatos.PNG" />

Além da limitação de formato já citada, a importação também sempre traz todos os dados, mesmo os que estão em branco... limitando filtro de dados
e por dados. Não da pra filtrar por data de adição do contato, por contatos de determinado domínio etc.

Assim sendo, criei esse pequeno utilitário em <b>Google App Script (GAS)</b> (lingaugem baseada em JavaScript para trabalhar especificamente com os serviços do Google,
fazendo as personalizações e automatizações que o usuário desejar) para importar os contatos do <b>Contacts</b> para o <b>Sheets</b>. Hoje, a rotina recupera apenas nome e e-mail do contato e apenas dos que estão preenchidos, fazendo uma espécie de sanitização em dados inconsistentes. Porém, pretendo evoluir o código colocando parametrização e permitindo
que o usuário quais dados ele quer importar.
