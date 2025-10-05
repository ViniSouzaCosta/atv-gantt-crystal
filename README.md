# atv-gantt-crystal

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Cronograma do Projeto - Sistema de Cadastro de Empresas Parceiras
    excludes weekends

    section Planejamento
    Req.                     :done,    reqs, 2025-10-01, 7d
    Doc. e Layout           :active,  docs, after reqs, 10d

    section Desenvolvimento
    Amb. Config.           :dev1, after docs, 7d
    Banco de Dados                  :dev2, after dev1, 10d
    Login e Autenticação            :dev3, after dev2, 12d
    CRUD de Empresas                :dev4, after dev3, 14d
    Upload Logotipo                 :dev5, after dev4, 10d
    Relat. PDF e Excel              :dev6, after dev5, 10d
    Painel Administrativo           :dev7, after dev6, 12d

    section Testes e Entrega
    Test. e Integ.                  :qa1, after dev7, 10d
    Usabilidade                     :qa2, after qa1, 7d
    Impla. Final                    :deliver, after qa2, 5d





  ```
```mermaid
graph TD
    gantt
    title Planejamento do Projeto - Sistema de Cadastro de Empresas Parceiras
    dateFormat  YYYY-MM-DD
    axisFormat  %m-%d

    section FASE 1: Documentação e Design
    Levantamento de Requisitos    :a1, 2025-01-01, 1w
    Documentação Funcional        :a2, after a1, 1w
    Rascunhos e Layout Definitivo :a3, after a2, 1w

    section FASE 2: Desenvolvimento - Entregas Incrementais
    Configuração do Ambiente (Dev/DB/Git)  :d1, after a3, 1w
    Criação do Banco de Dados              :d2, after d1, 1w
    Programação do Módulo de Login         :crit, active, 2025-01-22, 1w  
    **Entrega 1 (Login)** :milestone, m1, 2025-01-28, 0d
    Programação do CRUD de Empresas        :crit, 2w
    **Entrega 2 (CRUD)** :milestone, m2, after d6, 0d
    Implementação do Upload de Logotipo    :crit, 2w
    **Entrega 3 (Upload)** :milestone, m3, after d7, 0d
    Desenvolvimento dos Relatórios (PDF/Excel) :crit, 2w
    **Entrega 4 (Relatórios)** :milestone, m4, after d8, 0d
    Configuração do Painel Administrativo  :crit, 2w
    **Entrega 5 (Painel Adm)** :milestone, m5, after d9, 0d
    
    section FASE 3: Testes e Implantação
    Testes Unitários e de Integração (QA)  :t1, after m5, 4w
    Testes de Usabilidade com Usuários     :t2, after t1, 4w
    Implantação Final no Servidor e Entrega:t3, after t2, 4w
    **Entrega Final (Sistema Validado)** :milestone, m6, after t3, 0d
    classDef amarelo fill:#FFD84D, stroke:#000, stroke-width:1px;
    classDef laranja fill:#FFA233, stroke:#000, stroke-width:1px;
    classDef vermelho fill:#E64C3C, stroke:#000, stroke-width:1px;
```
