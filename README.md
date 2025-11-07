# Batalha-_de_Gladiadores
Uma projeto que simula uma batalha entre gladiadores, utilizando métodos de programa como POO, Orientada a Eventos, Estruturada, Procedural
🏛️ Batalha de Gladiadores
<p align="center"> <img src="https://cdn-icons-png.flaticon.com/512/742/742751.png" width="120" alt="Gladiador Icon"/> </p>

⚔️ Um projeto acadêmico desenvolvido por Richard para a disciplina de Programação de Soluções Computacionais, com o objetivo de aplicar os conceitos de Programação Orientada a Objetos (POO) e desenvolvimento com Spring Boot.

🧩 Descrição

O projeto Batalha de Gladiadores simula combates entre dois gladiadores em uma arena repleta de torcedores.
Cada gladiador possui nome, vidas, armadura e uma arma, que influencia na força dos golpes.
A arena reage de acordo com o resultado da batalha — ficando feliz ou triste, e alterando o número de torcedores.

🎯 Objetivos do Projeto

Aplicar conceitos de POO (abstração, encapsulamento, herança e polimorfismo).

Praticar estruturas de controle, objetos e métodos.

Desenvolver com Spring Boot e Maven.

Criar um sistema modular e escalável.

Implementar uma lógica de batalha dinâmica e atualização de estado da arena.

⚙️ Tecnologias Utilizadas
Tecnologia	Descrição
☕ Java 17+	Linguagem principal
🌱 Spring Boot	Framework para criação de aplicações Java modernas
🧩 Maven	Gerenciador de dependências e build
🧠 POO (Programação Orientada a Objetos)	Estrutura base da aplicação
🧰 Lombok	Reduz código boilerplate
🧪 JUnit	Testes automatizados
🏗️ Estrutura do Projeto
batalha-de-gladiadores/
│
├── src/main/java/com/richard/gladiadores/
│   ├── model/
│   │   ├── Arma.java
│   │   ├── Gladiador.java
│   │   └── Arena.java
│   │
│   ├── service/
│   │   └── BatalhaService.java
│   │
│   ├── controller/
│   │   └── BatalhaController.java
│   │
│   └── GladiadoresApplication.java
│
├── src/test/java/com/richard/gladiadores/
│
└── pom.xml
🧙‍♂️ Regras da Batalha
Elemento	Descrição
Gladiador	Possui nome, 5 vidas e pode usar armadura
Armadura	Reduz o dano em 2 pontos da força da arma adversária
Armas	Espada (5), Lança (4), Arco e Flecha (3)
Arena	Possui torcedores; ficam felizes ou tristes após a luta
Torcida	Se ambos sobrevivem → torcida triste (-25%)
Se há morte → torcida feliz (+10%)
💥 Exemplo de Simulação
🏟️ Arena inicial: 1000 torcedores (felizes)

⚔️ Gladiador 1: Maximus (Espada, com armadura)
⚔️ Gladiador 2: Spartacus (Lança, sem armadura)

💥 Maximus ataca Spartacus com Espada (força 5)
➡️ Spartacus perde 5 vidas

💥 Spartacus ataca Maximus com Lança (força 4, reduzida para 2)
➡️ Maximus perde 2 vidas

☠️ Spartacus morreu!  
🎉 Torcida feliz! (+10%) → 1100 torcedores

🧠 Conceitos Aplicados

Classes e Objetos

Encapsulamento de atributos

Regras de negócio com métodos

Controle de estado (vida, armadura, torcida)

Simulação via lógica de combate

Injeção de dependência (Spring Boot)

Boas práticas de arquitetura (MVC)

🚀 Como Executar
1️⃣ Clone o repositório
git clone https://github.com/seuusuario/batalha-de-gladiadores.git

2️⃣ Entre na pasta do projeto
cd batalha-de-gladiadores

3️⃣ Compile e rode o projeto
mvn spring-boot:run

4️⃣ Acesse no navegador
http://localhost:8080

🧩 Exemplo de Requisição (API REST)

POST /batalha/iniciar

🔹 Exemplo JSON
{
  "gladiador1": { "nome": "Maximus", "armadura": true, "arma": "Espada" },
  "gladiador2": { "nome": "Spartacus", "armadura": false, "arma": "Lança" },
  "torcedores": 1000
}

🔹 Exemplo de Resposta
{
  "resultado": "Spartacus morreu!",
  "torcedores": 1100,
  "status": "Torcida feliz!"
}

📸 Futuras Melhorias

Interface Web para o combate

Sistema de ranking de gladiadores

Persistência em banco de dados (JPA/H2)

Histórico de batalhas

Efeitos sonoros e visuais

🧾 Autor

Projeto desenvolvido por Diego Vinicius

⭐ Mostre seu apoio!

Se gostou do projeto:

⭐ Dê uma estrela no repositório!

<p align="center">Feito com ☕, 💡 e muita coragem de gladiador!</p>
