name: 🆕 Adicionar Novo Site
description: Sugerir a adição de um novo site de anime/mangá/manhua ao catálogo
labels: [Novo Site]
body:

  - type: input
    id: site-name
    attributes:
      label: Nome do Site
      description: |
        Nome do site que você deseja adicionar.
      placeholder: |
        Exemplo: "SlimeRead ou Mangalivre"
    validations:
      required: true

  - type: input
    id: site-url
    attributes:
      label: URL do Site
      description: |
        URL principal do site.
      placeholder: |
        Exemplo: "https://slimeread.com"
    validations:
      required: true

  - type: input
    id: site-language
    attributes:
      label: Idioma do Site
      description: |
        Idioma principal do site.
      placeholder: |
        Exemplo: "Português"
    validations:
      required: true

  - type: textarea
    id: site-description
    attributes:
      label: Descrição do Site
      description: |
        Breve descrição do site e do conteúdo que ele oferece.
      placeholder: |
        Exemplo: "SlimeRead é uma plataforma que oferece uma vasta coleção de mangás no idioma Português, com suporte para leitura online e download."
    validations:
      required: true

  - type: textarea
    id: site-features
    attributes:
      label: Funcionalidades do Site
      description: |
        Liste as funcionalidades principais do site.
      placeholder: |
        Exemplo:
          - Leitura online de mangás
          - Download de capítulos
          - Suporte para múltiplos idiomas
    validations:
      required: true

  - type: textarea
    id: site-popularity
    attributes:
      label: Popularidade do Site
      description: |
        Informações sobre a popularidade do site (opcional).
      placeholder: |
        Exemplo: "SlimeRead é um dos sites mais populares para leitura de mangás, com milhões de usuários ativos mensalmente."

  - type: checkboxes
    id: acknowledgements
    attributes:
      label: Confirmações
      description: Por favor, confirme que você fez os seguintes passos.
      options:
        - label: Eu pesquisei no repositório e este site não foi adicionado anteriormente.
          required: true
        - label: Eu forneci todas as informações necessárias sobre o site.
          required: true
        - label: Eu confirmo que o site é legítimo e não viola direitos autorais.
          required: true
        - label: Eu estou ciente de que a adição do site está sujeita à aprovação.
          required: true