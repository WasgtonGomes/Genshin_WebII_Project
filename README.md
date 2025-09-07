# ProgetoWeb# 🎮 Genshin Impact Web II Project

## 📌 Objetivo do Projeto
Este projeto foi desenvolvido como **atividade final da disciplina Programação Web II** (IFRO - Ji-Paraná) com o objetivo de aplicar de forma prática os conceitos aprendidos durante o semestre. O sistema permite o **cadastro, consulta e gerenciamento de personagens do jogo Genshin Impact**, utilizando tanto dados inseridos pelo usuário quanto informações obtidas via API externa.

O projeto demonstra conhecimentos em **desenvolvimento web full-stack**, integração com **banco de dados MySQL**, consumo de **APIs externas** e boas práticas de **validação e usabilidade**.

# 🎮 Genshin Impact Web II Project

## 📌 Objetivo do Projeto
Este projeto foi desenvolvido como **atividade final da disciplina Programação Web II** (IFRO - Ji-Paraná), com o objetivo de aplicar os conceitos aprendidos durante o semestre.  

O sistema permite o **cadastro, consulta e gerenciamento de personagens do jogo Genshin Impact**, utilizando dados inseridos pelo usuário e informações obtidas via **API externa**.  

Demonstra conhecimentos em **desenvolvimento web full-stack**, integração com **banco de dados MySQL**, consumo de **APIs externas** e boas práticas de **validação e usabilidade**.


---

## 🏫 Disciplina

**Programação Web II** — Aplicação prática de conceitos avançados de desenvolvimento web, incluindo Node.js, HTML, CSS, JavaScript, Bootstrap, e integração com banco de dados relacional e APIs externas.
=======
**Programação Web II** — Aplicação prática de conceitos avançados de desenvolvimento web, incluindo:

- Node.js  
- HTML5 & CSS3  
- JavaScript  
- Bootstrap 4  
- Integração com banco de dados relacional e APIs externas  


---

## 🛠️ Ferramentas e Tecnologias Utilizadas

- **Node.js** — Back-end, gerenciamento de rotas, manipulação de dados e integração com API.
- **Express.js** — Framework para criação de servidor web e gerenciamento de endpoints.
- **MySQL** — Banco de dados relacional para armazenamento e consulta de informações dos personagens.
- **Axios & node-fetch** — Consumo de APIs externas.
- **@vitalets/google-translate-api** — Tradução de dados da API para o português.
- **HTML5, CSS3, JavaScript** — Construção das interfaces e interatividade.
- **Bootstrap 4** — Responsividade e estilização das páginas.
=======

