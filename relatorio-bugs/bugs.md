# Relatório de Bugs

Este documento apresenta os bugs identificados durante a execução dos testes no módulo de **cadastro e listagem de cursos** da aplicação.

---

## BUG 1 – Sistema permite cadastro de curso sem nome

**Severidade:** Alta  

**Descrição:**  
O sistema permite cadastrar um curso mesmo quando o campo **nome do curso** está vazio.

**Passos para reproduzir:**

1. Acessar a página de cadastro de cursos  
2. Deixar o campo **Nome do curso** vazio  
3. Preencher os demais campos  
4. Clicar em **Salvar**

**Resultado atual:**  
O sistema permite concluir o cadastro do curso.

**Resultado esperado:**  
O sistema deve impedir o cadastro e exibir mensagem informando que o campo é obrigatório.

---

## BUG 2 – Exclusão de curso não remove item da listagem

**Severidade:** Alta  

**Descrição:**  
Ao excluir um curso, o sistema exibe mensagem de sucesso, porém o curso permanece na listagem mesmo após atualizar a página.

**Passos para reproduzir:**

1. Acessar a aplicação  
2. Cadastrar um novo curso  
3. Ir para a listagem de cursos  
4. Clicar na opção **Excluir**  
5. Confirmar a exclusão  
6. Atualizar a página (refresh)

**Resultado atual:**  
O sistema mostra mensagem de exclusão concluída, porém o curso continua aparecendo na lista.

**Resultado esperado:**  
O curso deve ser removido da listagem e não deve aparecer após atualizar a página.

---

## BUG 3 – Sistema não possui opção para editar cursos cadastrados

**Severidade:** Média  

**Descrição:**  
Não existe opção na interface para editar informações de cursos cadastrados.

**Passos para reproduzir:**

1. Acessar a aplicação  
2. Cadastrar um curso  
3. Ir para a listagem de cursos  
4. Verificar se existe opção para editar o curso

**Resultado atual:**  
A interface não apresenta opção de edição.

**Resultado esperado:**  
O sistema deveria disponibilizar opção para editar cursos cadastrados.

---

## BUG 4 – Sistema permite cadastro de cursos duplicados

**Severidade:** Média  

**Descrição:**  
O sistema permite cadastrar múltiplos cursos com **nome e dados idênticos**, sem qualquer validação ou alerta.

**Passos para reproduzir:**

1. Cadastrar um curso com determinado nome  
2. Cadastrar outro curso utilizando os mesmos dados

**Resultado atual:**  
O sistema permite cadastrar cursos duplicados.

**Resultado esperado:**  
O sistema deveria impedir duplicidade ou alertar o usuário.

---

## Resumo dos Bugs

Total de bugs encontrados: **4**

- **Alta severidade:** 2  
- **Média severidade:** 2

Esses problemas podem impactar a **integridade das informações do sistema e a experiência do usuário**, sendo recomendada a correção antes da disponibilização da aplicação em ambiente de produção.
