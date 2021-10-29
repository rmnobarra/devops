1. O que é devops

Muita gente fala bastante coisa sobre devops, eu gosto de tomar inspirações do que as gigantes do mercado
falam.

Microsoft

DevOps é a união de pessoas, processos e produtos para permitir a entrega contínua de valor aos nossos usuários finais.

Red hat

DevOps descreve abordagens para acelerar os processos pelos quais uma ideia (como um novo recurso de software, uma solicitação de aprimoramento ou uma correção de bug) vai do desenvolvimento à implantação em um ambiente de produção onde pode fornecer valor ao usuário.

Google

O movimento organizacional e cultural que visa aumentar a velocidade de entrega de software, melhorar a confiabilidade do serviço e construir propriedade compartilhada entre as partes interessadas do software

Em todos essas frases, algumas palavras se destacam

pessoas
processos
aceleração
cultura
compartilhamento

Eu tb acredito e vivo isso, devops mais do que uma coleção de ferramenta, fabricante, é cultura

2. Quais são os benefícios do DevOps? O que isso pode nos ajudar a alcançar?

Colaboração

Melhor entrega

Segurança

Velocidade

Escala

Confiabilidade

3. Como tudo começou?

Para falarmos sobre a história sobre DevOps, precisamos retroceder no tempo e falar sobre desenvolvimento e também sobre o manifesto ágil. Em 2001, 17 desenvolvedores reuniram-se nas montanhas nevadas do estado norte-americano de Utah para discutir metodologias para processos de desenvolvimento e o resultado deste encontro foi o então chamado manifesto ágil.

# Manifesto agil

O Manifesto Ágil é uma declaração de valores e princípios essenciais para o desenvolvimento de software.

Basicamente, o manifesto ágil afirma que melhores resultados no desenvolvimento de software podem ser obtidos através da valorização de:

Indivíduos e interações, mais que processos e ferramentas

Software em funcionamento, mais que documentação abrangente

Responder a mudanças, mais que seguir um plano


# Agile Conference

Em 2008 Andrew Schafer apresentou sua palestra de infraestrutura ágil para apenas uma pessoa, Patrick Debois. Guardem esses nomes. =)

# Velocity Conference

Em 2009, na Velocity Conference da O’Reilly, John Allspaw e Paul Hammond apresentaram “10+ Deploys per Day: Dev and Ops Cooperation at Flickr”. Jogando luz a temas como

Interação entre os Desenvolvedores e a equipe de operações;
Como conseguir um aumento dos deploys com ferramentas e mudanças culturais.
Após lamentar no twitter sua não participação na palestra, Patrick Debois, recebeu a resposta do time do Flickr:

“Porque não organizar sua própria conferência de Velocity na Bélgica?”

# DevopsDays

Motivado pela palestra dos engenheiros da Flickr, Patrick Debois decidiu criar sua própria conferência na Bélgica, que ficou conhecida como DevOpsDays e foi um sucesso. Para lembrar o dia, foi criada a tag #DevOps no Twitter, que posteriormente seria usado como o nome da cultura.

Ai o resto é história

4. Pilares

# C de Cultura

Respeite a cultura.
Precisamos colaborar, compartilhar e entender a importância de manter uma relação saudável entre todas as áreas para que as equipes multidisciplinares possam trabalhar juntas e atingir os resultados.

# A de Automação

Automatize se possível
Quando falamos de DevOps, queremos eliminar o máximo de trabalho laboral possível, trabalho laboral é aquele trabalho repetitivo. Se você, por exemplo, gasta todo dia 30 minutos para efetuar uma determinada ação, porque não gastar um tempo superior, como, por exemplo, 2 horas para automatizar esta rotina e poupar esses 30 minutos a partir de então?

# M de Medição

Meça os resultados
Precisamos medir tudo que é possível: de processos a pessoas. Afinal, a única maneira de verificar se estamos no caminho certo ou melhorando é através da medição. O processo de melhoria contínua é o coração do DevOps!

# S de Compartilhamento Compartilhando feedbacks

