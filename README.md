# 📝 To-Do List 

Uma aplicação de **lista de tarefas (To-Do List)** desenvolvida com **React**, permitindo adicionar, concluir e excluir tarefas de forma simples e interativa.

O projeto utiliza **React Hooks**, **Styled Components**, **React Icons** e **UUID** para criar uma interface dinâmica e organizada.

---

## 🎯 Sobre o Projeto

O projeto consiste em uma lista de tarefas onde o usuário pode:

* ✍️ Adicionar novas tarefas
* ✅ Marcar tarefas como concluídas
* 🗑️ Excluir tarefas
* 📋 Visualizar as tarefas cadastradas
* 💬 Exibir uma mensagem quando não existem tarefas

Cada tarefa recebe um **ID único**, permitindo que as operações de conclusão e exclusão sejam realizadas individualmente.

---

## 🚀 Funcionalidades

* ➕ Adicionar tarefas
* ✅ Finalizar e desfazer tarefas concluídas
* 🗑️ Remover tarefas
* 🆔 Identificação única para cada tarefa
* 🎨 Alteração visual das tarefas concluídas
* 📭 Mensagem para lista vazia
* 🖱️ Interação através de ícones
* ⚛️ Gerenciamento de estado com React

---

## 🛠️ Tecnologias Utilizadas

* **React** — Construção da interface e gerenciamento de estado
* **JavaScript** — Lógica da aplicação
* **Styled Components** — Estilização dos componentes
* **React Icons** — Ícones de conclusão e exclusão
* **UUID** — Geração de identificadores únicos

---

## ⚛️ React Hooks

O projeto utiliza o Hook `useState` para controlar os estados da aplicação.

### Lista de tarefas

```javascript
const [list, setList] = useState([])
```

Responsável por armazenar todas as tarefas adicionadas pelo usuário.

### Campo de entrada

```javascript
const [inputTask, setInputTask] = useState('')
```

Responsável por armazenar o conteúdo digitado no campo de texto.

---

## ➕ Adicionando Tarefas

Ao clicar no botão **Adicionar**, uma nova tarefa é criada contendo:

```javascript
{
    id: uuid(),
    task: inputTask,
    finished: false
}
```

Cada tarefa possui:

* `id` → Identificador único da tarefa
* `task` → Texto da tarefa
* `finished` → Define se a tarefa foi concluída

---

## ✅ Concluindo Tarefas

A função responsável por finalizar uma tarefa utiliza `map()` para percorrer a lista e localizar a tarefa através do seu ID.

Quando encontrada, a propriedade `finished` é alterada:

```javascript
finished: !item.finished
```

A estilização do item também muda de acordo com esse estado, permitindo identificar visualmente quando uma tarefa foi concluída.

---

## 🗑️ Excluindo Tarefas

Para remover uma tarefa, o projeto utiliza o método `filter()`:

```javascript
const newList = list.filter(item => item.id !== id)
```

Dessa forma, a tarefa correspondente ao ID selecionado é removida da lista.

---

## 🎨 Estilização

A interface foi desenvolvida utilizando **Styled Components**, permitindo criar componentes estilizados diretamente no JavaScript.

Entre os elementos estilizados estão:

* Container principal
* Lista de tarefas
* Campo de entrada
* Botão de adicionar
* Itens da lista
* Ícone de exclusão
* Ícone de conclusão
* Mensagem de lista vazia

A interface utiliza um fundo em gradiente, cards para as tarefas e diferentes cores para representar o estado dos itens.

---

## 📂 Estrutura do Projeto

```text
📁 Primeiro-projeto-react
│
├── 📁 public
│
├── 📁 src
│   ├── 📄 App.jsx
│   ├── 📄 globalStyles.js
│   ├── 📄 main.jsx
│   └── 📄 style.js
│
├── 📁 .github
│   └── 📁 workflows
│       └── 📄 deploy.yml
│
├── 📄 .gitignore
├── 📄 eslint.config.js
├── 📄 index.html
├── 📄 package.json
├── 📄 package-lock.json
└── 📄 vite.config.js
```

---

## 📚 O que foi praticado

Durante o desenvolvimento deste projeto, foram praticados conceitos importantes de **React e JavaScript**, como:

* Componentes React
* `useState`
* Renderização condicional
* Renderização de listas com `map()`
* Manipulação de arrays
* `filter()`
* Eventos
* Funções
* Props
* Operador spread
* Desestruturação de objetos
* Identificadores únicos com UUID
* Styled Components
* React Icons
* Manipulação dinâmica da interface

---

## 🎯 Objetivo

O objetivo do projeto foi praticar os fundamentos do **React**, principalmente o gerenciamento de estados e a criação de uma interface interativa.

O projeto também permitiu aplicar conceitos de JavaScript em uma aplicação prática, trabalhando com **arrays, funções, eventos e atualização dinâmica da interface**

---

## 👨‍💻 Autor

**Rian Lucas**

Desenvolvedor Front-End sempre evoluindo...

---

## 🔗 Link do Projeto

https://riannlucass.github.io/Primeiro-projeto-react/

---

