# SERVIÇO NACIONAL DE APRENDIZAGEM COMERCIAL
## SENAC

---

### CURSO DE TECNOLOGIA EM ANÁLISE E DESENVOLVIMENTO DE SISTEMAS

---

### PROJETO INTEGRADOR III:
DESENVOLVIMENTO DE SISTEMAS ORIENTADO A OBJETOS

---

**Autores:**
* André Trecco
* Edward Mairene Ribeiro
* Rafaela Correa Pastor
* Vivian Barbosa Pinheiro

---

EAD - ENSINO À DISTÂNCIA - 2025

---

**Professor:**
Enoque Felipe dos Santos Leal

---

**Trabalho para aprovação em disciplina**

---

# Sumário

1. Diagrama de casos de uso
2. Descrição dos cenários dos casos de uso
3. Diagrama de classe
4. Protótipos
5. Arquivo do Projeto no GitHub

---

### Referências

# 1. DIAGRAMA DE CASOS DE USO

---

![Figura 1. Diagrama de Casos de Uso de Sistema de Cadastro de Universidade.](https://lucid.app/lucidchart/e03dbe29-88c3-488e-a2e4-ea9a64c4d8dc/edit?viewport_loc=-588%2C2%2C2558%2C1184%2C.Q4MUjXso07N&invitationId=inv_903969aa-6a98-4e90-9e3f-6f6fa28d3767)

---

# 2. DESCRIÇÃO DOS CENÁRIOS DOS CASOS DE USO

---

### 2.1 Caso de Uso 1: Cadastro de Aluno

* **Atores Principais:** Secretária e Aluno.
* **Pré-condição:** Ambos devem estar autenticados no sistema.
* **Pós-condição:** O aluno é cadastrado com uma matrícula gerada automaticamente.

**Cenário Principal:**
1.  Secretária ou Aluno acessa a função "Cadastrar Aluno" no sistema.
2.  Informa os dados pessoais do aluno (nome, CPF).
3.  O sistema valida o CPF.
4.  O sistema gera automaticamente uma matrícula.
5.  O aluno é adicionado à base de dados.

**Cenário Alternativo 1 — CPF inválido:**
* 3a. O sistema detecta um CPF inválido.
* 3b. É exibida uma mensagem de erro e o cadastro é cancelado.

**Cenário Alternativo 2 — CPF já cadastrado:**
* 3a. O CPF informado já pertence a um aluno existente.
* 3b. O sistema informa que o aluno já está cadastrado.

---

### 2.2 Caso de Uso 2: Cadastro de Professor

* **Atores Principais:** Secretária e Professor.
* **Pré-condição:** Ambos devem estar autenticados no sistema.
* **Pós-condição:** O professor é cadastrado e sua disciplina associada.

**Cenário Principal:**
1.  Secretária ou Professor acessa a opção "Cadastrar Professor".
2.  Informa nome, CPF e disciplina.
3.  O sistema valida o CPF.
4.  O sistema registra o professor com os dados informados.

**Cenário Alternativo 1 — CPF inválido:**
* 3a. O sistema detecta um CPF inválido.
* 3b. Exibe mensagem de erro e cancela o cadastro.

**Cenário Alternativo 2 — Campo de disciplina vazio:**
* 2a. O campo "disciplina" não é preenchido.
* 2b. O sistema alerta sobre o campo obrigatório.

---

### 2.3 Caso de Uso 3: Cadastro de Fornecedor

* **Ator Principal:** Fornecedor.
* **Pré-condição:** O fornecedor deve estar autenticado no sistema.
* **Pós-condição:** O fornecedor é cadastrado junto aos seus produtos.

**Cenário Principal:**
1.  Fornecedor acessa "Cadastrar Fornecedor".
2.  Informa nome, ramo e CNPJ.
3.  O sistema valida o CNPJ.
4.  O fornecedor insere uma lista de produtos (nome, preço, categoria).
5.  O sistema salva os dados.

**Cenário Alternativo 1 — CNPJ inválido:**
* 3a. O sistema detecta um CNPJ inválido.
* 3b. Exibe mensagem de erro e não realiza o cadastro.

**Cenário Alternativo 2 — Nenhum produto informado:**
* 4a. Nenhum produto é adicionado.
* 4b. O sistema alerta que pelo menos um produto deve ser registrado.

---

### 2.4 Caso de Uso 4: Listar Produtos

* **Ator Principal:** Universidade.
* **Pré-condição:** A universidade deve estar autenticada no sistema.
* **Pós condição:** Uma lista de produtos dos fornecedores cadastrados é exibida.

**Cenário Principal:**
1.  Universidade acessa "Listar Produtos".
2.  O sistema busca todos os fornecedores cadastrados.
3.  Recupera e exibe os produtos associados a esses fornecedores.

**Cenário Alternativo 1 — Nenhum fornecedor cadastrado:**
* 2a. O sistema detecta que não há fornecedores vinculados.
* 2b. Exibe a mensagem: “Nenhum fornecedor foi encontrado”.

**Cenário Alternativo 2 — Produtos não disponíveis:**
* 3a. O sistema detecta que os fornecedores não possuem produtos cadastrados.
* 3b. Exibe a mensagem: “Sem produtos disponíveis no momento”.

---

### 2.5 Observações:

* Os casos de uso estão diretamente conectados às responsabilidades das classes no diagrama de classes.
* O sistema prevê validações essenciais (como CPF e CNPJ) e garante integridade nos cadastros.
* A secretária exerce papel administrativo, enquanto a universidade interage principalmente com produtos.
* Os cenários alternativos reforçam a robustez do sistema frente a falhas ou dados incompletos.

---

# 3. DIAGRAMA DE CLASSES

---

![Figura 2. Diagrama de Classes de Sistema de Cadastro de Universidade.](https://lucid.app/lucidchart/e03dbe29-88c3-488e-a2e4-ea9a64c4d8dc/edit?viewport_loc=-623%2C23%2C2558%2C1184%2C-gNnRRc.eFz5&invitationId=inv_903969aa-6a98-4e90-9e3f-6f6fa28d3767)

---

# REFERÊNCIAS

* OLIVEIRA, H. P. G. **Análise de sistemas**. São Paulo: Editora Senac São Paulo, 2019. (Série Universitária)
* PESSÔA FILHO, J. **Programação orientada a objetos com C#**. São Paulo: Editora Senac São Paulo, 2023. (Série universitária)
