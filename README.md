# API-REST
Publicação de uma API REST na Nuvem Usando Spring Boot 3, Java 17 e Railway


classDiagram
    class User {
        +String name
        +Account account
        +Card card
        +List~Feature~ features
        +List~News~ news
    }

    class Account {
        +String number
        +String agency
        +String balance
        +float limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +float limit
    }

    class News {
        +String icon
        +String description
    }

    User --> Account
    User --> Card
    User --> Feature : has many
    User --> News : has many
