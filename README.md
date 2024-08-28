Sistema de Gerenciamento de Biblioteca
Descrição
Este é um aplicativo de gerenciamento de biblioteca desenvolvido em Python utilizando a biblioteca Tkinter para a interface gráfica. O sistema permite o cadastro e visualização de livros e usuários, bem como a solicitação de livros pelos usuários.

Diagrama UML

Você pode criar e hospedar o diagrama UML do seu sistema e substituir "link-para-diagrama" pelo link para o diagrama.

Documentação das Classes e Métodos
Classe ItemBiblioteca
Atributos:

titulo: O título do item na biblioteca.
Classe Livro (Herda de ItemBiblioteca)
Atributos:

autor: O autor do livro.
isbn: O número ISBN do livro.
Métodos:

__init__(self, titulo, autor, isbn): Inicializa um objeto Livro com título, autor e ISBN.
Classe Usuario (Herda de ItemBiblioteca)
Atributos:

matricula: A matrícula do usuário.
Métodos:

__init__(self, nome, matricula): Inicializa um objeto Usuário com nome e matrícula.
Classe Biblioteca
Atributos:

livros: Lista de livros na biblioteca.
usuarios: Lista de usuários cadastrados.
Métodos:

adicionar_livro(self, livro): Adiciona um livro à biblioteca.
adicionar_usuario(self, usuario): Adiciona um usuário à biblioteca.
Classe GerenciadorDePedidos
Atributos:

biblioteca: Referência para a instância de Biblioteca.
pedidos: Lista de pedidos de livros.
Métodos:

solicitar_livro(self, usuario, livro): Solicita um livro para um usuário, se o livro estiver na biblioteca.
Classe BibliotecaApp
Atributos:

root: A janela principal do Tkinter.
biblioteca: Instância da classe Biblioteca.
main_frame: Frame principal da interface gráfica.
Métodos:

__init__(self, root): Inicializa a interface gráfica e configura os botões principais.
cadastro_livro(self): Exibe a tela de cadastro de livros.
cadastro_usuario(self): Exibe a tela de cadastro de usuários.
visualizar_livros(self): Exibe a tela de visualização dos livros cadastrados.
visualizar_usuarios(self): Exibe a tela de visualização dos usuários cadastrados.
voltar(self, frame): Retorna à tela principal.
Descrição das Funcionalidades
Cadastro de Livros: Permite ao usuário cadastrar um novo livro informando título, autor e ISBN. O livro é adicionado à lista de livros da biblioteca.
Cadastro de Usuários: Permite ao usuário cadastrar um novo usuário informando nome e matrícula. O usuário é adicionado à lista de usuários da biblioteca.
Visualização de Livros: Exibe todos os livros cadastrados na biblioteca, mostrando título, autor e ISBN.
Visualização de Usuários: Exibe todos os usuários cadastrados na biblioteca, mostrando nome e matrícula.
Roadmap de Execução
Inicialização: O aplicativo é iniciado com a criação da janela principal (root) e da instância de BibliotecaApp.
Tela Principal: O usuário interage com a tela principal para escolher entre as opções de cadastro e visualização.
Cadastro de Livros/Usuários: Ao selecionar as opções de cadastro, o usuário é direcionado a uma tela específica para inserir os dados e salvar as informações na biblioteca.
Visualização: Ao selecionar as opções de visualização, a aplicação exibe as informações dos livros ou usuários cadastrados.
Voltar: Permite ao usuário retornar à tela principal a partir das telas de cadastro e visualização.
Manual de Instalação e Uso
Dependências
tkinter: Para criar a interface gráfica do usuário.
Instalação
Tkinter geralmente vem pré-instalado com o Python. Se necessário, você pode instalar Tkinter usando o gerenciador de pacotes apropriado para sua distribuição Python.

Inicialização
Para iniciar o programa, execute o seguinte comando no terminal:

bash
Copiar código
python nome_do_arquivo.py
Substitua nome_do_arquivo.py pelo nome do arquivo que contém o código.

Uso
Inicie o aplicativo: Execute o script Python.
Use a Interface Gráfica: Utilize os botões disponíveis na tela principal para cadastrar livros, cadastrar usuários, ou visualizar os livros e usuários cadastrados.
