# 🎮 Genshin Impact Web II Project 
  
## 📌 Objetivo do Projeto
Este projeto foi desenvolvido como **atividade final da disciplina Programação Web II** (IFRO - Ji-Paraná) com o objetivo de aplicar de forma prática os conceitos aprendidos durante o semestre.  

O sistema permite o **cadastro, consulta e gerenciamento de personagens do jogo Genshin Impact**, utilizando dados inseridos pelo usuário e informações obtidas via **API externa**.  

Demonstra conhecimentos em **desenvolvimento web full-stack**, integração com **banco de dados MySQL**, consumo de **APIs externas** e boas práticas de **validação e usabilidade**.

---

## 🏫 Disciplina
**Programação Web II** — Aplicação prática de conceitos avançados de desenvolvimento web, incluindo:

- Node.js  
- HTML5 & CSS3  
- JavaScript  
- Bootstrap 4  
- Integração com banco de dados relacional e APIs externas  

---

## 🛠️ Ferramentas e Tecnologias Utilizadas

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

## ⚙️ Funcionalidades e Métodos
- **CRUD completo**: Create, Read, Update e Delete de personagens  
- **Validação de formulários** para garantir integridade dos dados  
- **Integração com API externa** do Genshin Impact  
- **Tradução automática** de informações da API  
- **Organização de rotas** separando cadastro, consulta e API  
- **Interface responsiva** via Bootstrap 4  

---

# Explicação Detalhada do Código do Projeto Genshin Impact Web II

---

## 🔹 Conexão com Banco de Dados

- **`mysql.createConnection`**  
  Cria uma conexão direta com o **banco de dados MySQL**.

- **`host`, `user`, `password`, `database`**  
  Informações necessárias para acessar o banco.

- **`connection.connect`**  
  Testa e estabelece a conexão; se houver erro, o programa lança uma exceção.

- **`console.log`**  
  Confirma visualmente que a conexão foi estabelecida.

```sh
const connection = mysql.createConnection({
   host: 'localhost',
   user: 'root',
   password: 'root',
   database: 'genshin_impact'
});

connection.connect((err) => {
    if(err) throw err;
    console.log('Conexão com o MySQL estabelecida');
});
```

## 🖼️ Páginas do Projeto

### 1️⃣ Tela Inicial (`inicial.html`)  
- **Função:** Portal de boas-vindas, introduz o projeto e conecta as funcionalidades principais.  
- **Print:**  
![Tela Inicial](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Welcome.PNG)

---

### 2️⃣ Tela Home (`home.html`)  
- **Função:** Centraliza o acesso às funcionalidades principais: cadastro, consulta e integração com API.  
- **Prints:**  
![Home](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Home.PNG)  
![Home Menu Consulta](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Home_menu_query.png)  
![Home Menu Cadastro](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Home_register_menu.png)

---

### 3️⃣ Cadastro de Personagem (`formulario.html`)  
- **Função:** Criar personagens personalizados com atributos detalhados.  
- **Prints:**  
![Cadastro 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character01.PNG)  
![Cadastro 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character02.PNG)  
![Cadastro 03](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character03.PNG)  
![Cadastro 04](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character04.PNG)  
![Confirmação](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character05_registration_confirmation.PNG)  
![Cadastro 06](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_registration_character06_check_registration.png)

---

### 4️⃣ Consulta de Personagens (`tabelaCadastrados.html`)  
- **Função:** Visualizar personagens cadastrados no banco de dados.  
- **Prints:**  
![Consulta 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Check_registration01.PNG)  
![Consulta 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Check_registration02.PNG)

---

### 5️⃣ Integração com API (`personagensAPI.html`)  
- **Função:** Exibir personagens do Genshin Impact via API externa com tradução automática.  

---

### 6️⃣ Equipe de Desenvolvimento (`equipeDesenvolvimento.html`)  
- **Função:** Apresentar os integrantes do projeto, funções e responsabilidades.  
- **Prints:**  
![Equipe 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_development_team01.PNG)  
![Equipe 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_development_team02.PNG)

---

### 7️⃣ Descrição do Projeto (`descricao.html`)  
- **Função:** Explicar objetivos, tecnologias utilizadas e funcionalidades implementadas.  
- **Prints:**  
![Descrição 01](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Description01.PNG)  
![Descrição 02](https://github.com/WasgtonGomes/Genshin_WebII_Project/blob/main/Prints/Page_Description02.PNG)

---

## ⚡ Considerações Finais
Este projeto combina **desenvolvimento web full-stack**, integração com **APIs externas** e manipulação de **banco de dados**, proporcionando uma **experiência completa de criação e gerenciamento de conteúdo**. É um exemplo de aplicação prática dos conceitos ensinados na disciplina de **Programação Web II**, com foco em usabilidade, organização e desempenho.

---

## 🔗 Estrutura do Projeto

```sh
Genshin_WebII_Project/
├── 📂 public/               # Arquivos públicos acessíveis via navegador
│   ├── 📂 CSS/              # Folhas de estilo
│   │   ├── descricao.css
│   │   ├── equipeDesenvolvimento.css
│   │   ├── formulario.css
│   │   ├── geral.css
│   │   ├── inicial.css
│   │   ├── menu.css
│   │   ├── personagensAPI.css
│   │   └── tabela.css
│   ├── descricao.html
│   ├── equipeDesenvolvimento.html
│   ├── formulario.html
│   ├── geral.html
│   ├── inicial.html
│   ├── personagensAPI.html
│   └── tabelaCadastrados.html
│
├── 📂 Prints/               # Prints das telas do sistema
│   ├── Page_Welcome.PNG
│   ├── Page_Home.PNG
│   ├── Page_Home_menu_query.png
│   ├── Page_Home_register_menu.png
│   ├── Page_registration_character01.PNG
│   ├── Page_registration_character02.PNG
│   ├── Page_registration_character03.PNG
│   ├── Page_registration_character04.PNG
│   ├── Page_registration_character05_registration_confirmation.PNG
│   ├── Page_registration_character06_check_registration.png
│   ├── Page_Check_registration01.PNG
│   ├── Page_Check_registration02.PNG
│   ├── Page_development_team01.PNG
│   ├── Page_development_team02.PNG
│   ├── Page_Description01.PNG
│   └── Page_Description02.PNG
│
├── 📂 node_modules/         # Dependências do Node.js
├── server.js                # Servidor principal em Node.js
├── server2.js               # Versão alternativa de servidor
├── package.json             # Configuração do projeto Node.js
├── package-lock.json        # Detalhes das dependências
├── banco de dados Genshin impact.sql   # Script do banco MySQL
├── Dados completos api genshim impact.png
├── destbord genshim impact.png
└── README.md                # Documentação do projeto
```


