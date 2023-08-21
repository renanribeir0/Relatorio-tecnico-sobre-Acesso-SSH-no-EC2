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

<img width="454" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/4a1e8a27-babb-4553-ab01-68f46a6a3a1f">


Rolando a tela para baixo, encontramos a opção destacada em laranja “Executar Instância”:

<img width="454" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/2814e0f9-8e62-4f40-8650-dbdb2b4a83b3">


Clicando na opção, seremos redirecionados para a aba a seguir:

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/9881afe4-21ee-4cce-ad51-ab260b9a9119">


Nesta aba, temos a opção nome. Para adicionarmos um nome a nossa instância:

<img width="453" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/28186c5a-78c5-41c6-b3e0-11c9e3a194da">


Rolamos a tela para baixo e, onde teremos opção de escolher em qual sistema operacional queremos criar nossa instância, a escolha fica a critério de cada um:

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/d50840cb-8adf-4364-8a7d-25b68e335cf1">


Em “descrição”, temos duas opções: 64bits (x86) e 64bits (Arm).  64bits (x86) é mais indicado para computadores e 64bits (Arm) é mais indicado para smartphones.

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/a3f2e823-c356-4d19-ac52-56df8ce25180">


Rolando a tela para baixo, temos a opção de escolhermos o “tipo de instância”, a escolha fica a critério do usuário. Dica: atente-se ao valor cobrado em cada instância.

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/cc716af9-84d4-443b-8d4b-3783b9642b56">


Rolando a tela para baixo, teremos a opção “Par de chaves (login)”, onde você criará uma senha/chave para acessar a máquina que você está criando: Clique na opção “Criar novo par de chaves.

<img width="457" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/13e4aaac-ef7f-4f53-a0c1-c7019780eb86">


Você será redirecionado para esta aba, onde poderá criar sua chave. Após a criação da chave, clique no botão laranja “Criar par de chaves”.

<img width="457" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/1e101e69-3776-4533-9e63-5d0528de9941">


Rolando a tela para baixo, você terá a opção de  “configuração de rede”, configure da forma que você achar melhor.

<img width="454" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/61b1d541-2b8a-4c50-b33a-a3a34cf49cc7">


Rolando para baixo, você terá a opção “configuração de armazenamento”, escolha da forma que você achar melhor.

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/e80c023d-a615-44a7-8e9e-903a0ed9b0a6">


Após seguir o passos anteriores, clique no botão em laranja “Executar instância”

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/93ffb24f-a400-4b46-ad64-3224a13f30db">


Após isso, você será redirecionado para está página “Êxito”, o que significa que sua instância foi criada:

<img width="456" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/abbb4e94-ce9a-418d-8477-8cd4c1468d61">


Clicando no link “Execução da instância iniciada com êxito (i-07e0f1eaa08aeace3)”, você consegue ver detalhes da instância que você acabou de criar.

<img width="454" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/83b383ac-abfd-49e0-b302-50a8766318d7">


Assim1: 

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/c28c7ec3-dc9a-4ffe-91f8-c397fb01c98b">


Para acessar esta máquina, você pode fazer isso clicando na opção “conectar”, que está presente no topo da página:

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/ec81744a-681f-41a2-b24b-f2ad532c7660">


Assim, você direcionado para esta página:

<img width="458" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/c90b31a3-3831-4aea-9263-5fb3a6c8dec3">


Clicando na opção “Cliente SSH”, você recebe instruções:

<img width="456" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/ac03fbaf-ff05-4de4-8d8a-bfdf532c9200">


Acessando a máquina com o SSH, via CMD:
Na parte inferior, copie o caminho:  ssh -i "atividadeweb4.pem" ec2-user@ec2-184-72-83-242.compute-1.amazonaws.com 


<img width="454" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/3c732fb3-11f7-43b0-aebd-91b2754fbbac">


Entre no cmd (Prompt de Comando) do seu computador e cole o caminho copiado anteriormente.

<img width="455" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/c943ac5b-972b-4aea-9fb2-a54bc780da74">


Assim, você terá acesso a sua instância via SSH.

<img width="452" alt="image" src="https://github.com/renanribeir0/Relatorio-tecnico-sobre-Acesso-SSH-no-EC2/assets/110369271/d2987343-c44c-4b0d-9f30-2e186841aacb">












