| Tecnologia | Ícone | Finalidade |
|------------|-------|------------|
| **Node.js** | ![Node.js](https://img.icons8.com/color/48/000000/nodejs.png) | Back-end, gerenciamento de rotas, manipulação de dados |
| **Express.js** | ![Express](https://img.icons8.com/ios/50/000000/express-js.png) | Framework para servidor web e endpoints |
| **MySQL** | ![MySQL](https://img.icons8.com/ios-filled/50/000000/mysql-logo.png) | Banco de dados relacional |
| **Axios** | ![Axios](https://img.shields.io/badge/Axios-API-blue?logo=axios&logoColor=white) | Consumo de APIs externas |
| **node-fetch** | ![Node-Fetch](https://img.shields.io/badge/node--fetch-HTTP-green?logo=node.js&logoColor=white) | Requisições HTTP |
| **@vitalets/google-translate-api** | ![Google Translate](https://img.icons8.com/ios-filled/50/000000/google-translate.png) | Tradução automática de dados |
| **HTML5** | ![HTML5](https://img.icons8.com/color/48/000000/html-5.png) | Estrutura das páginas |
| **CSS3** | ![CSS3](https://img.icons8.com/color/48/000000/css3.png) | Estilização e layout |
| **JavaScript** | ![JavaScript](https://img.icons8.com/color/48/000000/javascript.png) | Interatividade e lógica |
| **Bootstrap 4** | ![Bootstrap](https://img.icons8.com/color/48/000000/bootstrap.png) | Responsividade e componentes visuais |


---

## 💻 Linguagens

- JavaScript (Node.js e front-end)
- HTML5
- CSS3
- SQL (MySQL)

---

## ⚙️ Métodos e Funcionalidades
- **CRUD completo** (Create, Read, Update, Delete) para gerenciamento de personagens.
- **Validação de formulários** para garantir integridade dos dados.
- **Integração com API externa do Genshin Impact**, incluindo tradução automática de dados.
- **Organização das rotas** para separar cadastro, consulta e inserção de dados via API.
- **Interface responsiva** com Bootstrap, garantindo boa usabilidade em diferentes dispositivos.

---

## 🖼️ Páginas e Prints do Projeto

### 1️⃣ Tela Inicial (`inicial.html`)
- **Finalidade:** Página de entrada do sistema, apresentando o projeto e facilitando o acesso às funcionalidades.
- **Relevância:** Serve como hub principal, conectando todas as páginas do sistema.  
- **Print:** ![Tela Inicial](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Welcome.PNG)

---

### 2️⃣ Tela de Cadastro de Personagem (`formulario.html`)
- **Finalidade:** Permite que o usuário cadastre personagens personalizados com atributos detalhados (elemento, arma, habilidades, estatísticas).
- **Relevância:** Implementa o **Create** do CRUD e validação de dados.  
- **Prints:**  
  ![Cadastro 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character01.PNG)  
  ![Cadastro 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character02.PNG)  
  ![Cadastro 03](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character03.PNG)

---

### 3️⃣ Tela de Confirmação de Cadastro (`Page_registration_character05_registration_confirmation.PNG`)
- **Finalidade:** Confirma ao usuário que o personagem foi registrado com sucesso.
- **Relevância:** Feedback visual importante para a **experiência do usuário**.  

---

### 4️⃣ Tela de Consulta de Personagens (`tabelaCadastrados.html`)
- **Finalidade:** Lista todos os personagens cadastrados pelo usuário e permite consultas detalhadas.
- **Relevância:** Implementa o **Read** do CRUD, permitindo visualização organizada dos dados.  
- **Prints:**  
  ![Consulta 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Check_registration01.PNG)  
  ![Consulta 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Check_registration02.PNG)

---

### 5️⃣ Tela de Integração com API (`personagensAPI.html`)
- **Finalidade:** Exibe informações dinâmicas de personagens do Genshin Impact obtidas de uma API externa.
- **Relevância:** Demonstra **consumo de API**, tradução de dados e integração com o banco.  

---

### 6️⃣ Tela da Equipe de Desenvolvimento (`equipeDesenvolvimento.html`)
- **Finalidade:** Apresenta os integrantes do projeto, suas funções e responsabilidades.
- **Relevância:** Evidencia a **colaboração e organização do time**.  
- **Prints:**  
  ![Equipe 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_development_team01.PNG)  
  ![Equipe 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_development_team02.PNG)

---

### 7️⃣ Tela de Descrição do Projeto (`descricao.html`)
- **Finalidade:** Explica detalhadamente os objetivos do projeto, tecnologias usadas e funcionalidades implementadas.
- **Relevância:** Fornece contexto completo para avaliadores e futuros desenvolvedores.  
- **Prints:** ![Descrição](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Description01.PNG)

=======
- ![JavaScript](https://img.icons8.com/color/48/000000/javascript.png) **JavaScript** (Node.js e front-end)  
- ![HTML5](https://img.icons8.com/color/48/000000/html-5.png) **HTML5**  
- ![CSS3](https://img.icons8.com/color/48/000000/css3.png) **CSS3**  
- ![MySQL](https://img.icons8.com/ios-filled/50/000000/mysql-logo.png) **SQL (MySQL)**  

---

## ⚙️ Funcionalidades e Métodos
- **CRUD completo**: Create, Read, Update e Delete de personagens  
- **Validação de formulários** para garantir integridade dos dados  
- **Integração com API externa** do Genshin Impact  
- **Tradução automática** de informações da API  
- **Organização de rotas** separando cadastro, consulta e API  
- **Interface responsiva** via Bootstrap 4  

---

## 🖼️ Páginas do Projeto

### 1️⃣ Tela Inicial (`inicial.html`)  
- **Função:** Portal principal do sistema, conecta todas as funcionalidades  
- **Print:**  
![Tela Inicial](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Welcome.PNG)

---

### 2️⃣ Cadastro de Personagem (`formulario.html`)  
- **Função:** Criar personagens com atributos detalhados e Confrmação de cadastro 
- **Prints:**  
![Cadastro 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character01.PNG)  
![Cadastro 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character02.PNG)  
![Cadastro 03](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character03.PNG)
![Cadastro 04](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character04.PNG)
![Confirmação](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character05_registration_confirmation.PNG)
![Cadastro 06](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character06_check_registration.png)

---

### 3️⃣ Consulta de Personagens (`tabelaCadastrados.html`)  
- **Função:** Visualizar personagens cadastrados  
- **Prints:**  
![Consulta 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Check_registration01.PNG)  
![Consulta 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Check_registration02.PNG)

---

### 4️⃣ Integração com API (`personagensAPI.html`)  
- **Função:** Exibir personagens via API externa com tradução automática  
- **Print:** *(sem print fornecido)*

---

### 5️⃣ Equipe de Desenvolvimento (`equipeDesenvolvimento.html`)  
- **Função:** Apresenta integrantes, funções e responsabilidades  
- **Prints:**  
![Equipe 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_development_team01.PNG)  
![Equipe 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_development_team02.PNG)

---
 
### 6️⃣ Descrição do Projeto (`descricao.html`)  
- **Função:** Explica objetivos, tecnologias e funcionalidades  
- **Print:**  
![Descrição](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Description01.PNG)
![Descrição](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Description02.PNG)

---

## 🔗 Estrutura do Projeto


=======


---

## ⚡ Considerações Finais
Este projeto combina **desenvolvimento web full-stack**, integração com **APIs externas** e manipulação de **banco de dados**, proporcionando uma **experiência completa de criação e gerenciamento de conteúdo**. É um exemplo de aplicação prática dos conceitos ensinados na disciplina de **Programação Web II**, com foco em usabilidade, organização e desempenho.


