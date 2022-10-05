### Passo a passo mais simples para utilização do Git com GitHub

- Criar um repositório no site do GitHub.

- Pode ser criado junto ao repositório o README em arquivo markdown.

- Copiar o link https do repositório no GitHub.

- No seu computador procurar ou criar uma pasta para receber os arquivos do GitHub.

- Com o botão direito clicar em Git Bash Here e iniciar o GitBash na pasta selecionada.

- Utilizar o comando: git clone (e colar o link).

- Pode ser que peça alguma autenticação caso seja o primeiro acesso ou por algum outro fator.
- Não esquecer de entrar no repositório `cd repositorio`  na `main`
- `git status` para verificar se está tudo ok

#### Após haver criações e modificações dentro da pasta

- `git status` para verificar assim será possível perceber que houve modificações dentro da pasta

- `git add .`  ou `git add -A`  para adicionar todos os arquivos ao controle de versão local

- `git status` já vão aparecer os arquivos prontos 

- `git commit -m "mensagem"` para criar o commit para as alterações e deixar uma mensagem sobre as alterações

- `git status` já vão aparecer agora os arquivos prontos para o envio para o repositório do GitHub

- `git push origin main` agora vão ser enviados todos os commits locais







