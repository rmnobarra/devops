## DevOps

<details>
<summary>O que é DevOps?</summary><br><b>

Antes de emitir qualquer opinião pessoal, é interessante observar o que as bigtech's dizem sobre devops:

Microsoft:

"DevOps é a união de pessoas, processos e produtos para permitir a entrega contínua de valor aos nossos usuários finais. A contração de" Dev "e" Ops "refere-se à substituição de Desenvolvimento e Operações em silos para criar equipes multidisciplinares que agora trabalham em conjunto com e práticas e ferramentas eficientes. As práticas essenciais de DevOps incluem planejamento ágil, integração contínua, entrega contínua e monitoramento de aplicativos. "

Red Hat:

"DevOps descreve abordagens para acelerar os processos pelos quais uma ideia (como um novo recurso de software, uma solicitação de aprimoramento ou uma correção de bug) vai do desenvolvimento à implantação em um ambiente de produção onde pode fornecer valor ao usuário. Essas abordagens exigem que as equipes de desenvolvimento e de operações se comuniquem com frequência e abordem seu trabalho com empatia por seus colegas de equipe. Escalabilidade e provisionamento flexível também são necessários. Com DevOps, aqueles que mais precisam de energia conseguem - por meio de autoatendimento e automação. Desenvolvedores, geralmente codificação em um ambiente de desenvolvimento padrão, trabalhe junto com as operações de TI para acelerar compilações, testes e lançamentos de software - sem sacrificar a confiabilidade. "

Google:

"... O movimento organizacional e cultural que visa aumentar a velocidade de entrega de software, melhorar a confiabilidade do serviço e construir propriedade compartilhada entre as partes interessadas do software"
</b></details>

<details>
<summary>Quais são os benefícios do DevOps? O que isso pode nos ajudar a alcançar?</summary><br><b>

* Colaboração
* Melhor entrega
* Segurança
* Velocidade
* Escala
* Confiabilidade
</b></details>

<details>
<summary>Como tudo começou?</summary><br><b>

* Manifesto ágil

Para falarmos sobre a história sobre DevOps, precisamos retroceder no tempo e falar sobre desenvolvimento e também sobre o manifesto ágil.
Em 2001, 17 desenvolvedores reuniram-se nas montanhas nevadas do estado norte-americano de Utah para discutir metodologias para processos de desenvolvimento e o resultado
deste encontro foi o então chamado manifesto ágil.

O Manifesto Ágil é uma declaração de valores e princípios essenciais para o desenvolvimento de software. 

Basicamente, o manifesto ágil  afirma que melhores resultados no desenvolvimento de software podem ser 
obtidos através da valorização de: 

  * Indivíduos e interações, mais que processos e ferramentas
  * Software em funcionamento, mais que documentação abrangente
  * Responder a mudanças, mais que seguir um plano

* Agile Conference

Em 2008 Andrew Schafer apresentou sua palestra de infraestrutura ágil para apenas uma pessoa, Patrick Debois. Guardem esses nomes. =)

* Velocity Conference

Em 2009, na Velocity Conference da O’Reilly, John Allspaw e Paul Hammond apresentaram “10+ Deploys per Day: Dev and Ops Cooperation at Flickr”.
Jogando luz a temas como

  * Interação entre os Desenvolvedores e a equipe de operações;
  * Como conseguir um aumento dos deploys com ferramentas e mudanças culturais.

Após lamentar no twitter sua não participação na palestra, Patrick Debois, recebeu a resposta do time do Flickr:

“Porque não organizar sua própria conferência de Velocity na Bélgica?”


* DevopsDays

Motivado pela palestra dos engenheiros da Flickr, Patrick Debois decidiu criar sua própria conferência na Bélgica, que ficou conhecida como DevOpsDays e foi um sucesso. Para lembrar
o dia, foi criada a tag #DevOps no Twitter, que posteriormente seria usado como o nome da cultura.
</b></details>

<details>
<summary>Pilares</summary><br><b>

C.A.M.S. ( Culture, Automation, Measure, Sharing)

C de Cultura
* Respeite a cultura.

Precisamos colaborar, compartilhar e entender a importância de manter uma relação saudável entre todas as áreas para que as equipes multidisciplinares possam trabalhar juntas e atingir os resultados.

A de Automação
* Automatize se possível

Quando falamos de DevOps, queremos eliminar o máximo de trabalho laboral possível, trabalho laboral é aquele trabalho repetitivo. Se você, por exemplo, gasta todo dia 30 minutos para efetuar uma determinada ação, porque não gastar um tempo superior, como, por exemplo, 2 horas para automatizar esta rotina e poupar esses 30 minutos a partir de então?

M de Medição
* Meça os resultados

Precisamos medir tudo que é possível: de processos a pessoas. Afinal, a única maneira de verificar se estamos no caminho certo ou melhorando é através da medição. O processo de melhoria contínua é o coração do DevOps!

S de Compartilhamento
Compartilhando feedbacks

Ambientes DevOps têm como uma das características fundamentais a cultura Blameless ou, em português, “Sem Culpa”, que é exatamente o que cria um ambiente propício ao compartilhamento. Não é sobre ninguém ser culpado por uma determinada ação que levou os sistemas a ficarem indisponíveis, é sobre todos se sentirem seguros e não terem medo de cometer erros. O erro faz parte do processo de aprendizado e deve ser compartilhado, assim como todas as melhorias que aplicamos em nosso ambiente de trabalho

</b></details>

<details>
<summary>Conhecimentos e tecnologias</summary><br><b>

![Devops roadmap](https://roadmap.sh/roadmaps/devops.png)

Fonte: https://roadmap.sh/devops

</b></details>

<details>
<summary>Lab</summary><br><b>

1. Crie um projeto no github

2. Add o Dockerfile

```Dockerfile
FROM debian:9.5-slim

ADD entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
```
3. crie o arquivo entrypoint.sh com o seguinte conteúdo

```bash
#!/bin/sh -l

sh -c "echo Hello world my name is $INPUT_MY_NAME"
```

</b></details>