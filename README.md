# DESAFIO QA - BEEDOO 2026

## 1. Introdução

Este repositório contém a documentação do desafio técnico para a vaga de **Analista de Qualidade de Software Júnior**.

O objetivo deste desafio foi analisar e testar o módulo de **cadastro e listagem de cursos** da aplicação disponibilizada, identificando possíveis falhas e documentando os testes realizados.

Durante o processo foram aplicados conceitos de **teste funcional, validação de campos, testes negativos e análise de comportamento do sistema**, com foco em identificar inconsistências que possam impactar a experiência do usuário ou a integridade dos dados.

---

# 2. Objetivo da aplicação

A aplicação tem como objetivo permitir que usuários realizem o **cadastro de cursos** e visualizem esses cursos em uma **lista organizada dentro do sistema**.



---

# 3. Fluxos principais identificados

Durante a exploração da aplicação foram identificados os seguintes fluxos principais:

### Cadastro de cursos
Permite inserir informações de um novo curso e salvá-lo no sistema.

### Listagem de cursos
Exibe os cursos cadastrados em uma lista para visualização.

### Exclusão de cursos
Possibilidade de excluir cursos diretamente da listagem.

---

# 4. Pontos críticos para testes

Os seguintes pontos foram considerados mais críticos durante a análise:

- Validação de campos obrigatórios
- Persistência das informações cadastradas
- Integridade da listagem de cursos
- Funcionamento da exclusão de cursos
- Prevenção de dados duplicados
- Consistência entre ações do usuário e resposta do sistema

Esses pontos são importantes para garantir que o sistema mantenha **dados confiáveis e uma boa experiência de uso**.

---

# 5. Estratégia de testes

A estratégia de testes foi baseada nos seguintes critérios:

- Teste do fluxo principal de cadastro
- Testes de listagem de cursos
- Validação de campos obrigatórios
- Testes de comportamento inesperado

Os cenários foram definidos buscando validar tanto o **comportamento esperado do sistema quanto possíveis falhas na aplicação**.

---

# 6. Casos de teste

Os cenários e casos de teste foram documentados na planilha abaixo:

📄 **Planilha de Casos de Teste**  
(https://docs.google.com/spreadsheets/d/1xN_uP8mhiWLJY21JGLwMoNO0lhey-zfy-i-Fq2dJH04/edit?gid=0#gid=0)

A planilha contém:

- Cenário
- Caso de teste
- Passos de execução
- Resultado esperado
- Resultado obtido
- Status do teste

---

# 7. Execução dos testes

Os testes foram executados manualmente na aplicação disponibilizada em https://creative-sherbet-a51eac.netlify.app/

Durante a execução foram registradas evidências de cada cenário testado.

 **Evidência dos testes**  

![tenor (2)](https://github.com/user-attachments/assets/c602136a-02e8-47e1-b150-c3d0e73694c0)

---

# 8. Bugs encontrados

Durante a execução dos testes foram identificados **4 bugs no sistema**.

Principais problemas encontrados:

- Sistema permite cadastro de curso sem nome
- Exclusão de cursos não remove item da listagem
- Sistema não possui opção de edição de cursos
- Sistema permite cadastro de cursos duplicados

---

# 9. Análise dos problemas encontrados

Os principais problemas identificados estão relacionados a:

- Falhas de validação de dados
- Inconsistência entre ação do usuário e resposta do sistema
- Falta de funcionalidades importantes para gerenciamento de cursos

Esses problemas podem impactar diretamente:

- Integridade das informações
- Experiência do usuário
- Confiabilidade do sistema

---

# 10. Melhorias sugeridas

Com base na análise realizada, algumas melhorias poderiam ser implementadas no sistema:

- Implementar validação obrigatória de campos
- Corrigir funcionalidade de exclusão de cursos
- Adicionar funcionalidade de edição de cursos
- Implementar controle de duplicidade de dados
- Melhorar mensagens de erro exibidas ao usuário

Essas melhorias contribuiriam para aumentar a **qualidade e confiabilidade da aplicação**.

---

# 11. Conclusão

O desafio permitiu realizar uma análise prática do sistema, identificando falhas importantes relacionadas à validação de dados e funcionamento das funcionalidades.

A aplicação apresenta funcionalidades básicas de cadastro e listagem, porém necessita de melhorias para garantir maior robustez, confiabilidade e melhor experiência ao usuário.

A execução dos testes demonstrou a importância de um processo estruturado de **garantia de qualidade de software (QA)** para identificar e corrigir problemas antes que afetem os usuários finais.
