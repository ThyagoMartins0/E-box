E-commerce criado com microsservices, mensageria e kubernets

COMO NOVO DESAFIO, PRETENDO DESENVOLVER UM E-COMMERCE UTILIZANDO JAVA E ANGULAR
![image](https://github.com/ThyagoMartins0/E-box/assets/58978196/a692c9e2-d474-4f2c-8ea9-77ed0a60b63e)

![image](https://github.com/ThyagoMartins0/E-box/assets/58978196/8531b2e1-e54a-47e4-95de-d5d68f1084f9)



DETALHES TECNICOS 

messaging
https://www.canva.com/design/DAGI1ZapLcQ/HlM7sBYyuMYwUVIezWVB8A/view?utm_content=DAGI1ZapLcQ&utm_campaign=designshare&utm_medium=link&utm_source=editor
PADRÃO ARQUITETURAL 
DDD
FOI PENSANDO EM DDD DEVIDO SUA CLAREZA NA MODELAGEM DE DOMINIO
com.example.ecommerce
│
├── application
│   ├── service
│   ├── dto
│   └── messaging
│       ├── command
│       ├── event
│       └── handler
│
├── domain
│   ├── model
│   │   ├── entity
│   │   ├── valueobject
│   │   └── aggregate
│   ├── repository
│   └── service
│
├── infrastructure
│   ├── repository
│   │   └── jpa
│   ├── messaging
│   │   ├── kafka
│   │   └── rabbitmq
│   └── configuration
│
└── presentation
├── controller
└── view