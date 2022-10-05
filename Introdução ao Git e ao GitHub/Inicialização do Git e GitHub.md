

## INICIALIZAÇÃO DE CHAVE SSH NO GITHUB E AGENT



No site __GitHub__ vá em Settings e busque por: SSH Keys gere uma chave.

**GitBash **

Terminal para compatibilização do sistema de operação.

No __GitBash__ : Comando para a geração de chave:

`ssh-keygen -t ed25519 -C email@gmail.com`

Pede para inserção de uma senha e confirme.

No diretório local haverá a chave pública (*esta que será usada no GitHub*) e a chave privada.

Navegar até o local (.ssh) e “abrir” o arquivo .pub

`cat id_ed25519.pub` (enter)

Vai mostrar a chave pública(começa no ssh!), copiar e colocar no GitHub!



### Inicializar o SSH Agent ( encarregado de cuidar das chaves)

No __GitBash__:

`eval $(ssh-agent -s)`

resposta terminal: `agent pid 3746` (*exemplo de n°*)

Sempre na pasta .ssh!!

`ssh-add id_ed25519`   (*chave privada*)

Vai pedir a senha (*a mesma que foi criada no GitBash anteriormente*)

resposta terminal: `Identity added: …`



Desta forma é possível clonar repositório a partir da aba ssh, mesmo a partir de um repositório privado.

No __GitBash__:

`git clone` ( *e colar o caminho ssh gerado no GitHub*)

vai aparecer uma mensagem, assim você confirma digitando  `yes`

### Passos importantes para a utilização do Git com GitHub

##### Iniciar o Git

`git init`  (Deve ser iniciado com o GitBash na pasta definida ou pode ser iniciado clicando com o botão direito do mouse e utilizar no menu suspenso o **Git Bash Here**)

Iniciar o versionamento

`git add`

Criar um commit

`git commit`

*Obs: No terminal sempre se coloca o nome do programa na frente e o comando depois.*

##### configurar o email e o  nome para registro no commit


git config -- global user.email “email@email.com”

git config -- global user.name NomeNome


