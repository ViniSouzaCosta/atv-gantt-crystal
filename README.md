# atv-gantt-crystal

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Cronograma do Projeto - Sistema de Cadastro de Empresas Parceiras
    excludes weekends

    section Planejamento
    Levantamento de Requisitos           :done,    reqs, 2025-10-01, 7d
    Documentação Funcional e Layout      :active,  docs, after reqs, 10d

    section Desenvolvimento
    Configuração do Ambiente             :dev1, after docs, 7d
    Criação do Banco de Dados            :dev2, after dev1, 10d
    Módulo de Login                      :dev3, after dev2, 12d
    CRUD de Empresas                     :dev4, after dev3, 14d
    Upload de Logotipo                   :dev5, after dev4, 10d
    Relatórios PDF/Excel                 :dev6, after dev5, 10d
    Painel Administrativo                :dev7, after dev6, 12d

    section Testes e Entrega
    Testes Unitários e de Integração     :qa1, after dev7, 10d
    Testes de Usabilidade                :qa2, after qa1, 7d
    Implantação Final e Entrega          :deliver, after qa2, 5d
  ```
