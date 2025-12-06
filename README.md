🛥️ Sistema de Contato + Área Administrativa

Projeto acadêmico desenvolvido para a disciplina de Desenvolvimento Web, contendo:

Página de contato com envio de mensagens via API.

Área administrativa com autenticação.

Página de mensagens com leitura, visualização e exclusão.

Armazenamento local de mensagens utilizando localStorage.

📁 Estrutura do Projeto
/projeto
│── index.html
│── aluguel.html
│── destinos.html
│── tripulacao.html
│── contato.html
│── admin.html
│── mensagens.html
│
├── js/
│   ├── jquery-3.6.4.min.js
│   └── api.js
│
├── css/
│   └── default.css
│
└── images/
    ├── barco1.png
    └── barco2.png

📌 1. Funcionalidades Implementadas
✅ Página Contato (contato.html)

Formulário com campos:

Nome

Email

Mensagem

Criação do objeto mensagem conforme exigido:

{
  nome: "...",
  email: "...",
  mensagem: "..."
}


Envio utilizando inserirMensagem(mensagem) da API do professor.

Limpeza do formulário após envio.

Confirmação de sucesso ao usuário.

📌 2. Área Administrativa (admin.html)

Formulário com e-mail e senha.

Autenticação utilizando:

validarUsuario(objLoginSenha)


Objeto obrigatório:

{
  email: "...",
  senha: "..."
}

✔ Credenciais válidas:

email: admin@admin.com

senha: 1234

Resultado:

Sucesso → Redireciona para mensagens.html

Erro → Exibe mensagem “E-mail e Senha inválidos”

📌 3. Página de Mensagens (mensagens.html)

Funcionalidades implementadas:

✔ Obter mensagens da API:
obterMensagens()

✔ Salvar mensagens localmente:

Usando:

localStorage.setItem('mensagens_salvas')

✔ Exibir mensagens em tabela dinâmica:

Nome

Email

Mensagem

Ações (Ler / Excluir)

✔ Destacar mensagens não visualizadas:

Negrito = não visualizada

Normal = visualizada

Controle usando:

localStorage.setItem('vista_indice')

✔ Botões:

✔ Lida → marca mensagem como visualizada

❌ Excluir → remove mensagem do localStorage

Ambos com confirmação via confirm().

✔ Atualiza automaticamente a cada 30 segundos.
📌 4. Requisitos do Professor (Checklist)
Requisito	Status
Importar jQuery + api.js em todas as páginas	✔️
Enviar mensagem usando inserirMensagem()	✔️
Autenticação com validarUsuario()	✔️
Exibir mensagens usando obterMensagens()	✔️
Tabela dinâmica	✔️
Salvar mensagens no localStorage	✔️
Destacar mensagens não lidas	✔️
Botões de excluir e visualizar com confirmação	✔️
Redirecionar admin -> mensagens	✔️
🛠️ Tecnologias Utilizadas

HTML5

CSS3

JavaScript

jQuery

localStorage

API fictícia fornecida pelo professor

🚀 Como Executar

Baixe ou clone o repositório:

git clone https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git


Abra o projeto em um navegador (não precisa de servidor).

Acesse as páginas:

/contato.html → Enviar mensagens

/admin.html → Login

/mensagens.html → Gerenciar mensagens

📸 Layout

O projeto utiliza o layout padrão presente nos HTMLs fornecidos pelo professor, com estilos unificados nas páginas admin, contato e mensagens.

👨‍🏫 Autor

Projeto desenvolvido como atividade prática para fins acadêmicos.
