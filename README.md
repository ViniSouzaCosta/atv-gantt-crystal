# atv-gantt-crystal

```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title Cronograma do Projeto - Sistema de Cadastro de Empresas Parceiras
    excludes weekends

    section Planejamento
    Levantamento de\nRequisitos           :done,    reqs, 2025-10-01, 7d
    Documentação Funcional\n e Layout     :active,  docs, after reqs, 10d

    section Desenvolvimento
    Configuração do\nAmbiente             :dev1, after docs, 7d
    Criação do Banco\n de Dados           :dev2, after dev1, 10d
    Módulo de Login\n(Autenticação)       :dev3, after dev2, 12d
    CRUD de\nEmpresas                    :dev4, after dev3, 14d
    Upload de\nLogotipo                  :dev5, after dev4, 10d
    Relatórios\nPDF/Excel                :dev6, after dev5, 10d
    Painel\nAdministrativo               :dev7, after dev6, 12d

    section Testes e Entrega
    Testes Unitários\ne de Integração     :qa1, after dev7, 10d
    Testes de\nUsabilidade               :qa2, after qa1, 7d
    Implantação Final\ne Entrega          :deliver, after qa2, 5d

  ```