Ambientes DevOps têm como uma das características fundamentais a cultura Blameless ou, em português, “Sem Culpa”, que é exatamente o que cria um ambiente propício ao compartilhamento. Não é sobre ninguém ser culpado por uma determinada ação que levou os sistemas a ficarem indisponíveis, é sobre todos se sentirem seguros e não terem medo de cometer erros. O erro faz parte do processo de aprendizado e deve ser compartilhado, assim como todas as melhorias que aplicamos em nosso ambiente de trabalho

5. Conhecimentos e tecnologias

# Aprenda alguma linguagem de programação

Pode começar com shell script ou power shell, vai te ajudar a entender melhor as linguagens no futuro

# Conceitos de sistemas operacionais

gerenciamento de processo

threads e concorrencia

sockets

básico de redes

I/O

virtualização

memória

storage

file system (xfs, brts, nfs)

# gerenciamento de servidores

unix / linux / windows

falando em linux, é bom aprender a se virar bem em um terminal

# redes e protocolos

http

https

ssl / tls

ssh

dns

# infraestrutura como código

containers - docker, podman, lxc

# gerenciamento de configuração

ansible

chef

salt

puppet

# orquestração de containers

kubernetes

# provisionamento de infraestrutura

terraform

# cloud providers

aws

gcp

azure

heroku

# observabilidade

log

tracing

monitoramento

6. CI/CD

CI/CD, continuous integration/continuous delivery, é um método para entregar aplicações com frequência aos clientes. Para isso, é aplicada a automação nas etapas do desenvolvimento de aplicações. Os principais conceitos atribuídos a esse método são integração, entrega e implantação contínuas. Com o CI/CD, é possível solucionar os problemas que a integração de novos códigos pode causar para as equipes de operações e desenvolvimento (o famoso “inferno de integração”).

Qual é a diferença entre CI e CD (e o outro CD)?

O acrônimo CI/CD tem alguns significados. “CI” sempre se refere à integração contínua, que é um processo de automação para desenvolvedores. Uma CI bem-sucedida é quando novas mudanças no código de uma aplicação são desenvolvidas, testadas e consolidadas regularmente em um repositório compartilhado. É a solução ideal para evitar conflitos entre ramificações quando muitas aplicações são desenvolvidas ao mesmo tempo.

“CD” se refere à entrega contínua e/ou à implantação contínua, conceitos relacionados e usados alternadamente às vezes. Em ambos os casos, se trata da automação de fases avançadas do pipeline, mas são usados às vezes separadamente para ilustrar o nível de automação presente.

Geralmente, a entrega contínua representa as mudanças feitas pelo desenvolvedor em uma aplicação, que são automaticamente testadas contra bugs e carregadas em um repositório, como o GitHub, ou em um registro de container. Nesse repositório, a equipe de operações pode implantar essas mudanças em um ambiente de produção ativo. Isso resolve o problema de baixa visibilidade e comunicação entre as equipes de negócios e desenvolvimento. Para isso, a finalidade da entrega contínua é garantir o mínimo de esforço na implantação de novos códigos.

A implantação contínua, outro significado para “CD”, se refere ao lançamento automático das mudanças feitas por um desenvolvedor do repositório à produção, onde podem ser usadas pelos clientes. Isso evita a sobrecarga das equipes de operações por conta dos processos manuais que atrasam a entrega de aplicações. Nesse conceito, são aproveitados os benefícios da entrega contínua ao automatizar a próxima etapa no pipeline.

Por fim, não vale a pena se prender a esses conceitos. Basta se lembrar de que o CI/CD é, na verdade, um processo muitas vezes visto como um pipeline, que envolve a inclusão de um alto nível de automação e monitoramento contínuos no desenvolvimento de aplicações. Em cada caso, o que esses termos querem dizer depende da quantidade de automação implantada no pipeline de CI/CD. Muitas empresas começam adicionando CI e depois trabalham para automatizar a entrega e implantação.

7. Devops aderente na realidade, ou não.

