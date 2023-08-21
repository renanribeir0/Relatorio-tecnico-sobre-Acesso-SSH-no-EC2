# Relatório Técnico: Criação e Acesso a uma Instância EC2 na AWS

## Introdução

Este relatório descreve o processo de criação de uma instância de máquina EC2 na Amazon Web Services (AWS) e o acesso a essa instância utilizando a ferramenta PuTTY para estabelecer uma conexão SSH. O objetivo é demonstrar os passos necessários para criar e acessar uma instância EC2, registrar o processo e capturar as evidências visuais do procedimento realizado.

## Objetivo

O objetivo deste relatório é guiar o leitor através das etapas para criar uma instância EC2 na AWS e acessá-la por meio de uma conexão SSH utilizando a ferramenta PuTTY. O processo será documentado em um arquivo Markdown hospedado em um repositório GitHub, contendo evidências visuais do console da AWS, acesso SSH bem-sucedido e informações relevantes da instância criada.

## Materiais

- Conta ativa na AWS
- Acesso à interface de linha de comando do Git


## Método

Na página inicial do console, clique em na engrenagem EC2:

<img width="363" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/da1462d5-ac58-4db2-ad83-6f94dca897c0">


Logo após, você será redirecionado para a aba instâncias:


Rolando a tela para baixo, encontramos a opção destacada em laranja “Executar Instância”:




Clicando na opção, seremos redirecionados para a aba a seguir:


Nesta aba, temos a opção nome, logo abaixo uma caixa “por exemplo meu servidor Web”, para você adicionar um nome para sua instância.


após adicionar o nome:


Rolamos a tela para baixo e, onde teremos opção de escolher em qual sistema operacional queremos criar nossa instância, a escolha fica a critério de cada um:



Em “descrição”, temos duas opções: 64bits (x86) e 64bits (Arm).  64bits (x86) é mais indicado para computadores e 64bits (Arm) é mais indicado para smartphones.


Rolando a tela para baixo, temos a opção de escolhermos o “tipo de instância”, a escolha fica a critério do usuário. Dica: atente-se ao valor cobrado em cada instância.
 

Rolando a tela para baixo, teremos a opção “Par de chaves (login)”, onde você criará uma senha/chave para acessar a máquina que você está criando: Clique na opção “Criar novo par de chaves  


Você será redirecionado para esta aba, onde poderá criar sua chave. Após a criação da chave, clique no botão laranja “Criar par de chaves”.



Rolando a tela para baixo, você terá a opção de  “configuração de rede”, configure da forma que você achar melhor.

Rolando para baixo, você terá a opção “configuração de armazenamento”, escolha da forma que você achar melhor.



Após seguir o passos anteriores, clique no botão em laranja “Executar instância”

Após isso, você será redirecionado para está página “Êxito”, o que significa que sua instância foi criada:










Clicando no link “Execução da instância iniciada com êxito (i-07e0f1eaa08aeace3)”, você consegue ver detalhes da instância que você acabou de criar.


Assim1: 







Para acessar esta máquina, você pode fazer isso clicando na opção “conectar”, que está presente no topo da página:








Assim, você direcionado para esta página:




Clicando na opção “Cliente SSH”, você recebe instruções:






























Acessando a máquina com o SSH, via CMD:

Na parte inferior, copie o caminho:  ssh -i "atividadeweb4.pem" ec2-user@ec2-184-72-83-242.compute-1.amazonaws.com 




Entre no cmd (Prompt de Comando) do seu computador e cole o caminho copiado anteriormente.




Assim, você terá acesso a sua instância via SSH.











































