# Devops

Para começar a falar sobre o assunto, é importante entendermos: **O que é Devops?**

Só que essa pergunta é um pouquinho mais complicada do que parece… Então para começar vamos falar um pouquinho sobre a história de Devops.

Tudo começou em 2009 quando Patrick Debois assistiu uma palestra de John Allspaw e Paul Hammond chamada ***“10 deploys por dia: operação entre dev e ops”*** no Flickr. A partir daí surgiu essa ideia inicial, que depois foi utilizada pela primeira vez em 2009 pelo próprio Patrick no evento que ele chamou de Devops Day. O termo Devops foi formado pela junção das palavras *“desenvolvimento”* e *“operações”* e já dá uma boa dica do que quer dizer esse termo.

É importante comentar que **Devops não é um processo, não é uma tecnologia, não é um padrão, nem muito menos são ferramentas**. Devops é entendido como uma **cultura**, também sendo citado em alguns momentos como um movimento.

## Mas quais problemas levaram à criação da cultura Devops?

Aqui, eu vou mostrar um pouquinho para vocês de como era o cenário antes de surgir Devops:

De um lado, tem o nosso **desenvolvedor**, que está preocupado em fazer seu código, em fazer a criação das aplicações. Do outro lado, temos o cara de **operações**, que está preocupado em manter o ambiente estável, em fazer o gerenciamento dos servidores. Como muita gente sabe, sempre existiu uma rixa muito grande entre essas duas equipes, que normalmente era permeada por algumas frases do tipo:

***“Funcionou muito bem desenvolvimento agora é problema de operações”***
***“Na minha máquina funciona”***

E várias outras frases que a gente sabe que são ditas entre essas duas áreas. Então, pensando em acabar com esse atrito entre as áreas, em reduzir o tempo de resolução de problemas, em melhorar a velocidade e a qualidade das entregas e diminuir a probabilidade de erro em produção, surgiu a **cultura Devops**!

## Pilares

Ao falar da cultura Devops, existem alguns pilares muito importantes que definem essa cultura, que são eles:

*-   Colaboração;*
*-   Automatização;*
*-   Integração continua;*
*-   Entrega continua;*
*-   Testes contínuos;*
*-   Monitoração continua.*
    
### Colaboração

A ideia da cultura devops veio para **quebrar paradigmas e criar pontes**, removendo as barreiras entre as equipes de desenvolvimento e operações, que não traziam nenhum benefício, nem para as pessoas, nem para a empresa. Além disso ela quer criar uma mudança de comportamento buscando um bom relacionamento entre as áreas, abraçando as mudanças e as novas experiências já que, para entrar nesse mundo Devops, ambas as equipes precisam ter a mente aberta, para mudar totalmente a forma de trabalho.

### Automatização

Quando falamos sobre automatização, temos como principal foco **evitar a execução de tarefas de forma repetitiva**. Muitas das atividades do dia-a-dia eram executadas manualmente, exigindo mais mão de obra e dificultando o crescimento e aprendizagem da equipe. A ideia com a cultura Devops é automatizar desde o provisionamento dos ambientes, ou seja, a criação das máquinas, até realizar um deploy em produção. Com isso, conseguimos garantir muito mais economia de tempo e de recursos.

### Integração Contínua

Com a integração continua a ideia é **fugir do cenário que tinhamos antigamente de criação de grandes monolitos** (enormes blocos de código), que chegavam a demorar meses para chegar em produção e quando esse deploy era realizado, já tinha uma quantidade muito grande de alterações. A probabilidade de gerar um problema em produção nesse cenário era muito grande. Então, com a integração continua, a ideia é que sejam feitas **pequenas alterações no código de cada vez e essas alterações sejam levadas até produção**. Dessa forma, é muito mais fácil identificar e corrigir bugs, erros, ou qualquer problema no código antes de subir para produção, além de melhorar a produtividade do desenvolvedor e do código ser entregue com mais qualidade.

### Entregas contínuas

