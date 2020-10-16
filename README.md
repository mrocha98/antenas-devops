# Laboratório de Projeto de Banco de Dados V – 2020.2
Este repositório é utilizado para compartilhar as entregas para a disciplina de Laboratório de Projeto de Bando de Dados V, ministrada pelo professor Eduardo Sakaue. 
O objetivo do projeto é implementar um conjunto de melhores práticas de desenvolvimento de software (Dev) e operações de TI (Ops), DevOps para disponibilizar a aplicação web Antenas.

## O que é o Projeto Antenas
Projeto desenvolvido pelos alunos da FATEC - Professor Jessen Vidal, para a matéria Padrões de Projeto, ministrada pelo Professor Giuliano. 
O software é uma iniciativa para aproximar os alunos das necessidades do mercado de trabalho. Consiste em uma aplicação web onde empresas da área de tecnologia propõem desafios, o conteúdo é avaliado pelos professores da Fatec e então enviado para que os alunos proponham soluções. 

## Equipe:
- Bruno Akira Ota;
- Gabriel Pereira Bastos;
- Leticia Macedo Prudente de Carvalho;
- Matheus Rocha da Silva;
- Thaís Bitencourt de Meneses;
- Vanessa Bessa Diogenes Castellano; e
- Yan Rodrigues de Azevedo.



## Repositórios:
Front-end: <https://github.com/mrocha98/antenas-front>

Back-end: <https://github.com/mrocha98/antenas-back>

## Acesso à aplicação:
http://18.231.13.0:3000/

## Acesso para desenvolvimento:
É necessário instalar o docker:
https://docs.docker.com/get-docker/
https://docs.docker.com/compose/install/

O nodeJS, na versão 12 ou posterior:
https://nodejs.org/en/download/

E utilizar uma IDE para visualizar o código; recomendamos o VSCode: 
https://code.visualstudio.com 


## Tecnologias:

### AWS (EC2)
Utilizado para hospedar e disponibilizar o software online para o cliente. Escolhemos a plataforma pela popularidade, por conta da escalabilidade de servidores e pela fácil integração com os demais serviços que a empresa oferece.

### GitHub
Aplicação web utilizada para o versionamento e centralização do projeto.

### Docker-compose
Utilizado para criar imagem do mongobd para que a infraestrutura não precise ser configurada. Foi utilizado para que os participantes do projeto não tivessem problemas de compatibilidade de ambiente. 

### Jest
Estrutura de teste de JavaScript, utilizada para fazer testes unitários e garantir que a aplicação está funcionando de acordo com os requisitos do negócio. Foi escolhido por ser open source, não necessitar configuração manual, possuir relatório de código de fácil acesso e pela velocidade, pois roda testes em paralelo. 

### Cypress
Framework de testes automatizados end-to-end usando JavaScript, utilizada para refletir as ações dos usuários. A ferramenta foi escolhida por ser open source, possuir recarga em tempo real, espera automática e ser responsivo com aplicações da web.

### MongoDB Atlas
Banco de dados em nuvem para MongoDB. A ferramenta foi escolhida por estar disponível via web e porque a infraestrutura, manutenção das máquinas e segurança não precisam de configuração manual.

### Zabbix
Uma ferramenta de software de monitoramento de código aberto para diversos componentes de TI, incluindo redes, servidores, máquinas virtuais e serviços em nuvem. O Zabbix fornece métricas de monitoramento, entre outras, utilização da rede, carga da CPU e consumo de espaço em disco.

## Road Map

![ilustração do road map](.github/images/roadmap.jpeg)

## Entregas

### Sprint 01 – 20/09/2020
- Deploy do Frontend e Backend: disponibilizar aplicação em ambiente remoto na [AWS EC2](https://aws.amazon.com/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc) ;
- [Configuração do arquivo Docker-compose](https://github.com/mrocha98/antenas-back/blob/master/docker-compose.yml) : integrar MongoDB e NodeJs para utilizar em ambiente de desenvolvimento; e para utilizarmos em desenvolvimento
- Criação do banco em nuvem:  disponibilizar a base de dados em ambiente remoto, no [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) .

### Sprint 02 – 04/10/2020
- Testes unitários: utilizado para verificar a menor parte testável da aplicação, garantindo que o software esteja de acordo com as regras de negócio, minimizando o retrabalho e tornando as correções mais ágeis.
- Integração contínua: fará com que cada alteração passe pelos testes antes de efetivar o commit, trazendo mais segurança e agilidade ao processo de desenvolvimento já que os testes são executados automaticamente.


### Sprint 03 – 18/10/2020
- Divisão dos ambientes em homologação/desenvolvimento, QA/Testes e Produção: Essa divisão se faz necessária para que nenhuma funcionalidade seja desenvolvida e/ou testada no ambiente de produção e assim blindar o ambiente do cliente de qualquer problema. Essa divisão também é benéfica para que os desenvolvedores e testes saibam que o ambiente que estão utilizando se encontra da melhor forma possível.
- Integração da ferramenta de monitoramento Zabbix para gerar logs: A geração de logs é importante para que possamos avaliar onde pode estar ocorrendo algum erro ou fazer o monitoramento do sistema para que se caso haja algum erro, seja possível identificar de forma rápida e precisa para uma correção mais acertiva.
- Deploy automático.


### Sprint 04 – 01/11/2020
- Testes de integração automatizado; e
- Implementação do load balance.



### Sprint 05 – 15/11/2020
- Testes de carga; e
- Testes E2E (end-to-end) automatizado.


### Sprint 06 – 29/11/2020
- Documentação de funcionalidades para usuários 
- Vídeo de apresentação que será apresentado na feira de soluções. 


