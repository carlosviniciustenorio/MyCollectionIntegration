Este projeto contém as coleções dos Testes de Integração da WebAPI MyCollection.

Você pode executá-los de diversas maneiras, citarei duas abaixo.

---------------------------------------------------------

Requisitos: Para executar os testes a aplicação precisa estar rodando localmente. Para executar via linha de comando, é necessário ter o Node.JS instalado na sua máquina. Para executar via Postman, é necessário ter o Postman em sua máquina.

OBS: Acesse ao arquivo de variáveis de ambiente pelo bloco de notas ou notepad++ (MyCollectionVariables.postman_environment)
Procure a linha ("value": "https://localhost:44356/api") e altere o valor do endereço "44356" para o endereço local da aplicação na sua máquina

---------------------------------------------------------

1° Opção- Prompt de Comando (CMD)
Clone ou faça o download do repositório para sua máquina

Abra seu prompt de comando e instale o newman com o seguinte comando: npm install -g newman

Após isso, pelo prompt de comando, acesse a pasta onde estão os arquivos clonados/baixados

Execute o seguinte comando: newman run "MyCollection.postman_collection.json" -e "MyCollectionVariables.postman_environment.json"

Os testes de integração rodarão na sua máquina automaticamente.
 
 ----------------------------------------------------------

2° Opção- Postman
Clone ou faça o download do repositório para sua máquina

No Postman, clique na opção do canto superior esquerdo ao lado de New OPÇÃO (Import)

Selecione os Arquivos (MyCollection.postman_collection) e (MyCollectionVariables.postman_environment) que estão na pasta clonada

Após isso, clique no canto superior direito onde está escrito ("No Environment") e selecione a opçao ("MyCollectionVariables")

Você pode executar os testes de maneira manual (Abra as pastas e realize as requisições) ou "automática" (Clique na opção de "play" no canto superior direito da pasta > run > Run MyCollection).
