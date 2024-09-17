# Introdução ao Git - Aula 01

Bem-vindo ao breve doumento de introdução ao Git! Neste documento, nosso objetivo é fornecer uma visão clara e prática sobre o uso do Git, ajudando a aplicar essas habilidades em projetos de dados. O Git é uma ferramenta fundamental para o versionamento de código e colaboração em equipes de desenvolvimento, especialmente quando múltiplas pessoas estão trabalhando em um mesmo projeto.

## 🐧 História do Git

### História do Git:
O Git foi criado em 2005 por Linus Torvalds, o criador do kernel Linux, como uma ferramenta de controle de versão distribuído. O objetivo principal era substituir o sistema anterior, BitKeeper, após uma disputa entre a comunidade de desenvolvedores Linux e a empresa responsável pelo BitKeeper.

Ao desenvolver o Git, Torvalds tinha como principais metas:
- **Velocidade**: O sistema deveria ser rápido e eficiente, mesmo em grandes projetos.
- **Integridade dos dados**: A integridade do histórico dos arquivos deveria ser garantida.
- **Suporte a desenvolvimento distribuído**: Git foi projetado para facilitar a colaboração de vários desenvolvedores, permitindo a cada um ter uma cópia completa do repositório.

Com o tempo, o Git se tornou amplamente adotado em vários projetos de software de código aberto e em empresas, tornando-se uma das ferramentas de controle de versão mais populares no mundo.

Hoje, o Git é uma ferramenta essencial para o desenvolvimento colaborativo e é usado por milhões de desenvolvedores em projetos de todos os tamanhos.

Para entender mais sobre Git:
- [Sobre Git com Akita e Palestra de Linus Torvalds sobre Git](https://www.youtube.com/watch?v=6Czd1Yetaac)

- ## 🛠️ O Que é o Git?

O Git é um sistema de controle de versão distribuído que permite o rastreamento de mudanças em arquivos e a coordenação do trabalho entre múltiplas pessoas em um projeto de software. Criado por Linus Torvalds em 2005, o Git oferece ferramentas para que os desenvolvedores possam trabalhar de forma independente, criar e gerenciar ramificações do projeto, e mesclar as mudanças facilmente.

### Principais características do Git:
- **Controle de versão distribuído**: Cada desenvolvedor tem uma cópia completa do histórico do projeto em sua máquina, o que permite maior independência e segurança.
- **Velocidade**: Operações como commit, branch e merge são extremamente rápidas, tornando-o ideal para grandes projetos.
- **Ramificações (branches)**: Git facilita a criação e o gerenciamento de branches, permitindo que diferentes funcionalidades sejam desenvolvidas de maneira paralela e, posteriormente, mescladas ao projeto principal.
- **Integridade dos dados**: Git armazena todos os dados com verificações de integridade, garantindo que o histórico de um projeto não seja corrompido.
- **Sistema de colaboração**: Git permite que múltiplos desenvolvedores contribuam para o mesmo projeto simultaneamente, oferecendo ferramentas para resolução de conflitos e unificação de mudanças.

Hoje, o Git é amplamente utilizado tanto em projetos de código aberto quanto em ambientes corporativos, sendo um dos sistemas de controle de versão mais populares e confiáveis do mundo.

## 💻 Como Instalar o Git

### Windows
1. Baixe o Git [aqui](https://git-scm.com/download/win).
2. Execute o instalador e siga as instruções.

### Linux
1. Abra o terminal.
2. Execute: `sudo apt-get install git`

### Mac
1. Abra o terminal.
2. Execute: `brew install git`

## 🎯 Configuração do Git

Configure o nome e o e-mail do usuário:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"
```
## 📂 Níveis de Configuração do Git

Os arquivos de configuração do Git armazenam as configurações feitas com os comandos `git config` em diferentes locais, dependendo do nível de configuração:

1. **🌍 Configurações Globais (`--global`)**:
   - As configurações globais são salvas no arquivo `.gitconfig` localizado no diretório home do usuário.
   - **📍 Localização**:
     - **🐧 Linux/Mac**: `~/.gitconfig`
     - **🖥️ Windows**: `C:\Users\SeuNomeDeUsuario\.gitconfig`
   - Você pode abrir esse arquivo em um editor de texto para visualizar ou editar as configurações.

2. **🖥️ Configurações de Sistema (`--system`)**:
   - As configurações de sistema são aplicadas a todos os usuários da máquina e são armazenadas no arquivo de configuração global do sistema.
   - **📍 Localização**:
     - **🐧 Linux**: `/etc/gitconfig`
     - **🖥️ Windows**: Pode estar em um caminho como `C:\Program Files\Git\etc\gitconfig`
   - Essas configurações requerem permissões de administrador para serem alteradas.

3. **📁 Configurações Locais (por repositório)**:
   - As configurações locais são específicas para um único repositório Git e são salvas no arquivo `config` dentro da pasta `.git` do repositório.
   - **📍 Localização**:
     - No diretório do repositório Git: `.git/config`

### 🔍 Visualizar Configurações do Git

Você pode visualizar as configurações atuais usando os seguintes comandos:

- **Para ver todas as configurações globais**:
  ```bash
  git config --global --list
  ```

Esses comandos vão listar as configurações e seus valores, permitindo que você veja detalhes como o nome de usuário e o e-mail configurados para o Git.


