# Azure Frontier Girls Challenge
## Objetivo e descrição
Este challenge tem como ideia principal criação de um agente para automação de envio de e-mails como lembretes de eventos. O diferencial é fazer esse agente ter uma abordagem similar ao do robô Baymax, do filme "Operação Big Hero", mostrando um pouco de informalidade, gentileza e dediação. Em adição foi implementada a informação sobre o tempo da cidade requisitada, para informar ao usuário e dar dicas, caso necessário, para como agir de acordo com o tempo. Uma melhor descrição do que foi inserido será dada ao decorrer dos **passos**, bem como os **prints de respostas**, incluindo também um **vídeo** ao final, mostrando a **execução do agente** em tempo real e seus resultados.
## Fluxo
O fluxo do agente está de acordo com as **imagens** mostradas a seguir e tem o seguinte curso:  
1. O chat faz a chamada para o agente;
2. O agente usa o Outlook e escreve parte do e-mail;
3. Para que as informações sejam preenchidas o agente as lê no arquivo enviado;
4. O agente, então, solicita as informações de tempo para aquela cidade em específico;
5. Com as informações completas, o e-mail é finalizado e o agente o envia;
6. A resposta é enviada ao chat através do agente, com o resultado do envio e o resumo do que foi enviado.  

Nos **prints** abaixo também estão os *inputs* e *outputs*, bem como o *metadata*.
![alt text](image-24.png)
![print fluxo 1](image-22.png)
![print fluxo 2 metadata](image-23.png)

>## Passos
>Para a execução do objetivo foram seguidos os seguintes **passos**:
## Passo 1
Fork do Challenge no Github
![print do fork](image-1.png)

## Passo 2
Criação da conta da Azure, na localização "Canada East"
![print conta azure](image-2.png)

## Passo 3
Criação do grupo de recursos 
![print resource group](image-3.png)

## Passo 4
Criação do AI Foundry
![print ai foundry](image-4.png)

## Passo 5
Passar o plano para pay-as-you-go.
##### Obs: houve uma dificuldade neste passo que foi resolvida através de revisão de aulas gravadas e consultas no grupo do curso, até então foi a parte de mais dificulade.
![print pay-as-you-go](image-6.png)

## Passo 6
Implantação do modelo, utilizando o gpt4.1, na localização "Canada East"
![print gpt4.1](image-5.png)

## Passo 7
Criando e instruindo o agente. Nesta seção foi criado o agente e definido qual seriam seus objetivos e ações a serem tomadas. Nesta etapa foram definidas as seguintes intruções:  
>Você é um Agente de envio de e-mails de lembretes de eventos. Você envia e-mails como se fosse o robô Baymax, do filme Operação Big Hero, para lembrar ao usuário que ele possui algo agendado para um horário próximo ao atual. Você não responde perguntas sobre qualquer outro assunto. Você envia e-mail somente sobre lembretes.

e a seguinte descrição do agente:
>Envia e-mails de lembretes de eventos como se fosse o Baymax, do filme Operação Big Hero.
![print criacao agente](image-8.png)

## Passo 8
Teste funcional do agente no playground. Foi feito um teste com o agente antes de enviar um e-mail, para checar se o conteúdo e linguagem estavam de acordo com a proposta inicial.
![print teste baymax](image-7.png)
![print teste baymax 2](image-9.png)

## Passo 9
Um e-mail para o agente foi criado, com uma assinatura do Office 365 outlook.
![print outlook](image-11.png)

## Passo 10
Foi adicionada uma ação para que o e-mail seja enviado de um e-mail válido, usando os recursos disponíveis.
![print acao agente](image-10.png)

## Passo 11
Ao adicionar a ação, mais testes foram enviados para verificar se o agente estava concluindo suas tarefas com êxito. Os testes foram bem sucedidos.
![print acao agente](image-12.png)
![print acao email](image-13.png)

## Passo 12
Uma lista de pessoas com nomes, e-mail e eventos fictícios foi criada, com a ajuda do ChatGPT. Uma linha com informações válidas foi adicionada para fins de testes de agente.
![print lista](image-14.png)

## Passo 13
O arquivo contendo a lista de pessoas fictícias foi adicionado a parte de "Conhecimento", para agregar o agente.
![print conhecimento](image-15.png)

## Passo 14
Mais testes foram feitos com o agente para testar novamente se tudo estava de acordo. Os e-mails foram enviados com as informações corretas.
![print teste conhecimento](image-16.png)
![print e-mail conhecimento](image-17.png)

## Passo 15
Foi adicionada uma ação para alertar como estará o tempo, caso necessário, na cidade da pessoa e ajudá-la com dicas para se previnir.
![print tempo acao](image-18.png)

## Passo 16
Com a nova implantação, mais teste foram executados para verificar se o agente correspondia ao esperado e se a adição de mais uma ação não havia interferido negativamente nos resultados. Novamente o agente enviou as informações corretamente.
![print teste tempo](image-19.png)
![print email tempo](image-20.png)

## Vídeo
O vídeo a seguir tem como propósito demonstrar o agente em ação, executando aquilo que foi solicitado e, de acordo com a ideia e objetivo proposto, enviando para o remetente requerido as informações necessárias para lembrar-lhe do evento que ocorrerá, o dia em que ocorrerá e ainda uma informação a mais para dar dicas sobre o tempo na cidade previsto para o dia em questão.  
###### (Clique na imagem para redirecionar ao vídeo)
[![video agente challenge](image-21.png)](https://youtu.be/6G2CTT74gDA)

## Referências
* https://github.com/Miyake-Diogo/AzureFrontierGirls-AI-Challenge/blob/main/README.md
* https://tinyurl.com/azuremicrosoftafgchallenge
* https://ai.azure.com
* https://excalidraw.com