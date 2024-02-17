# Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados

## Objetivo 🎯

Entrega do desafio DIO - Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados

## Instruções (PT-BR)

1- Entre no portal do Azure usando https://portal.azure.com e acesse com suas credenciais da Microsoft.

2- Em "Create a resource" selecione "AI Search" e clique em "Create"

3- Crie um recurso e preencha as informações necessárias, após clique em "Review + Create" (esse passo pode demorar alguns minutos, aguarde a mensagem de sucesso)

Obs.: Para Pricing Tier selecione a opção "Basic"

Obs.: Caso ainda não possua um Resource Group, basta clicar em "Create New" e criar um com título desejado

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/9ddc3439-ee47-4214-8fa7-2307b0528736)


4 - O passo seguinte será criar um recurso de IA. Para isso vá em "Create a resource" seleciona "AI + Machine Learning" e após em "Azure AI Services" clique em Create

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/1a8f8551-ba14-4613-b256-481b1a5f6d37)

5- Crie um recurso e preencha as informações necessárias, após clique em "Review + Create" (esse passo pode demorar alguns minutos, aguarde a mensagem de sucesso)

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/ea7d5918-c9fd-4365-9330-67c6cefb28c3)

6-Após a criação dos dois serviços "AI Search" e "Azure AI services", prosseguiremos com a configuração da "Storage Account". Para isso, pesquise por "Storage Account" na caixa de pesquisa do Azure e, em seguida, clique em "Create" após selecioná-lo.

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/e5b2dad4-692d-4b47-82e6-68cce3090d6b)

7- Para seguir com a criação, preencha as informações necessárias, após clique em "Review" e após "Create" (esse passo pode demorar alguns minutos, aguarde a mensagem de sucesso)

Obs.: Para Performance selecione Standard

Obs.: Para Redundancy selecione LRS

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/334b7ba2-de78-48e6-8d45-1a4f0b33ffb0)

8- Para esse laboratório será necessário liberar o acesso anónimo no Store Acconut. Para isso acesse em Configuration em Settings. Após marque em "Allow Blob anonymous access" a opção "Enabled"
-Salve

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/0dfe9d49-848b-481d-8b5b-38801eac254e)e 


9- Agora será o momento de carregar os arquivos no Containers. Para isso vá em "Containers" e clique em "+ Containers"

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/6b4c2c82-c77c-4c8f-bcbb-55a5912ae858)

10- Para esse labotatório, ao criar um novo container, em "Anonymous access level" selecione a opção "anonymours read access for containers and blobs"

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/7351e3da-cda6-40ef-b1bc-3cc88ddc8582)


11- Abra uma nova guia no seu navegador da web.
No campo de endereço, digite ou cole o seguinte link: https://aka.ms/mslearn-coffee-reviews.
O download das avaliações de café será realizado automaticamente.
Após o download ser concluído, localize o arquivo em seu computador e extraia-o para acessar seu conteúdo.

12- No container criado, clique em Upload para carregar os arquivos extraidos.

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/d07851af-70e8-4e3c-a511-c567d416b4be)

13- Os arquivos serão carregados no container selecionado.

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/3d1a8b91-8d83-47e5-82c9-d6ee6512a48b)

14- Até o momento já foi criado: o mecanisco de busca, um recurso de IA e um armazenamento em nuvem com alguns arquivos.

15- Vá até o mecanismo de busca criado durante o passo 2. Dentro do AI Search criado, clique em Importar Dados.

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/fe9717ad-0f1c-4fc9-817a-f93e4f3fe4c9)

16- Na tela de Importar Dados, em Data Source selecione a opção "Azure Blob Storage"

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/ca302729-d040-489b-8277-70adede844f0)

17- Será necessário preencher as informações e selecionar a conexão com o container criado no storage accont.

-Informações que serão preenchidas. Para blob folder pode deixar o preenchimento em branco.
![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/1f8914d0-69e3-4b37-8041-b667728f6d1d)

-Em "Connection string" clique em "Choose an existing connection" e siga com a seleção do storage account e container criados.

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/02d6f3cc-01dd-43b5-8225-8d9126f147b9)

18- Retorne a página anterior e vá para "Search explorer"

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/9ba1c9df-5aad-4fb0-9658-fa5593ada039)

19- Nessa tela o Index já virá prenchido conforme criado no passo anterior. E poderemos realizar a pesquisa conforme necessário.

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/965be08d-becc-4fb3-8a84-c551f74300b6)

Dica: brinque um pouco com a pesquisa usando o query options ou json.

![image](https://github.com/ellizsillva/LabDioIA900---Cognitive-Search/assets/155840444/0623433c-6467-4f06-9564-c15c84c31bcc)


# Doc de Referência - Lab Microsoft

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html
