Este projeto contém as coleções para realizar Requisições na API do projeto MyCollection.

Você pode executá-los de diversas maneiras, citarei duas abaixo.

---------------------------------------------------------

Requisitos: Para executar os testes, a aplicação back-end precisa estar rodando localmente

Para executar via linha de comando, é necessário ter o Node.JS instalado na sua máquina

Para executar via Postman, é necessário ter o Postman instalado na sua máquina

OBS: Acesse ao arquivo de variáveis de ambiente pelo bloco de notas ou notepad++ (MyCollectionVariables.postman_environment)
Procure a linha ("value": "https://localhost:44356/api"), altere o valor do endereço "44356" para o endereço local da aplicação na sua máquina e salve a alteração.

---------------------------------------------------------

1° Opção: Prompt de Comando (CMD)

Clone ou faça o download do repositório para sua máquina

Abra seu prompt de comando e instale o newman com o seguinte comando: npm install -g newman

Após isso, pelo prompt de comando, acesse a pasta onde estão os arquivos clonados/baixados

Execute o seguinte comando: newman run "MyCollection.postman_collection.json" -e "MyCollectionVariables.postman_environment.json"

Os testes de integração rodarão na sua máquina automaticamente.
 
 ----------------------------------------------------------

2° Opção: Postman

Clone ou faça o download do repositório para sua máquina

Desabilite a opçao (SSL certificate verification) nas configurações do Postman

Clique na opção do canto superior esquerdo (Import)

Selecione os Arquivos (MyCollection.postman_collection) e (MyCollectionVariables.postman_environment) que estão na pasta clonada

Após isso, clique no canto superior direito onde está escrito ("No Environment") e selecione a opção ("MyCollectionVariables")

Você pode executar os testes de maneira manual (Abra as pastas e realize as requisições) ou "automática" (Clique na opção de "play" no canto superior direito da pasta MyCollection > run > Run MyCollection).
