# 📘 Técnicas de Teste de Software – Resumo

Este documento resume os principais pontos abordados no conteúdo da disciplina, organizado por capítulos e técnicas relevantes para prática de testes.

---

## ✅ Fundamentos de Testes de Software

### ✔ Verificação vs Validação
- **Verificação**: garante que o software foi construído corretamente.
- **Validação**: garante que o software certo foi construído.

### ✔ Níveis de Teste
1. **Teste de Unidade**: verifica componentes isolados (módulos, funções).
2. **Teste de Integração**: testa interfaces entre componentes integrados.
3. **Teste de Validação**: assegura que o sistema atende aos requisitos do cliente.

---

## ✅ Técnicas de Teste Estruturais (Caixa Branca)

### ✔ Conceito
- Baseia-se na **estrutura interna** do código.
- Exige conhecimento do funcionamento interno do programa.

### ✔ Critérios Baseados em Fluxo de Controle
- **Todos-Nós, Todas-Arestas, Todos-Caminhos**.
- **Cobertura de condições e decisões**, **caminhos independentes**.

### ✔ Teste de Caminho Básico (McCabe)
- Usa **grafos de fluxo** para calcular a **complexidade ciclomática**:
  - `V(G) = E - N + 2` ou `V(G) = P + 1`
- Garante que todos os caminhos lógicos são testados ao menos uma vez.

### ✔ Variações:
- **Teste de condição** (booleans e expressões relacionais).
- **Teste de fluxo de dados** (definição e uso de variáveis).
- **Teste de ciclo** (loops simples, aninhados, concatenados).

---

## ✅ Testes Funcionais (Caixa Preta)

### ✔ Conceito
- Baseado nos **requisitos funcionais**, sem considerar a lógica interna.
- Foca no **comportamento externo do sistema**.

### ✔ Técnicas:
1. **Baseado em Grafos**:
   - Modelos: fluxo de transição, estados finitos, fluxo de dados.
2. **Particionamento de Equivalência**:
   - Divide entradas em **classes válidas e inválidas**.
3. **Análise de Valor Limite (BVA)**:
   - Testa **valores nas bordas** de intervalos.
4. **Teste de Matriz Ortogonal**:
   - Combina fatores e valores com **mínimo de testes e máxima cobertura**.
5. **Error Guessing**:
   - Baseado na **experiência do testador** para prever onde há chances de erro.

---

## ✅ Outras Técnicas de Teste de Software

### ✔ Testes Alfa e Beta
- **Alfa**: usuários testam no ambiente do desenvolvedor.
- **Beta**: teste ocorre no ambiente do usuário, sem supervisão direta.

### ✔ Testes de Regressão
- Garantem que **mudanças no código não causem novos defeitos**.
- Reexecutam testes antigos para validar alterações.

### ✔ Testes Não Funcionais
- Avaliam:
  - **Desempenho, usabilidade, segurança, confiabilidade, escalabilidade.**
- **Teste de estresse**: avalia limites do sistema em situações extremas.

### ✔ Teste para Ambientes e Arquiteturas
- Testes específicos para:
  - **Interfaces gráficas (GUIs)**.
  - **Ambientes distribuídos (cliente-servidor)**.

---

## 📚 Referências Importantes
- **Pressman (2011)** – Engenharia de Software.
- **Sommerville (2011)** – Engenharia de Software.
- **Jino, Maldonado, Delamaro (2016)** – Introdução ao Teste de Software.
- **Lourenço (2010)** – Testes de estresse e desempenho.
- **RUP-VC (2006)** – Teste de aceitação.

---