Atividade: AWS Elastic Beanstalk
Visão geral do laboratório
Esta atividade disponibiliza para você uma conta da Amazon Web Services (AWS) com um ambiente do AWS Elastic Beanstalk pré-criado. Você implantará um código nela e observará os recursos da AWS que compõem o ambiente do Elastic Beanstalk.

 

Duração
A atividade levará aproximadamente 30 minutos para ser concluída.

 

Restrições de serviço da AWS
Neste ambiente de laboratório, o acesso aos serviços e às ações de serviços da AWS pode ser restrito aos necessários para concluir as instruções do laboratório. Você poderá encontrar erros se tentar acessar outros serviços ou executar ações além das descritas neste laboratório.

 

Acessar o Console de Gerenciamento da AWS
No topo destas instruções, escolha  Iniciar laboratório.

A sessão de laboratório será iniciada.

Um cronômetro ficará visível no topo da página e mostrará o tempo restante da sessão.

 Dica: para atualizar a duração da sessão a qualquer momento, selecione  Iniciar laboratório novamente antes que o cronômetro seja zerado.

Antes de continuar, aguarde até o ícone circular à direita do link da AWS  no canto superior esquerdo ficar verde. 

 

Para se conectar ao Console de Gerenciamento da AWS, escolha o link da AWS no canto superior esquerdo.

Uma nova guia do navegador será aberta, e você acessará o console.

 Dica: se uma nova guia não for aberta, você verá um banner ou um ícone no topo do navegador com uma mensagem informando que o programa está impedindo que o site abra janelas pop-up. Selecione o banner ou ícone e escolha Permitir pop-ups.

 

Organize a guia do Console de Gerenciamento da AWS para que ela seja exibida com essas instruções. O ideal seria você poder visualizar as duas guias do navegador ao mesmo tempo para facilitar o acompanhamento das etapas do laboratório.

 

Como obter crédito para seu trabalho
Ao final deste laboratório, você receberá instruções de como enviar o laboratório para receber uma pontuação com base em seu progresso.

 Dica: o script que verifica seu trabalho só pode conceder pontos se você nomear recursos e definir as configurações conforme especificado. Em particular, os valores nessas instruções que aparecem This Format devem ser inseridos exatamente como documentado (diferenciando letras maiúsculas de minúsculas).

 

Tarefa 1: Acessar o ambiente do Elastic Beanstalk
No console, na caixa de pesquisa à direita de  *Serviços*, procure e selecione *Elastic Beanstalk*. 

Uma página intitulada Ambientes deve ser aberta com uma tabela que lista os detalhes de uma aplicação existente do Elastic Beanstalk.  

Observação: se o status na coluna Integridade não for OK, significa que a inicialização ainda não acabou. Aguarde alguns instantes, e ela deverá mudar para Ok.

elastic-beanstalk-app

 

Na coluna Nome do ambiente, selecione o nome do ambiente.

A página Painel do ambiente do Elastic Beanstalk é aberta.

 

Observe que a página mostra que a integridade do seu aplicativo está Ok.

O ambiente do Elastic Beanstalk está pronto para hospedar um aplicativo. No entanto, ele ainda não tem código em execução.

 

Testar o acesso ao ambiente.

Próximo ao topo da página, selecione o link do domínio (a URL termina com elasticbeanstalk.com).

Quando você selecionar a URL, uma nova guia do navegador será aberta. No entanto, você deve observar que ela exibe a mensagem HTTP Status 404 - Not Found (HTTP Status 404 - Não encontrado). 

Esse comportamento é esperado, porque esse servidor de aplicações ainda não tem nenhuma aplicação em execução. 

Retorne ao console do Elastic Beanstalk.

Na próxima etapa, você implantará o código em seu ambiente do Elastic Beanstalk.

 

Tarefa 2: Implantar um aplicativo de exemplo no Elastic Beanstalk
Para baixar um aplicativo de amostra, selecione este link:
https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/samples/tomcat.zip

 

Retorne ao painel do Elastic Beanstalk e selecione Fazer upload e implantar.

 

Selecione Escolher arquivo, navegue até o arquivo tomcat.zip que você acabou de baixar e abra-o.

 

Escolha Implantar.

Levará um ou dois minutos para o Elastic Beanstalk atualizar seu ambiente e implantar o aplicativo.

 

Após a conclusão da implantação, selecione o link da URL do domínio (ou, se a guia do navegador que exibia o status 404 ainda estiver aberta, atualize essa página).

O aplicativo web que você implantou é exibido.

web-app

Parabéns! Você implantou com sucesso um aplicativo no Elastic Beanstalk.

 

Retorne ao console do Elastic Beanstalk e selecione Configuração no painel esquerdo.

Observe os detalhes aqui.

Por exemplo, no painel Tráfego e escalabilidade da instância, ele indica os grupos de segurança do EC2, as instâncias mínimas e máximas e os detalhes do tipo de instância das instâncias do Amazon Elastic Compute Cloud (Amazon EC2) que hospedam o aplicativo web.

 

Não há exibição de detalhes de configuração no painel Redes, bancos de dados e etiquetas porque o ambiente não inclui um banco de dados.

 

Na linha Redes, bancos de dados e etiquetas, selecione Editar.

Observe que, se desejado, você pode ativar facilmente um banco de dados a esse ambiente; basta definir algumas configurações básicas e selecionar Aplicar. (No entanto, para a finalidade desta atividade, você não precisa adicionar um banco de dados.)

Selecione Cancelar na parte inferior da tela.
 

No painel esquerdo, em Ambiente, selecione Monitoramento.

Navegue pelos gráficos para ver os tipos de informações disponíveis para você.

 

Tarefa 3: Explorar os recursos da AWS que oferecem suporte ao seu aplicativo
No console, na caixa de pesquisa à direita de  *Serviços*, procure e selecione EC2.

 

Selecione Instâncias.

Observe que duas instâncias compatíveis com o aplicativo web estão em execução (ambas contêm samp em seus nomes). 

 

Você pode continuar explorando os recursos de serviço do Amazon EC2 criados pelo Elastic Beanstalk como desejar. Você encontrará:

Um grupo de segurança com a porta 80 aberta
Um balanceador de carga ao qual as duas instâncias pertencem
Um grupo do Auto Scaling que executa de duas a seis instâncias, dependendo da carga da rede
 O Elastic Beanstalk que criou esses recursos, mas você ainda tem acesso a eles.