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
    [cite_start]Levantamento de Requisitos    :a1, 2025-01-01, 1w [cite: 11]
    [cite_start]Documentação Funcional        :a2, after a1, 1w [cite: 11]
    [cite_start]Rascunhos e Layout Definitivo :a3, after a2, 1w [cite: 12]

    section FASE 2: Desenvolvimento - Entregas Incrementais
    [cite_start]Configuração do Ambiente (Dev/DB/Git)  :d1, after a3, 1w [cite: 14]
    [cite_start]Criação do Banco de Dados              :d2, after d1, 1w [cite: 15]
    [cite_start]Programação do Módulo de Login         :crit, active, 2025-01-22, 1w [cite: 16]
    [cite_start]Entrega 1 (Login) :milestone, m1, 2025-01-28, 0d [cite: 28]
    [cite_start]Programação do CRUD de Empresas        :crit, 2w [cite: 17]
    [cite_start]Entrega 2 (CRUD) :milestone, m2, after d6, 0d [cite: 29]
    [cite_start]Implementação do Upload de Logotipo    :crit, 2w [cite: 18]
    [cite_start]Entrega 3 (Upload) :milestone, m3, after d7, 0d [cite: 30]
    [cite_start]Desenvolvimento dos Relatórios (PDF/Excel) :crit, 2w [cite: 19]
    [cite_start]Entrega 4 (Relatórios) :milestone, m4, after d8, 0d [cite: 31]
    [cite_start]Configuração do Painel Administrativo  :crit, 2w [cite: 20]
    [cite_start]Entrega 5 (Painel Adm) :milestone, m5, after d9, 0d [cite: 32]
    
    section FASE 3: Testes e Implantação
    [cite_start]Testes Unitários e de Integração (QA)  :t1, after m5, 4w [cite: 21]
    [cite_start]Testes de Usabilidade com Usuários     :t2, after t1, 4w [cite: 22]
    [cite_start]Implantação Final no Servidor e Entrega:t3, after t2, 4w [cite: 23]
    [cite_start]Entrega Final (Sistema Validado) :milestone, m6, after t3, 0d [cite: 33]
```