Há uma expressão popular na área de TI que diz que todas as empresas atuais são também empresas de softwares. E a habilidade em fornecer novos serviços e funcionalidades aos clientes com rapidez é um dos principais diferenciais competitivos. A agilidade da TI é o segredo para que startups superem os enormes desafios e vençam as grandes batalhas. Surfar essa onde é o que podemos chamar de Transformação Digital.

# Transformação Digital

A transformação digital é uma mudança estratégica para as empresas. Com ela, é possível adaptar os principais serviços de acordo com as demandas do setor ou conforme novas regulamentações surgem, bem como lançar atualizações à medida que surgem novas vulnerabilidades.


Não existe uma definição comum para a transformação digital, mas podemos dizer que ela envolve um processo de “mudança”. Algumas vezes, esse termo é usado para designar novas arquiteturas (como microsserviços), novos processos (como DevOps) ou novas tecnologias (como os containers e interfaces de programação de aplicações).

# Transformação Digital, faz sentido?

• O Walmart implantou código durante a Black Friday, quando 200 milhões de pessoas estavam on-line.

• A Amazon implanta atualização de códigos a cada segundo (50 milhões por ano) em centenas de aplicativos e milhões de instâncias de cloud.

• A Etsy realiza 60 implantações por dia com um aplicativo monolítico.

• A Netflix realiza implantações centenas de vezes ao dia em uma arquitetura distribuída complexa. A empresa faz uma única alteração no código, indo do check-in à produção em 16 minutos.


# Resumindo

Transformação digital é uma mudança de mentalidade que as empresas passam com o objetivo de se tornarem mais modernas e acompanharem os avanços tecnológicos que não param de surgir.

8. Devops & Transformação Digital

A base da evolução digital é o DevOps. Assim como a estratégia corporativa, as aplicações são um reflexo das equipes e da comunicação entre elas. DevOps, ou mudanças similares nos processos, faz com que mais pessoas participem das discussões de desenvolvimento e, assim, oferecer insights mais amplos sobre como a equipe de operações mantém o software e a infraestrutura e como clientes e parceiros realmente usam essas aplicações. 

Ele cria um ciclo de feedback mais fechado entre as equipes, com linhas abertas de comunicação. E essa comunicação aberta é a base para qualquer outra etapa da evolução.

Ou seja, novamente pessoas, cultura, comunicação, compartilhamento, mais uma vez não falamos nada sobre ferramentas. Perceba que tanto a história
como dados sugerem algum tipo de mudança que muitas vezes começa com a cultura para permitir essas evoluções

9. Devops & Cultura

É importante notar que a evolução do software não é apenas uma mudança na tecnologia. Ela alterna entre mudanças em processos, equipes e infraestrutura, e as modificações culturais são infinitamente mais importantes.

É possível criar o diagrama de arquitetura mais perfeito e desejado. Depois de envolver as equipes e os processos, é preciso criar um ambiente cultural que ofereça suporte à entrega contínua e à disciplina no uso da arquitetura. Porque uma mudança nos processos ou na estrutura não é duradoura. As pessoas não são como os computadores que seguem regras. Portanto, as estruturas legadas da organização sempre destruirão a sua bela arquitetura.”

Para que o software e a tecnologia evoluam, o segredo é pensar na evolução como um processo natural do ambiente. Em uma empresa, isso é a cultura. Para garantir isso, as mudanças necessárias podem ter o suporte do gerenciamento, mas não podem ser impostas por ele. As pessoas precisam querer mudar. É uma questão de livre-arbítrio, e não imposição.

# Dados

O Gartner tem um dado que explica isso melhor: “90% das organizações que tentam usar o DevOps sem mudar especificamente a cultura falham.”

# A lei de conway

Melvin Conway, autor da célere frase que talvez tenha ficado conhecida por estar no livro O mítico homem-mês, um clássico da engenharia de software

A Lei de Conway diz: “Qualquer organização que criar um sistema, inevitavelmente, produzirá um projeto com uma estrutura igual a da comunicação da organização.” Isso pode ser interpretado de duas formas:

