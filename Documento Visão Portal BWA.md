**Engenharia de Requisitos \- Atividade Documento de Visão**  
**Componentes: Adna Oliveira Silva, [Italo Almeida Nascimento](mailto:nascimento.italo@escolar.ifrn.edu.br)**  
**Projeto:** Portal de Robotização Bwa  
**Descrição do problema:**

**O problema de:** Processos repetitivos que são feitos manualmente, tomando tempo dos colaboradores, que poderia ser aproveitado para o adiantamento de outras tarefas  
**Afeta:** Colaboradores da BWA Global  
**Impacto:** Os colaboradores teriam que realizar processos repetitivos, sem o acesso aos RPAs que podem realizar esse tipo de tarefa por eles.  
**Solução:** Criação de uma plataforma para os colaboradores da empresa terem acesso aos RPAs, poderem cadastrar as execuções dos robôs, visualizarem gráficos com informações dos robôs ativos, o andamento das execuções

**Descrição dos usuários**:

| Nome | Descrição | Responsabilidade |
| :---- | :---- | :---- |
| Visitante | Indivíduos não cadastrados no portal | Não pode fazer cadastro no portal, pois não é um colaborador da empresa |
| Colaborador | Individuos que possuem cadastro no portal | Tem seu login de acesso, pode visualizar os dados dos RPAs da empresa, visualizar a lista de clientes, cadastrar execuções, visualizar usuários cadastrados |
| Administradores/ Desenvolvedores | Individuo(s) que administra(m) o sistema | Gerencia as contas de usuários e clientes cadastrados, faz o gerenciamento dos robôs e das execuções, dar suporte aos usuários se houverem chamados |

**Principais necessidades dos usuários:**

- Realizar os processos de forma rápida e eficiente  
- Facilidade na utilização do portal  
- Qualidade do serviço  
- Suporte

**Requisitos FUNCIONAIS:**

| Código | Nome | Descrição |
| :---- | :---- | :---- |
| **RF01** | Gerenciar robôs | Permite aos administradores acesso completo a lista de robôs cadastrados no portal, podendo adicionar e remover robôs |
| **RF02** | Gerenciar usuários | Permite aos administradores acesso completo a lista de usuários cadastrados no portal, podendo adicionar e remover usuários |
| **RF03** | Gerenciar clientes | Permite aos administradores acesso completo a lista de clientes cadastrados no portal, podendo adicionar e remover clientes |
| **RF04** | Gerenciar execuções | Permite aos administradores terem acesso completo às execuções cadastradas, podendo até indisponibilizar ou excluir execuções |
| **RF05** | Apresentar dados das execuções | Permite ao colaborador visualizar os painéis de dados dos robôs e das execuções realizadas e em andamento |
| **RF06** | Chat com inteligência artificial voltado para informações contábeis | Permite ao colaborador trocar mensagens com um chat integrado a uma API de inteligência artificial |
| **RF07** | Adicionar execuções | Permite ao colaborador adicionar novas execuções em qualquer RPA que esteja disponível |
| **RF08** | Listar usuários | Permite ao colaborador visualizar todos os colaboradores cadastrados no portal |
| **RF09** | Listar clientes | Permite ao colaborador visualizar todos os clientes cadastrados no portal |

**Requisitos NÃO-FUNCIONAIS:**

| Código | Nome | Descrição | Categoria | Classificação |
| :---- | :---- | :---- | :---- | :---- |
| NF01 | Design responsivo | O sistema deve se adaptar a qualquer tipo de dispositivo | Usabilidade | Obrigatório |
| NF02 | Usabilidade eficiente | O sistema deve possuir uma interface apropriada, que facilite a interação com os usuários | Usabilidade | Obrigatório |