Com as entregas contínuas, a ideia é ter ferramentas e configurações para garantir que o **processo de Deploy e Rollback aconteçam de forma rápida e automatizada**, sem ter a necessidade do desenvolvedor precisar depender de alguém de operações para realizar esses procedimentos. A intenção é que o próprio desenvolvedor tenha a possibilidade de fazer o Deploy em todos os ambientes, utilizando uma esteira de deploy que vai desde o ambiente de desenvolvimento/homologação, até chegar em produção, sempre seguindo as regras de cada empresa.

### Testes contínuos

Com a cultura Devops, a intenção é de integrar os **testes necessários para garantir que a qualidade de código está satisfatória**, garantindo que o código que tá indo para produção é um código saudável, que está bem feito, integrando esses testes na pipeline (processo de deploy, baseado em várias etapas automatizadas). Assim, é possível garantir muito mais eficiência e padronização, além de economizar muito tempo em relação aos time de QA, que fariam esses testes manualmente.

### Monitoração continua

Com a monitoração contínua temos como objetivo garantir que **todas as fases desse ciclo de vida estejam sendo monitoradas**, além de tudo que está sendo utilizado em produção, para garantir integridade, desempenho e confiabilidade tanto das aplicações quanto da infraestrutura, desde o ambiente de desenvolvimento até produção. A ideia é sempre ter uma boa visibilidade sobre se as aplicações estão saudáveis, se o ambiente está saudável, se alguma coisa não está indo bem, para que seja possível fazer correções o mais rápido possível, diminuindo o impacto para o cliente final.

 ## Ferramentas
 
Para colocar em prática cada um desses pilares, existem diversas ferramentas que são utilizadas, que sustentam cada uma dessas etapas. Até por conta da quantidade enorme de ferramentas utilizadas por um devops, é muito comum ouvir as pessoas vincularem o termo devops a ferramentas. Aqui, vou citar algumas ferramentas que tenho mais familiaridade, porém não se prendam a essas ferramentas, pois existe uma diversidade enorme de ferramentas que podem ser utilizadas e não quer dizer que as citadas aqui são as melhores.

### Ferramentas de automação  

Na parte de automação temos como exemplo o **Ansible, Chef, Puppet**, entre outras. A ideia com essas ferramentas é automatizar atividades e executá-las em grande escala. Por exemplo: eu preciso alterar uma configuração em todas as máquinas do meu cluster e não quero ter que ficar acessando uma por uma das máquinas para fazer alteração. Com essas ferramentas, eu posso montar um playbook (que nada mais é que uma receita de tudo que deve ser feito nessas máquinas) e executar em todas as máquinas de forma remota, sem ter nenhuma atividade manual.

### Ferramentas de container

Na parte de containers, temos como exemplo o **Docker e o Kubernetes** que são muito utilizados em conjunto. O Docker é ferramenta utilizada para fazer um pequeno agrupamento de recursos dentro de uma máquina, que será utilizado para armazenar uma aplicação e todas as suas dependências, como libs e outros componentes, otimizando a utilização de recursos e garantindo muito mais segurança. O Kubernetes é um gerenciador de container, com ele é possível ter muito mais controle sobre os containers e muito mais escalabilidade, segurança e confiabilidade.

### Ferramentas de automação de build, deploy, testes

O **Jenkins** vai entrar em dois momentos porque ele é uma ferramenta que pode ser utilizada em várias etapas. Hoje, ele é uma ferramenta muito utilizada para automatizar o processo de build, de testes integrados, sendo fundamental para as etapas de integração e entrega continua. Ele é uma ferramenta muito robusta que ajuda em várias etapas do dia-a-dia Devops.

### Ferramentas de versionamento

Na parte de versionamento, temos **Git e GitLab**, que são algumas das ferramentas utilizadas como o controle de versões, sendo muito necessárias no desenvolvimento de software e fundamentais para a etapa de integração contínua, já que através delas é possível fazer o versionamento das alterações, visando ter sempre as versões anteriores que estavam estáveis disponíveis em caso de problemas, ou até mesmo permitindo que mais de um desenvolvedor trabalhe em cima da mesma aplicação ao mesmo tempo.