• Mudanças na arquitetura ou infraestrutura não terão qualquer efeito, a menos que você também modifique a estrutura de comunicação.

• Alterações na estrutura de comunicação resultarão em melhores processos e infraestrutura (independentemente da infraestrutura atual).

10. Devops como primeiro passo

Falar sobre devops é falar sobre agilidade, e indo as origens do devops, a metodologia agil é uma abordagem de design de software que tenta unir todas as partes envolvidas em um grupo mais coeso, possui diversos tipos de iterações e controle para as entregas

O ponto é que a metodologia ágil ainda lida somente com metade do verdadeiro ciclo de vida de uma aplicação. Depois de desenvolvido, a aplicação é transferida para a equipe de operações. Ela fica responsável pela implantação e suporte e ai que começa a ficar complexo, para dizer o mínimo.

# Problemática

O problema é que a equipe de operações nem sempre sabe o propósito da aplicação, o que pode gerar uma implantação menos eficiente. Os desenvolvedores podem não ter conhecimento sobre o verdadeiro ambiente operacional e criar uma aplicação que não tenha um bom desempenho no ambiente de produção. Então, para mitigar o risco de alterações, muitas organizações instituem um processo oneroso de gerenciamento de mudanças para tentar explicar e justificar qualquer alteração.

# Endereçando o problema

O DevOps é uma mudança cultural que tenta acabar com a separação entre os desenvolvedores, equipe de operações e demais envolvidos. A separação entre esses grupos é real, mas artificial. Uma equipe pode ser formada com profissionais de diversas funções. O DevOps tenta redefinir a equipe para incluir todos os grupos envolvidos no ciclo de vida de uma aplicação e criar uma abertura na comunicação entre esses grupos.

E transpassar essa barreira, a recompensa pode ser bem agradável

# Efeitos

O relatório “Puppet’s State of DevOps” mostra a eficácia alcançada ao mudar a estrutura e a comunicação da equipe. 11 O estudo revelou que as equipes de DevOps alcançam:

• Tempo de provisionamento 2.555 vezes mais rápido.

• 200 vezes mais implantações.

• Recuperação de falhas 24 vezes mais rápida.

• Taxa de falhas na mudança 3 vezes menor.

• 22% menos tempo gasto em retrabalho.

A rapidez é uma das principais vantagens do DevOps. Ao analisarmos todo o processo de lançamento, fica claro a necessidade de ter todas essas diferentes equipes envolvidas para a disponibilização de um aplicativo. O nível de esforço para o lançamento desse aplicativo irá depender da transparência e clareza dos processos, infraestrutura e base de códigos.

11. SRE - Site Reliability Engineer (Engenheiro de Confiabilidade de Sites)

SREs são, antes de tudo, Engenheiros. Profissionais de diferentes áreas da TI que aplicam os princípios da ciência da computação e da engenharia ao desenvolvimento de sistemas

SRE é o que acontece quando você pede a um engenheiro de software para projetar uma equipe de operações.

# Confiabilidade

SRE é sobre confiabilidade. Ponto.

Comum a todos os SREs é a crença e a aptidão para desenvolver sistemas de software a fim de resolver problemas complexos.

12. Esperança não é uma estratégia

Por design, é fundamental que as equipes de SRE estejam focadas em engenharia. Sem uma engenharia constante, a carga das operações aumenta e as equipes precisarão de mais pessoas somente para acompanhar esse aumento da carga de trabalho.

Em algum momento no futuro, um grupo tradicional focado em operações escalará linearmente conforme o volume do serviço: Se os produtos aos quais o serviço dá suporte forem bem sucedidos, a carga operacional aumentará com o tráfego. Isso significa contratar mais pessoas para fazer as mesmas tarefas repetidamente.

Para evitar esse destino, a equipe responsável pelo gerenciamento de um serviço deve escrever código, do contrário ficará sobrecarregada. Desse modo, o Google coloca um limite de 50% no trabalho agregado de ops para todos os SREs. tickets, plantão, tarefas manuais, etc. Esse limite garante que a equipe de SRE tenha emprego suficiente em seus cronogramas para deixar o serviço estável e operacional.

