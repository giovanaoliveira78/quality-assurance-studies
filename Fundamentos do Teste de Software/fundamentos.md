# 📘 Fundamentos do Teste de Software – Conceitos Essenciais para o Dia a Dia e Entrevistas

---

## 📌 1. O Que é Teste de Software?

> “Os testes são executados para descobrir situações em que o software se comporta de maneira incorreta, indesejável ou de forma diferente das especificações.” – Sommerville (2011)

- O teste **não garante ausência de defeitos**, mas **aumenta a confiança na qualidade**.
- Quanto mais cedo testar, **menor o custo da correção**.

---

## 📌 2. Verificação x Validação

| Conceito       | Descrição                                                                 |
|----------------|--------------------------------------------------------------------------|
| **Verificação** | O software foi construído corretamente? (ex: revisão de código, inspeção) |
| **Validação**   | O software certo foi construído? (ex: testes com base nos requisitos)     |

---

## 📌 3. Tipos de Teste por Nível

| Nível            | O que testa                                    | Responsável       |
|------------------|-------------------------------------------------|-------------------|
| **Unitário**     | Componentes isolados (funções, métodos)         | Desenvolvedor     |
| **Integração**   | Comunicação entre módulos                       | Dev / QA          |
| **Sistema**      | Sistema como um todo                            | QA                |
| **Aceitação**    | Validação final com dados reais e cliente       | Cliente + QA      |

---

## 📌 4. Teste Caixa Preta (Black-box)

- Foca no **comportamento externo** do software.
- O testador **não tem acesso ao código**.
- **Técnicas mais comuns:**
  - ### ✔ Particionamento de Equivalência
    > “O domínio de entrada de um programa é dividido em classes de dados de entrada de onde os casos de teste podem ser derivados.”  
    📄 *Página 19*
    - Divide os valores em classes válidas e inválidas.
    - Testa um valor representativo por classe.

  - ### ✔ Análise de Valor Limite
    > “Casos de teste são desenvolvidos com base nos limites de partições de equivalência.”  
    📄 *Página 19*
    - Testa os valores **nas bordas** do intervalo.

  - ### ✔ Tabela de Decisão
    > “Útil para representar a lógica de decisão [...] quando há número limitado de combinações.”  
    📄 *Página 20*
    - Mostra as condições e ações esperadas em uma tabela.

  - ### ✔ Estado-Transição
    > “Usada para testar sistemas que respondem a eventos dependendo do estado atual.”  
    📄 *Página 21*
    - Ideal para interfaces e sistemas com múltiplos estados.

> "Caixa preta é ideal para testar se o sistema está se comportando conforme o esperado, com base nos requisitos."

---

## 📌 5. Teste Caixa Branca (White-box)

- Foco na **estrutura interna e lógica do código**.
- O testador **tem acesso ao código-fonte**.
- **Técnicas comuns:**

  - ### ✔ Cobertura de Instruções
    > “Executar cada instrução do programa pelo menos uma vez.”  
    📄 *Página 23*

  - ### ✔ Cobertura de Decisões e Condições
    > “Cada decisão deve assumir valores verdadeiro e falso ao menos uma vez.”  
    📄 *Página 23*
    > “Cada condição booleana deve tomar os dois valores.”  
    📄 *Página 23*

  - ### ✔ Teste de Caminho Básico (McCabe)
    > “Construção de gráfico de fluxo e cálculo da complexidade ciclomática.”  
    📄 *Página 24*
    - Fórmula: `V(G) = E – N + 2`
    - Cada caminho independente deve ser testado.

---

## 📌 6. Testes de Regressão e Re-teste

| Tipo          | Objetivo                                                             |
|---------------|----------------------------------------------------------------------|
| **Re-teste**  | Verificar se o erro corrigido foi realmente resolvido               |
| **Regressão** | Verificar se funcionalidades existentes continuam funcionando       |

---

## 📌 7. Testes de Estresse e Performance

- Avaliam o comportamento do sistema sob **condições extremas**.

### Exemplos:
- **Estresse**: "10 mil usuários simultâneos"
- **Carga**: "100 requisições por segundo"
- **Performance**: "tempo de resposta inferior a 2 segundos"

---

## 📌 8. Processo de Teste – Ciclo de Vida

Etapas segundo Eliza e Lagares (2012):

1. **Planejamento**
   - Escopo, objetivos, riscos, ambiente de testes.
2. **Projeto**
   - Casos de teste, scripts, massa de dados.
3. **Execução**
   - Execução dos testes e registro de falhas.
4. **Entrega**
   - Apoio no teste de aceitação e documentação final.

---

## 📌 9. Artefatos de Teste

| Artefato                  | Finalidade                                                 |
|---------------------------|------------------------------------------------------------|
| **Plano de Teste**        | Estratégia, escopo, recursos                               |
| **Casos de Teste**        | Passos, entradas e resultados esperados                    |
| **Evidências de Teste**   | Prints, logs, documentos que provam a execução             |
| **Matriz de Rastreabilidade** | Mapeia requisitos ↔ casos de teste                  |

---

## 📌 10. Papéis no Processo de Teste

| Papel                  | Responsabilidades                                      |
|------------------------|--------------------------------------------------------|
| **Analista de Teste**  | Escreve planos e casos de teste, executa testes manuais |
| **Engenheiro de Teste**| Automatiza testes, configura ambiente                   |
| **Testador**           | Executa testes manuais e reporta defeitos              |
| **Coordenador de Teste**| Monitora indicadores, prazos e qualidade               |

---

## 📌 11. Boas Práticas para o Dia a Dia

- Use ferramentas como Jira, Azure DevOps.
- Comece a testar cedo (**Shift-left testing**).
- Use **análise de risco** para priorizar testes.
- **Automatize** testes repetitivos.
- Use **checklists** para garantir cobertura.
- Versione e compartilhe seus artefatos.

---