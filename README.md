# Sistema integrado para a gestão de chamados e suporte técnico baseado em IA - PIM 
O Projeto consiste no desenvolvimento de um sistema help desk que organize as chamadas e as auxilie inicialmente através de sugestões por IA.

## Requisitos
Os Requisitos estão divididos entre funcionais e não funcionais, onde os mesmos representam as funcionalidades do sistema.
### Requisitos Funcionais
1. Cadastrar Usuário

    1.1 - **Histórias de Usuário** - Cadastro de Clientes:

    Como ADM, quero ser o único a cadastrar clientes no sistema.

    - Deve criar a funcionalidade cadastro de clientes.
    - Restringi-la somente ao ADM do sistema.
    - Validar dados, (E-mail, nome, senha).
    - Exibir mensagem de erro ou sucesso.

    1.2 **Histórias de Usuário**: - Alterar Senha.

    Como ADM, quero poder alterar a senha do usuário quando solicitado, garantindo o controle de acesso ao sistema.

    - Criar funcionalidade para a alteração de senha.
    - Validar dados da nova senha.
    - Exibir mensagem de erro ou sucesso.

2. Login

    2.1 - **Histórias de Usuário**: - Login.

    Como Usuário, quero logar no sistema para fazer o uso das funcionalidades.

    - Criar o sistema de Login.
    - Validar dados de cadastro, (E-mail, nome, senha).
    - Exibir mensagem de erro ou sucesso.

3. CRUD de Chamados.

    3.1 - **Histórias de Usuário** - Criar Chamado

    Como usuário quero utilizar o sistema para abrir um novo chamado e solicitar suporte.

    - Criar o sistema de Novo chamado.
    - Permitir que o usuário infome sobre o chamado. (Título, descrição do problema, categoria e prioridade).
    - Exibir mensagem de erro ou sucesso ao criar o chamado.

    3.2 **Histórias de Usuário** - Vizualizar Chamado

    Como usuário, quero vizualizar o chamado recém criado, ou chamados antigos em espera para consultar o andamento.

    - Permitir a visualização dos chamados disponiveís.
    - Permitir a visualização das especificações dos chamados.
    - Exibir status do chamado (Aberto, Em andamento, Fechado).

    3.3 **Histórias de Usuário** - Editar Chamado

    Como usuário, quero poder editar os chamados criados, permitindo incluir ou excluir especificações, facilitando a resolução.

    - Permitir a edição das especificações a partir da vizualização do chamado.
    - Salvar os dados alterados
    - Exibir mensagem de erro ou sucesso.

    3.4 **Histórias de Usuário** - Excluir Chamado.

    Como ADM, quero excluir chamados fechados, garantindo a organização do trabalho.

    - Criar a funcionalidade de exclusão.
    - Validar dados do Administrador.
    - Restringir funcionalidade somente ao ADM.
    - Exibir mensagem de erro ou sucesso.


4. Filtragem e Resolução de Chamados por IA.

    4.1 **Histórias de Usuário** - Filtragem de Chamados.

    Como IA, quero analisar os chamados automáticamente, identificando o problema e sua categoria.

    - Criar um mecanismo de IA para analisar os chamados.
    - Receber o feedback da IA após a filtragem com as especifiações do problema.
    - Exibir mensagem indicando que ela resolverá ou se será necessário acionar um técnico.

    4.2 **Histórias de Usuário** - Resolução por IA.

    Como usuário, quero receber a resolução do problema solicitado após a filtragem e análise do mesmo, diminuindo o tempo de espera.

    - Criar a funcionalidade para a IA dar sugestões automáticas. 
    - Validar as soluções antes de encerrar o chamado.
    - Caso a solução não resolver, encaminhar ao técnico especialista.

5. Resolução por Técnico.

    5.1 **Histórias de Usuário** - Encaminhamento de chamados

    Como sistema, quero enchaminhar chamados aos técnicos quando a IA não resolve-los.

    - Criar a funcionalidade de acionar técnico.
    - Enviar uma notificação ao técnico contendo o problema e suas especificações.
    - Alterar o status do chamado ao usuário para "Aguardando Técnico".

    5.2 **Histórias de Usuário** - Resolução por Técnico

    Como técnico, quero analisar os chamados encaminhados para análisa-los e devolver uma solução.

    - Criar interface para os técnicos vizualizarem os chamados.
    - Verificar e validar dados de acesso do técnico.
    - Permitir que o técnico registre a solução.
    - Exibir mensagem de erro ou sucesso.

### Requisitos não funcionais
    - Compatibilidade com SQL Server.
    - Integração com IA.
    - Segurança dos dados
        - Máscara na senha.

    
Diagrama de Caso de Uso
![Diagrama de Caso de Uso](https://github.com/PedroRSouza0/PIM3/blob/main/DiagramaProjeto.asta)

