<Nome do Projeto>
=================
Plano de Gerenciamento de Configuração
======================================
Versão &lt;1.0&gt;
------------------

_[Observação: O template a seguir é fornecido para uso com o Rational Unified Process (RUP).  O texto exibido entre colchetes e em itálico foi incluído para orientar o autor e deve ser excluído antes da publicação do documento._

_Este documento utiliza a formatação da linguagem [Markdown] (http://daringfireball.net/projects/markdown/). Você pode encontrar um guia de referência rápido [aqui] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).]_

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|_&lt;09/12/2014&gt;_|_&lt;1.0&gt;_|_&lt;Versão inicial&gt;_|_&lt;Simone Magalhaes&gt;_|
|_&lt;dd/mm/aaaa&gt;_|_&lt;1.1&gt;_|_&lt;Outra versão&gt;_  |_&lt;autor&gt;_|



1. Introdução
==============

_[A introdução do Plano de Gerenciamento de Configuração  oferece uma visão geral de todo o documento. 
Ela inclui a finalidade, o escopo, as definições, os acrônimos, as abreviações, as referências e uma visão geral deste
Plano de Gerenciamento de Configuração.]_

1.1 Finalidade
---------------
Este Plano de Gerenciamento de Configuração visa definir como, quando e onde deverá ser feita a gestão de configuração e mudança do Projeto Livraria.

1.2 Escopo
----------
_[Uma breve descrição do escopo deste Plano de Gerenciamento de Configuração; o modelo ao qual ele está associado e tudo o que é afetado ou influenciado por este documento.]_

1.3 Definições, Acrônimos e Abreviações
---------------------------------------
_[Esta subseção apresenta as definições de todos os termos, acrônimos e abreviações necessários para a correta interpretação do Plano de Gerenciamento de Configuração.  Essas informações podem ser fornecidas mediante referência ao Glossário do projeto.]_

1.4 Referências
---------------
_[Esta subseção apresenta uma lista completa de todos os documentos mencionados no Plano de Gerenciamento de Configuração. Identifique os documentos por título, número de relatório (se aplicável), data e organização responsável pela publicação. Especifique as fontes a partir das quais as referências podem ser obtidas. Essas informações podem ser fornecidas por um anexo ou outro documento.]_

1.5 Visão Geral
---------------
_[Esta subseção descreve o conteúdo restante do Plano de Gerenciamento de Configuração e explica como o documento está organizado.]_



2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------
Responsável pela execução das diversas atividades de Gerenciamento de Configuração (CM) descritas no Processo de CM: Aline, Simone, Jacqueline

2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------
_[Descreva o ambiente de computação e as ferramentas de software a serem utilizadas para desempenhar as funções de CM em todo o ciclo de vida do projeto ou produto.]_
Ferramentas e os procedimentos necessários utilizados para o controle de versão dos itens de configuração gerados no ciclo de vida do projeto ou produto: Controle de versão:  GIT; Gestão de mudanças: Mantis.
_[As questões envolvidas na configuração do ambiente de CM incluem:_
* _tamanho previsto dos dados do produto_
* _distribuição da equipe do produto_
* _localização física dos servidores e clientes]_
 


3. O Programa de Gerenciamento de Configuração
==============================================

3.1 Identificação da Configuração
---------------------------------
### 3.1.1 Métodos de Identificação
----------------------------------
_[Descreva como os artefatos do projeto ou produto devem ser nomeados, marcados e numerados. O esquema de identificação deve abranger o hardware, o software do sistema, os produtos de terceiros (COTS) e todos os artefatos de desenvolvimento de aplicativos listados na estrutura de diretórios do produto; por exemplo, planos, modelos, componentes, software de teste, resultados e dados, executáveis e assim por diante.]_

### 3.1.2 Itens de Configuração
_[Relacionar os artefatos ou grupos de artefatos, separando por tipo, modulo ou subsistema, responsável ou momento em que deverão ser incluídos em baselines._
* _“Inclusão em Baseline” em branco significa que o grupo de artefatos não participará de baseline. Pode ser expresso como uma data ou identificador de uma baseline, fase ou ponto de controle_
* _“Responsável”: indicar nominalmente, sempre que possível]_

| Item (ou Tipo de Item)                           | Responsável na equipe	     | Inclusão em Baseline |
|--------------------------------------------------|----------------------------|----------------------|
|_&lt;Artefatos:Regras de Negócio, casos;_ 
_&lt;de uso, diagramas de análise e projeto,;_
_&lt;mensagens, regras de validadção, requisitos,;_
_&lt;casos de teste, plano de projeto, cronograma&gt;_|_&lt;Simone&gt;_|_&lt;baselineartef1.0122014&gt;_|
                                         
|_&lt;Código-fonte&gt;_                            |_&lt;Jacqueline&gt;_        |_&lt;baselinecodigo1.0122014&gt;_|

### 3.1.3 Baselines do Projeto

_[As baselines funcionam como um padrão oficial no qual os trabalhos subseqüentes são baseados. Somente mudanças autorizadas podem ser efetuadas nas baselines._
_Descreva em que pontos do ciclo de vida do projeto ou produto as baselines devem ser estabelecidas. As baselines mais comuns devem ser definidas ao final de cada uma das fases de Iniciação, Elaboração, Construção e Transição. Elas também podem ser geradas no final de iterações ocorridas dentro das várias fases ou com freqüência ainda maior._
_Descreva quem autoriza uma baseline e o que ela contém.]_
baseline_artefVERSAOMESANO - Regras de Negócio, casos de uso, diagramas de análise e projeto, mensagens, regras de validação, requisitos, casos de teste, plano de projeto, cronograma - Autorizado pelo Gestor do Projeto
baseline_codigoVERSAOMESANO - Código-fonte - Autorizado pelo Gestor do Projeto

### 3.1.4 Estrutura do Repositório de Versões
_[Descreva a organização de diretórios do seu repositório e que itens/arquivos devem ser armazenados em cada diretório.]_
Artefatos > Especificação > Requisitos; Regras de Negócio; Casos de uso; Mensagens; Regras de Validação;
Artefatos > Especificação > Teste > Casos de teste
Artefatos > Análise e Projeto > Diagramas de Análise e Projeto (Classe, Sequencia..);
Artefatos > Projeto > Plano de projeto; Cronograma.
Código Fonte > Arquivos do sistema (dll, fontes...)

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança
_[Descreva o processo pelo qual os problemas e as mudanças são submetidos, revisados e dispostos. Inclua como funciona a transição de estados de uma solicitação de mudança]_
Ciclo de vida de uma solicitação de mudança: Novo, Atribuído, Em desenvolvimento, resolvido, Testado, Fechado, re-aberto.
Estrutura do CCB do seu projeto: ??


### 3.2.2 Comitê de Controle de Mudança (CCB)
_[Descreva a participação e os procedimentos para processar solicitações e aprovações de mudança a serem seguidos pelo CCB. Informe quem são os membros do CCB e suas responsabilidades.]_
Integrantes: Aline, Simone, Jacqueline


4. Padrões e Procedimentos
==========================
_[Descreva os padrões e procedimentos que devem ser seguidos no projeto. Crie subseções se achar necessário, para organizá-los melhor.]_
Quando será obrigatório criar: Manutenção de uma versão em produção x trabalho na nova
versão, Atividade impactante e demorada, Customizações para diferentes.
clientes ou ambientes
Padrão para o nome do branch: nomefuncionalidade.0000
Quem é responsável por criar: GC - Aline
Quando e por quem o merge deve ser feito - a cada nova entrega ou versão - GC


5. Treinamento e Recursos
=========================
_[Descreva as ferramentas de software, o pessoal e o treinamento necessários para implementar as atividades de CM especificadas.]_
Ferramentas: GIT, Mantis


6. Auditorias de Configuração
=============================
_[Descreva o cronograma das auditorias de configuração e o que será verificado. Informe também como serão reportados os problemas encontrados e onde sera feito o acompanhamento dos itens corretivos.]_