### Ferramentas de testes contínuos

Na etapa de testes continuos, o **SonarQube** é um exemplo de ferramenta utilizada para inspeção da qualidade de código. Ela consegue detectar odor de código e falhas de segurança em mais de 20 linguagens de programação, colaborando muito para identificar códigos que, por mais que pareçam estar bem feitos, podem precisar de alguns ajustes, o Sonar vai sinalizar para correção.

### Ferramentas de monitoração  

Falando em monitoração, falaremos de algumas ferramentas mas existe uma quantidade enorme de opções. Segue algumas delas:

*-   Prometheus;*
*-   Grafana;*
*-   Zabbix;*
*-   APM (Instana, NewRelic, Dynatrace);*
*-   Entre outras.*

Todas as ferramentas citadas acima são utilizadas para ter uma boa visibilidade de todo o ambiente, desde as aplicações, mostrando erros que podem estar ocorrendo, picos de latência, além de toda a parte de infraestrutura, permitindo a criação de alertas de que algum serviço tá fora.

## Por que que as empresas querem a cultura devops?

Agora que já conhecemos um pouco sobre Devops, vem a pergunta: *Por que que as empresas querem a cultura devops?*

Hoje Devops é a estratégia chave para aumento da produtividade na área de TI das empresas, sendo parte fundamental na redução de erros e entregas mais rápidas. Alguns pontos importantes para a tomada de decisão são:

**-   Economia de tempo e recursos:** sabemos que tempo é dinheiro. Então, um projeto que demora muito tempo para ser entrega, que está estrapolando prazos ou que toda hora precisa de correção, gera muito prejuízo. Com Devops, o desenvolvimento é feito com mais qualidade, trabalhando de forma mais estratégica e automatizada e consequentemente gerando menos desperdício de recursos;
    
**-   Otimização de processos**: as etapas das atividades são facilitadas, fluindo de maneira mais rápida e mais produtiva. Então, essa otimização de processos é boa não só para equipe de devops, mas acaba influenciando também outras áreas da empresa, melhorando a performance de forma geral;
    
**-   Melhora na qualidade:** a cultura Devops tem como objetivo fazer com que as equipes se comuniquem melhor e compreendam que todos precisam ajudar para atingir os objetivos da empresa;
    
**-   Melhoria na velocidade de produção:** pois como os processos são desenvolvidos com a utilização da esteira para evolução do código, desde desenvolvimento até produção, acaba sendo muito mais rápido do que no padrão de trabalho anterior, além de ter uma menor probabilidade de erros e atrasos;
    
**-   Aumento da motivação:** quando existe um ambiente mais propício para o desenvolvimento profissional, que tem possibilidade de evolução constante, que tem incentivos a colaboração entre as equipes, a probabilidade de ter um profissional mais motivado é muito grande.
    
## Para trabalhar como devops, precisa ter trabalhado com infraestrutura? 

Uma dúvida muito comum é: *para trabalhar como devops, precisa ter trabalhado com infraestrutura?* **Não!** Tanto pessoas de desenvolvimento quanto de infraestrutura podem trabalhar como devops. Ter devops com diferentes backgrounds enriquece muito o dia-a-dia, pois traz diferentes pontos de vista para uma mesma situação.

*A cultura Devops surgiu para resolver problemas comuns de falha de comunicação e consegue entregar diversas outras soluções para as áreas de TI, sendo assim uma cultura altamente utilizada utilmamente e com alto indice de sucesso.*

## Leituras Recomendadas/Fontes:

-   The Devops Handbook, de Gene Kim, Patrick DEbois, John Willis, John Allspaw e Jaz Humble
-   The Phoenix Project, de Gene Kim, George Spafford e Kevin Behr.Para começar a falar sobre o assunto, é importante entendermos: O que é Devops?