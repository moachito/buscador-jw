# 📖 Wiki do Projeto: Buscador Inteligente JW

Este documento serve como a "Fonte Única da Verdade" (Single Source of Truth) para a arquitetura, decisões e progresso do projeto.

---

## 🛠️ Stack Tecnológica
| Camada | Tecnologia | Descrição |
| :--- | :--- | :--- |
| **Runtime** | Node.js (LTS) | Motor que executa nosso código JavaScript no servidor. |
| **Frontend** | React | Biblioteca para construção da interface de usuário. |
| **Versionamento** | Git / GitHub | Controle de versão e hospedagem do código. |
| **Padrão de Módulos** | ESM (ECMAScript Modules) | Uso de `import/export` para código moderno e limpo. |

---

## 📂 Estrutura de Pastas
- `docs/`: Documentação técnica e registros de aprendizado.
- `src/`: Todo o código-fonte da aplicação.
  - `scripts/`: Utilitários para captura e processamento de dados (ex: `extrator.js`).
- `package.json`: Manifesto do projeto e gerenciamento de dependências.

---

## ✅ Funcionalidades Implementadas
### 📡 Extração de Dados (Data Scrapping)
- [x] Conexão com servidores externos via Fetch API.
- [x] Captura de arquivos `.vtt` (WebVTT) brutos.
- [x] Tratamento básico de erros e fluxos assíncronos (`async/await`).

---

## 🏗️ Decisões Arquiteturais (ADRs)
1. **ES Modules over CommonJS:** Adotado o `"type": "module"` no `package.json` para garantir compatibilidade futura com ferramentas de build modernas (Vite/React).
2. **Local Development over Cloud IDEs:** Decisão de focar no ambiente local (VS Code) para domínio completo do FileSystem e Git.

---

## 🚀 Próximos Marcos (Roadmap)
1. **Parser de VTT:** Transformar texto bruto em objetos JSON estruturados.
2. **Normalização de Tempo:** Converter timecodes (HH:MM:SS) em segundos numéricos.
3. **Módulo de Pesquisa:** Implementar busca por palavras-chave em memória.
4. **Integração IA:** Conectar o texto extraído a um modelo de linguagem para síntese.