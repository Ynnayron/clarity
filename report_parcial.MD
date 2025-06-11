# 📄 Relatório de Acompanhamento de Projeto — Sistemas Multiagente

> Preencha com atenção. Este relatório tem o objetivo de **organizar o pensamento, identificar bloqueios e alinhar os próximos passos do seu projeto**.

---

## 🧠 1. Visão Geral do Projeto

- **Título do Projeto**:  
Clarity agente de documentação de software
- **Integrantes da Equipe**:  
  - Fabricio Moreno (interface e integração)
  - Ynnayron Juan (LLM e arquitetura)

- **Resumo em uma frase**:  
  Um agente que documenta qualquer projeto de software.

---

## ⚙️ 2. Arquitetura Atual

- **Quantos agentes existem no sistema atualmente?**  
  Apenas 1 agente: `AgenteGeradorDocumentação`.

- **Função principal de cada agente:**  
  Receber acesso a todo projeto de via vscode e gera um readme e gera um diagrama de classes.

- **Eles interagem entre si? Como?**  
  Ainda não. A ideia final é dividir as tarefas em dois agentes um de leitura e interpretação do projeto e outro para gerar os diagramas.

- **Já existe algum ambiente de simulação/teste?**  
  Não.

---

## ✅ 3. Avanços Concretos

- Desenvolvimento da extensão do sistema para vscode.
- LLM com acesso ao projeto.

---

## 🧱 4. Dificuldades Enfrentadas

- A LLM alucina em algumas partes do readme e da geração do diagrama
- Adicionar mais features ao projeto
- Integrar o sistema a uma extensão no vscode

---

## 🛠️ 5. Estratégias de Superação

- Ajustamos o chunking para considerar hierarquia de headings no `.docx`.
- Testamos usar o `e5-base` no lugar do `e5-small`, mas não tivemos ganho significativo.
- Fizemos logging dos documentos retornados na busca vetorial para entender o que está vindo.

---

## 🎯 6. Próximos Passos

- Testar om sistema com outros projetos.
- Realizar fine tuning.
- integrar um novo agente para a geração dos diagramas.

---

## 📢 7. Pedido de Ajuda

- Precisamos de ajuda para realizar um fine tuning do modelo.
- Também gostaríamos de ouvir sugestões de novas features.

---
