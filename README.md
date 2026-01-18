 # 🎮 Genshin Impact Web II Project    
       
## 📌 Project Objective   
This project was developed as the **final assignment of the Web Programming II course** (IFRO – Ji-Paraná) with the goal of practically applying the concepts learned throughout the semester.   
      
The system allows **registration, consultation, and management of Genshin Impact characters**, using user-provided data and information obtained through an **external API.**  
  
It demonstrates knowledge in full-stack web development, MySQL database integration, external API consumption, and best practices related to validation and usability.

---  

## 🏫 Course
**Web Programming II** — Practical application of advanced web development concepts, including:

- Node.js   
- HTML5 & CSS3  
- JavaScript  
- Bootstrap 4  
- Integration with relational databases and external APIs  

---

## 🛠️ Ferramentas e Tecnologias Utilizadas

| Tecnologia | Ícone | Finalidade |
|------------|-------|------------|
| **Node.js** | ![Node.js](https://img.icons8.com/color/48/000000/nodejs.png) | Back-end, route management, data handling |
| **Express.js** | ![Express](https://img.icons8.com/ios/50/000000/express-js.png) | Web server framework and endpoints |
| **MySQL** | ![MySQL](https://img.icons8.com/ios-filled/50/000000/mysql-logo.png) | Relational database |
| **Axios** | ![Axios](https://img.shields.io/badge/Axios-API-blue?logo=axios&logoColor=white) | External API consumption |
| **node-fetch** | ![Node-Fetch](https://img.shields.io/badge/node--fetch-HTTP-green?logo=node.js&logoColor=white) | HTTP requests |
| **@vitalets/google-translate-api** | ![Google Translate](https://img.icons8.com/ios-filled/50/000000/google-translate.png) | Automatic data translation |
| **HTML5** | ![HTML5](https://img.icons8.com/color/48/000000/html-5.png) | Page structure |
| **CSS3** | ![CSS3](https://img.icons8.com/color/48/000000/css3.png) | Styling and layout |
| **JavaScript** | ![JavaScript](https://img.icons8.com/color/48/000000/javascript.png) | Interactivity and logic |
| **Bootstrap 4** | ![Bootstrap](https://img.icons8.com/color/48/000000/bootstrap.png) | Responsiveness and UI components |

---

## 💻 Languages

- JavaScript (Node.js e front-end)  
- HTML5  
- CSS3  
- SQL (MySQL)  

---

## ⚙️ Funcionalidades e Métodos
- **Full CRUD**: Create, Read, Update, and Delete characters  
- **Form validation** to ensure data integrity  
- **External API integration with** Genshin Impact data 
- **Automatic translation** of API information  
- **Route organization** separating registration, consultation, and API logic  
- **Responsive interface** using Bootstrap 4  

---

# Detailed Explanation of the Genshin Impact Web II Project Code

---

## 🔹 Database Connection

- **`mysql.createConnection`**  
  Creates a direct connection to the **MySQL database.**

- **`host`, `user`, `password`, `database`**  
 Required information to access the database.

- **`connection.connect`**  
Tests and establishes the connection; if an error occurs, an exception is thrown.
- **`console.log`**  
Visually confirms that the connection has been established.
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

## 🖼️ Project Pages

### 1️⃣ Welcome Page (`inicial.html`)  
- **Purpose:** Welcome portal that introduces the project and connects the main functionalities.  
- **Screenshot:**  
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


