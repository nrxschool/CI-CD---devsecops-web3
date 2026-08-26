# CI/CD e DevSecOps para Web3

**NearX | Formação em Blockchain**

---

## 1. Apresentação do Curso

Este curso apresenta os fundamentos, práticas e ferramentas de CI/CD aplicadas ao desenvolvimento Web3. O estudante aprenderá a automatizar testes, verificações de segurança e deploys de smart contracts em ambientes descentralizados, garantindo segurança, eficiência e confiabilidade no ciclo de desenvolvimento.

---

## 2. Objetivos do Curso

Ao final do curso, o aluno será capaz de:

- Compreender as diferenças arquiteturais críticas entre esteiras tradicionais (Web2) e os requisitos de imutabilidade e segurança de redes descentralizadas.
- Configurar workflows que executam formatação, linting e testes automatizados (unitários e com fork de rede real) a cada novo commit.
- Integrar ferramentas de análise estática (como o Slither) diretamente no pipeline para barrar vulnerabilidades financeiras (ex: Reentrancy) antes que o código seja mesclado.
- Orquestrar a publicação automatizada de Smart Contracts em redes de teste e produção, incluindo a verificação automática de código-fonte em exploradores de blocos (ex: Etherscan).
- Estruturar um fluxo onde o pipeline extrai os artefatos de build (ABIs e endereços) do contrato e os injeta de forma automatizada no deploy do Frontend descentralizado.

---

## 3. Público-Alvo

- Desenvolvedores;
- Engenheiros de Software;
- Profissionais de DevOps.

---

## 4. Pré-requisitos

### Controle de Versão

Familiaridade com Git e uso básico do GitHub (commits, branches, pull requests).

### Desenvolvimento Web

Conhecimento intermediário em JavaScript/TypeScript e noções de Node.js.

### Blockchain e Smart Contracts

Entendimento básico de como a EVM funciona e noções de programação em Solidity (saber o que é um contrato, funções e variáveis de estado).

---

# 5. Conteúdo Programático

## Módulo 1 — Fundamentos da Automação Web3

- **O Paradigma Web2 vs. Web3:** As limitações do CI/CD tradicional frente à arquitetura descentralizada.
- **A Imutabilidade como Fator Crítico:** O alto custo de regressões e a necessidade do “Shift-Left Security”.
- **Arquitetura de Repositórios:** Estratégias de Monorepo para orquestrar Smart Contracts e Frontend na mesma esteira.
- **Setup do Ambiente:** Configuração do controle de versão, Runners e definição dos stages do pipeline.

---

## Módulo 2 — Integração Contínua (CI) e Garantia de Qualidade

- **Padronização Estrita:** Configurando Jobs de Linting e formatação (Solhint/Prettier) para manter a integridade do código.
- **Automação de Testes:** Integração de testes unitários e de integração no pipeline (Hardhat ou Foundry).
- **Simulação de Estados (Mocks e Forking):** Como configurar a esteira para testar contratos manipulando o tempo (`block.timestamp`) ou espelhando o estado de uma rede real.
- **Controle de Custos de Execução:** Geração de relatórios de Gas Profiling automatizados para evitar que atualizações encareçam o uso do contrato.

---

## Módulo 3 — DevSecOps – Segurança Contínua no Pipeline

- **Auditoria Estática Automatizada:** Implementação do Slither e/ou Mythril para barrar preventivamente falhas clássicas (ex: Reentrância, Quebra de Controle de Acesso) antes do merge.
- **Fuzzing Básico (Opcional):** Introdução a testes baseados em propriedades para estressar a matemática do contrato no CI.
- **Gestão de Segredos:** Técnicas para mascarar e injetar com segurança Chaves Privadas, Mnemônicos e RPC URLs nas variáveis de ambiente da plataforma de CI.

---

## Módulo 4 — Entrega Contínua (CD) On-Chain

- **Determinismo de Deploy:** Criação de scripts automatizados para publicar contratos de forma consistente em ambientes de Teste e Produção.
- **Verificação Automatizada:** Integração com APIs de exploradores de blocos (como Etherscan) para publicar o código-fonte assim que o deploy for concluído.
- **Gestão de Artefatos de Build:** Orquestrando o pipeline para extrair as ABIs (Interfaces) e os endereços gerados, disponibilizando-os para os próximos serviços.

---

## Módulo 5 — CI/CD para Aplicações Clientes (Frontend/DApps)

- **Consumo de Artefatos:** Automatizando a injeção das ABIs geradas na etapa de CD diretamente no código da aplicação cliente.
- **Testes de Integração de UI:** Execução de testes automatizados para validar a conexão do frontend (React/Next.js) com as bibliotecas provedoras (Ethers.js/Viem).
- **Deploy Descentralizado e Híbrido:** Publicação da interface web através do pipeline em provedores tradicionais (Vercel) ou redes de armazenamento distribuído (IPFS).

---

# 6. Carga Horária

**Carga horária sugerida:** conforme a profundidade prática desejada.
