MODULO 1:

Existem três modelos principais de serviços em nuvem. Cada modelo representa uma parte diferente da pilha de computação em nuvem e oferece um nível diferente de controle sobre seus recursos de TI:
•Infraestrutura como serviço (IaaS): os serviços nesta categoria são os componentes básicos da TI em nuvem e, geralmente, fornecem acesso (virtual ou no hardware dedicado) a recursos de rede e computadores, bem como espaço para o armazenamento de dados. A IaaS oferece o mais alto nível de flexibilidade e controle de gerenciamento sobre seus recursos de TI. É o modelo mais semelhante aos recursos de TI existentes com os quais muitos departamentos e desenvolvedores de TI já estão familiarizados.
•Plataforma como serviço (PaaS): os serviços nessa categoria reduzem a necessidade de gerenciar a infraestrutura subjacente (geralmente hardware e sistemas operacionais) e permitem que você se concentre na implantação e no gerenciamento de seus aplicativos.
•Software como serviço (SaaS): os serviços nesta categoria fornecem um produto completo que o provedor de serviços executa e gerencia. Na maioria dos casos, o software como serviçorefere-se a aplicativos de usuário final. Com uma oferta de SaaS, não é necessário pensar na manutenção do serviço ou no gerenciamento da infraestrutura subjacente. 
É necessário pensar apenasem como você planeja usar esse software específico. Um exemplo comum de aplicação do SaaS é o webmail, no qual você pode enviar e receber e-mails sem precisar gerenciar recursos adicionais para o produto de e-mail nem manteros servidores e sistemas operacionais no qual o programa de e-mail está sendo executado.

principais lições da seção 1
Algumas das principais lições desta seção do módulo são:•O termo “computação em nuvem” se refere à entrega de recursos de TI sob demanda por meio da Internet, com pagamento conforme o uso.
•A computação em nuvem permite pensar em sua infraestrutura (e usá-la) como software.•Existem três modelos de serviços em nuvem: IaaS, PaaS e SaaS.•Existem três modelos de implantação em nuvem: nuvem, híbrida e no local (ou nuvem privada).
•Existem muitos serviços parecidos com os da AWS para o espaço de TI tradicional, no local.© 2022, Amazon Web Services, Inc. ou sua safiliadas. Todos os  direitos reservados.
13 Principais lições da Seção 1
•O termo“computaçãoemnuvem” se refereà entregade recursosde TI sob demanda pormeioda Internet, com pagamento conformeo uso.
•A computação em nuvem permite
pensar em sua infraestrutura(e usá-la) como software.•Existem três modelos de serviços em nuvem: IaaS, PaaS e SaaS. 
•Existem três modelos de implantação em nuvem: nuvem, híbridae no local (ou nuvem privada).•Praticamente tudoo que você pode implementar com a TI tradicional também pode implementar como um serviço de computação em nuvem da AWS

Seção 1: Introdução à computação em nuvem 

Vantagem 1 –Troque despesas de capital por despesas variáveis: as despesas de capital (capex)são os fundos que uma empresa usa para adquirir, atualizar e manter ativos físicos, como propriedades, edifícios industriais ou equipamentos. Você se lembra do exemplo de datacenter no modelo de computação tradicional em que era necessário colocar em rack e empilhar o hardware e, em seguida, gerenciar tudo isso? É necessário pagar por tudo no datacenter, e não importa se você não tiver usado tudo.Por outro lado, uma despesa variávelé aquela que pode ser alterada ou evitada facilmente. Em vez de investir substancialmente em datacenters e servidores antes de saber como eles serão usados, você pode pagar somente quando consome recursos e somente pela quantidade consumida. Assim,você economiza dinheiro em tecnologia. A computação em nuvem também permite que você se adapte a novos aplicativos com o espaço necessário em minutos, em vez de semanas ou dias. A manutenção é reduzida, o que permite que você se concentre mais nos principais objetivos da sua empresa.

Vantagem 2 –Beneficie-se da grande economia de escala: o uso da computação em nuvem permite obter um custo variável inferior ao de ambientes locais. Considerando que o uso de centenas de milhares de clientes é agregado na nuvem, provedores como a AWS conseguem obter economias de escala maiores, resultando em preços mais baixos com pagamento conforme o uso.

Principais lições da Seção 2:

As principais lições desta seção do módulo incluem as seis vantagens da computação em nuvem:
•Troque despesas de capital por despesas variáveis
•Grande economia de escala
•Pare de tentar adivinhar a capacidade•Aumente a velocidade e a agilidade
•Pare de gastar dinheiro com a operação e manutenção de datacenters•Tenha alcance global em minutos

Seção 3: Introdução à AmazonWeb Services (AWS)

O que são serviços web?
Um serviço web é qualquer software disponibilizado pela Internet que usa um formato padronizado, como Extensible Markup Language(XML) ou JavaScrip tObject Notation(JSON), para a solicitação e resposta de uma interação de Application Programming Interface (API).

Em geral, um serviço web é qualquer software disponibilizado pela Internet ou em redes privadas (intranet). Um serviço web usa um formato padronizado, como Extensible Markup Language (XML) ou JavaScript Object Notation(JSON), para a solicitação e a resposta de uma interação de interface de programação de aplicativos (API). Ele não está vinculado a nenhum sistema operacional ou linguagem de programação. Ele é autodescritivo por meio de um arquivo de definição de interface e é detectável.

Exemplode solução simples :
#Redes
#Computação
#Banco de dados
#Armazenamento
#Usuário
#Nuvem AWS
#Virtual Private Cloud (VPC)
#Amazon DynamoDB
#amazon EC2
#Amazon S3

Por exemplo, digamos que você esteja criando um aplicativo de banco de dados. Seus clientes podem estar enviando dados para suas instâncias do Amazon Elastic Compute Cloud (AmazonEC2), que é um serviço na categoria de computação. Esses servidores EC2 agrupam os dados em lotes em incrementos de um minuto e adicionam um objeto por cliente ao Amazon Simple Storage Service (AmazonS3), o serviço de armazenamento da AWS que você escolheu usar. Em seguida, você pode usar um banco de dados não relacional, como o Amazon DynamoDB, para potencializar seu aplicativo, por exemplo, para criar um índice que permita encontrar todos os objetos de determinado cliente que foram coletados durante determinado período. É possível executar esses serviços dentro de uma Amazon Virtual Private Cloud (AmazonVPC), que é um serviço na categoria de rede.

O objetivo deste exemplo simples é ilustrar a possibilidade de selecionar serviços web de diferentes categorias e usá-los juntos para criar uma solução (neste caso, um aplicativo de banco de dados). Naturalmente, as soluções criadas podem ser bastante complexas.

Três maneiras de interagir com a AWS:

# Console de Gerenciamento da AWS Interface gráfica fácil de usar

# Interface da linhade comando(CLI da AWS)Acessoa serviços por comando sou scripts específicos

# Kits de desenvolvimento de software (SDKs)Acesse serviços diretamentedo seu código(como Java, Python e outros) 

Principais lições da Seção 4 :

•A adoção da nuvem não é instantânea para a maioria das organizações, ela exige uma estratégia e alinhamento consciente em toda a organização.

•O AWS CAF foi criado para ajudar as organizações a desenvolver planos eficientes e eficazes para sua jornada de adoção da nuvem.

•Ele organiza orientações em seis áreas de foco, chamadas perspectivas.

•As perspectivas consistem em conjuntos de recursos
empresariais ou tecnológicos que são responsabilidade das principais partes interessadas.

