<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+12"><center>
**Escola Infinito**
</center></font>

>*Observação 1: A estrutura inicial deste documento é só um exemplo. O seu grupo deverá alterar esta estrutura de acordo com o que está sendo solicitado na disciplina.*

**Conteúdo**

- [Autores](#autores)
- [Descrição do projeto](#descrição-do-projeto)
- [Análise de requisitos funcionais e não-funcionais](#análise-de-requisitos-funcionais-e-não-funcionais)
- [Diagrama de casos de uso](#diagrama-de-casos-de-uso)
- [Descrição dos casos de uso](#descrição-dos-casos-de-uso)
  - [Registrar falta](#registrar-falta)
  - [Relatório de Faltas](#relatório-de-faltas)
  - [Notificaçoes](#notificaçoes)
  - [Acessibilidade](#acessibilidade)
- [Diagrama de sequencia](#diagrama-de-sequencia)
- [Diagrama de classes](#diagrama-de-classes)
- [Diagrama de Componentes](#diagrama-de-componentes)
- [Decisões de arquitetura](#decisões-de-arquitetura)
- [Diagrama de implantação](#diagrama-de-implantação)
- [Referências](#referências)


# Autores

* Pablo Borba Leal


# Descrição do projeto

*Estou prestes a desenvolver um sistema, com o objetivo principal de monitorar e gerenciar a presença dos alunos, abrangendo desde a primeira até a quinta série de uma respeitável instituição de ensino. O desafio que se apresenta diante de nós é verdadeiramente significativo, pois a administração da frequência escolar é um pilar fundamental para a qualidade do ensino e o bem-estar dos estudantes.*

# Análise de requisitos funcionais e não-funcionais
**Requisitos Funcionais:**

1. Registro de Faltas Intuitivo:
O sistema deverá permitir que os professores registrem as faltas dos alunos de forma simples e intuitiva. Isso garantirá que o processo de controle de presença seja eficiente e eficaz, facilitando a vida dos educadores.

2. Geração de Relatórios Detalhados:
Uma das funcionalidades-chave será a capacidade do sistema de gerar relatórios abrangentes de faltas. Esses relatórios deverão possibilitar o agrupamento das informações por data, ano do ensino, turma, professor, disciplina e aluno. Isso fornecerá uma visão clara e estruturada dos dados de presença, auxiliando a escola na tomada de decisões informadas.

3. Análise Facilitada de Faltas:
O sistema deverá ser projetado de maneira a facilitar a análise e o acompanhamento do número de faltas. Os gestores e professores poderão acessar informações de presença de forma rápida e eficaz, ajudando-os a identificar tendências e tomar medidas preventivas quando necessário.

4. Notificações por E-mail Automáticas:
Quando a porcentagem de comparecimento às aulas de um aluno estiver abaixo de 80%, o sistema deverá enviar notificações por e-mail aos pais ou responsáveis. Essas notificações automáticas manterão os responsáveis informados sobre a frequência de seus filhos, incentivando uma participação ativa na educação.

**Requisitos não-funcionais:**

1. Tecnologias de Desenvolvimento:
O sistema será implementado utilizando as linguagens HTML, CSS e JS, garantindo uma interface amigável e responsiva.

2. Integração com Banco de Dados:
Será essencial que o sistema seja interligado a um banco de dados confiável para armazenar e gerenciar as informações de presença dos alunos.

3. Acessibilidade Múltipla:
O sistema deverá ser funcional tanto na web quanto em dispositivos móveis, garantindo que professores e gestores possam acessá-lo de qualquer lugar e a qualquer momento, tornando-o altamente acessível.

4. Capacidade de Suporte a Acessos Simultâneos:
O sistema deverá ser robusto o suficiente para suportar vários acessos simultâneos, garantindo que todos os usuários possam utilizá-lo sem problemas, mesmo em horários de pico.

5. Senhas Seguras:
Para garantir a segurança dos dados, os usuários serão obrigados a escolher senhas fortes, com no mínimo 6 dígitos, pelo menos 1 caractere especial e pelo menos 1 letra maiúscula. Isso ajudará a proteger as informações sensíveis armazenadas no sistema e a manter a integridade dos dados dos alunos.

# Diagrama de casos de uso

![alt](img/SistemaDePresença.png)

# Descrição dos casos de uso

## Registrar falta

Ator: Professores

Descrição: O professor registra a falta do mesmo aluno em dois horários diferentes durante o dia.

Fluxo básico:

- O professor utiliza "Registrar Falta".
- O sistema exibe a lista de turmas e alunos.
- O professor escolhe a turma e identifica o aluno ausente.
- O professor registra a ausência do aluno na data presente.
- O sistema armazena a informação da falta registrada.
  
## Relatório de Faltas

Ator: Professores

Descrição: Produz um relatório contendo informações consolidadas sobre as ausências.

Fluxo básico:

- O usuário utiliza a funcionalidade "Gerar Relatório de Faltas".
- O sistema disponibiliza funcionalidades de busca, incluindo opções como aluno, turma, data, disciplina e professor, visando facilitar o acesso às informações de falta.
- O usuário escolhe os filtros desejados.
- O sistema cria o relatório de acordo com os filtros selecionados.
- O usuário examina o relatório de ausências produzido.
- O usuário verifica a porcentagem de faltas.
  
## Notificaçoes

Ator: Responsaveis

Descrição: Envia uma notificação por e-mail aos pais/responsáveis informando sobre a situação de faltas do aluno.

Fluxo básico:

- O sistema realiza a verificação diária do percentual de faltas de cada aluno.
- O sistema, automaticamente, ativa o caso de uso "Enviar Notificação" para os alunos que possuem um percentual de faltas abaixo do limite definido.
- O sistema coleta os dados de e-mail dos pais/responsáveis.
- O sistema encaminha a notificação por e-mail.

## Acessibilidade

Ator: Sistema

Descrição: Permite a configuração das opções de acessibilidade e outras configurações do sistema.

Fluxo básico:

- O administrador entra na tela de configurações do sistema.
- O administrador modifica as configurações de fonte, contraste, notificações e outras opções, tanto na versão web quanto na versão mobile do sistema.
- O sistema armazena as configurações que foram aplicadas.
- O sistema possibilita a modificação do registro de faltas.

# Diagrama de sequencia

*&lt;Diagrama de ordem e interação dos objetos&gt;*

# Diagrama de classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

# Diagrama de Componentes

*&lt;Diagrama para exibir a relação estrutural dos componentes de um sistema de software

# Decisões de arquitetura

*&lt;Descrever a infraestrutura escolhida para arquitetura do projeto&gt;*

# Diagrama de implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

# Referências

*&lt;Lista de referências&gt;*
