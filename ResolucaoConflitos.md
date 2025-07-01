Conflitos:

1- Se um colaborador tentar adicionar uma execução (RF07) a um robô que um administrador acabou de remover (RF01)? O sistema se torna inconsistente.

2 \- Um **cliente** (RF03) pode também ser um **usuário** do sistema para acompanhar suas execuções? (RF02)

3-  **Ponto de Vista 1 (Admin/Segurança \- RF03):** A lista de clientes é um ativo sensível e deve ser gerenciada com controle total por administradores.  
**Ponto de Vista 2 (Colaborador \- RF09):** Para realizar seu trabalho, o colaborador precisa de acesso fácil à informação dos clientes e quer visualizar todos eles.

4- O conflito é direto e fundamental: RF05, em sua forma literal, concede um acesso amplo e irrestrito ("visualizar os painéis de dados"), o que viola diretamente a regra de acesso restrito e seguro imposta por NF1

5- O colaborador (RF07) inicia um processo, enquanto o administrador (RF04) tem o poder de interromper ou apagar esse mesmo processo, possivelmente enquanto ele ainda está em andamento.

6- O conflito reside na ação de **"excluir"**. A capacidade de apagar permanentemente um registro de execução (RF04) pode violar diretamente as necessidades de auditoria e retenção de dados impostas por NF1.

Resolução com as técnicas do livro:

1-  Imposição : Para garantir que o histórico de execuções nunca seja corrompido por um robô deletado, a remoção física de robôs é proibida. A funcionalidade será alterada para 'desativar'.

2- Acordo: O acordo define a regra, por exemplo: "Um cliente pode ter um ou mais perfis de usuário associados". Esta regra é então usada para refinar os requisitos e eliminar o conflito. Além da mudança da nomenclatura.

3- Acordo: Chegar a uma solução que satisfaça plenamente os dois lados. Na discussão, pode-se descobrir que a necessidade real do colaborador não é ver "todos" os clientes, mas sim "todos os clientes do seu departamento".

4- Imposição: Requisitos não-funcionais como segurança, performance ou conformidade legal (LGPD, por exemplo) geralmente não são negociáveis. Eles são restrições impostas ao projeto por uma autoridade superior (a empresa, a lei, o cliente).

5- Votação: Administradores podem cancelar qualquer execução a qualquer momento. A exclusão de registros só será permitida para execuções finalizadas há mais de 90 dias. Esta é a política para equilibrar controle operacional e governança.

6- Acordo: A solução acordada é substituir a função `Excluir` por `Arquivar`. Uma execução arquivada desaparece das listas e painéis do dia a dia, mas continua existindo no banco de dados, acessível através de uma busca avançada ou em relatórios de auditoria.