A regra geral é que uma equipe de SRE deve gastar os outros 50% de seu tempo fazendo desenvolvimento.

# Ações

O SRE nos da um bom framework de como implementar devops, claro que implementar Devops em uma empresa é uma tarefa díficl, por isso eu acho que 
pequenas ações, apoiadas neste framework pode ser um bom ponto de partida.

Confiabilidade - Pense desde o princípio em construir sistemas com alto nível de confiabilidade

Resolver Problemas - Dificilmente você verá um SRE dizendo que o "Problema não é dele"

Automatização - Com automatização ganhamos tempo para a principal atividade, ao meu ver.

A regra geral é que uma equipe de SRE deve gastar os outros 50% de seu tempo fazendo desenvolvimento.

Sei que nesse ponto você deve estar se perguntando "Quando não estou em reunião estou atendendo chamado". É fato que grande parte
de nós, sysadmins, devops e correlatos passamos grande parte do tempo realizando o que o SRE chama de tarefas penosas

13. Tarefas Penosas

Se um operador humano precisar tocar o sistema durante as operações normais, você tem um bug. A definição de “normal” muda na mesma medida em que seus sistemas evoluem

No SRE, queremos dedicar mais tempo ao trabalho de engenharia de projeto a longo prazo, em vez do mero trabalho operacional. Como o termo trabalho operacional pode ser mal interpretado, usamos uma palavra específica: toil (tarefas penosas)

# o que é

Toil é o tipo de trabalho vinculado à execução de um serviço de produção que tende a ser manual, repetitivo, automatizado, tático, desprovido de valor duradouro e que escala linearmente à medida que o serviço cresce.

Alguns tipos:

Manual

Isso inclui trabalhos como a execução manual de um script que automatiza algumas tarefas. Executar um script pode ser mais rápido do que executar manualmente cada etapa do mesmo, mas o tempo prático que um ser humano gasta executando esse script (não o tempo em si decorrido) ainda é um tempo de trabalho toil.

Repetitivo

Se você está realizando uma tarefa pela primeira vez, ou mesmo pela segunda vez, este trabalho não é toil. Toil é o trabalho que você faz continuamente. Se você está resolvendo um novo problema ou inventando uma nova solução, este trabalho não é toil.

Automatizável

Se uma máquina pode realizar a tarefa tão bem quanto um ser humano, ou a necessidade da tarefa pode ser projetada, então essa tarefa é um trabalho toil. Se o julgamento humano é essencial para a tarefa, há uma boa chance de não ser um toil.

Sem valor duradouro

Se o seu serviço permanecer no mesmo estado depois de concluir uma tarefa, provavelmente a tarefa foi toil. Se a tarefa produziu uma melhoria permanente em seu serviço, provavelmente não foi toil, mesmo se alguma quantidade de trabalho sujo – como cavar em códigos e configurações legados e corrigi-los – estiver envolvida.

# Resumo

Se todos nós nos comprometermos a eliminar um pouco de trabalho toil a cada semana com alguma boa Engenharia, iremos continuamente limpar nossos serviços e podemos mudar nossos esforços coletivos para a Engenharia em escala, arquitetando a próxima geração de serviços e construindo conjuntos de ferramentas SRE cruzadas. Em resumo, vamos inventar mais e trabalhar menos.

14. Devops ou SRE?

O termo "Devops" surgiu no mercado no final do ano de 2008 e seus principios essenciais - envolvimento da função de TI em cada fase do design e do desenvolvimento de um sistema, alta dependencia de automação em comparação com esforços humanos, aplicação de práticas e ferramentas de engenharia em tarefas de operação, são consistentes com muitas práticas e dos principios de SRE. Poderíamos ver o Devops como uma generalização de vários principios essencias de SRE para uma variedade maior de organizações, estruturas gerenciais e recursos humanos. Do mesmo modo, poderíamos ver a SRE como uma implementação especifica de Devops, com algumas extensões idiossincráticas.

15. Obrigado