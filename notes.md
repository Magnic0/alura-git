# Comandos Básicos

- `git init` = Inicia (cria) um repositório git no diretório atual;

- `git init --bare` = Cria um repositório sem uma cópia dos arquivos para ser utilizado como servidor;

- `git status` = Informa o estado atual do repositório;

- `git add <file>` = Adiciona arquivos para o *commit*, pode ser usado um "." no lugar do nome do arquivo para adicionar todos os arquivos presentes;

- `git remote` = Lista todos os repositórios remotos disponíveis;

- `git remote -v` = Lista todos os repositórios remotos disponíveis, assim como a sua localização;

- `git remote add <name> <link>` = Adiciona um link para um repositório remoto. Normalmente o *name* é origin;

- `git commit -m "<msg>"` = Envia a informação das alterações para o *Log*;

- `git log --oneline` = Imprime o *Log* em uma linha;

- `git log -p` = Imprime o *Log* com todos os detalhes de alterações feitas em cada *commit*;

- `git log -n <num>` = Imprime os últimos *commits* até o número especificado. Ex.: <git log -n 2> exibe os últimos 2 *commits*;

- `git diff` = Imprime a diferença entre o código no HEAD em relação ao último *commit* feito;

- `git diff <info> <info>` = Imprime de forma detalhada todas as diferenças entre os *commits* ou *branches* especificados;

- `git clone` = Clona (baixa) um repositório pela primeira vez para o local atual;

- `git push \ pull <repository> <branch>` = Envia as alterações feitas para \ baixa os arquivos atualizados de um repositório remoto especificado;

- `git tag` = Imprime todas as *tags* existentes;

- `git tag -a <version>` = Cria uma nova *tag*, podendo ser adicionada uma mensagem digitando `-m "<msg>"` logo após, na mesma linha de comando;

# Branches

- `git branch` = Imprime todas as *branchs* existentes no repositório;

- `git branch <branch_name>` = Cria uma branch com o <branch_name> especificado no repositório;

- `git checkout <branch>` = Move o **HEAD** para a branch especificada;

- `git checkout -b <branch_name>` = Cria uma branch e move o **HEAD** para a mesma;

- `git merge <branch>` = Transfere o trabalho feito em uma branch para a atual;

- `git rebase <branch>` = Une uma branch com a atual de forma a não bagunçar a ordem dos commits;

- `git branch -d <branch>` = Deleta a branch especificada caso ela já tenha sido merged com a remote branch;

# Time traveling 

- `git checkout --<file>` = Desfaz as alterações antes de fazer o *commit*;

- `git checkout <branch>` = Deixa o **HEAD** no mesmo estado da *branch* especificada;

- `git checkout <hash>` = Deixa o **HEAD** no mesmo estado do *commit* especificado;

- `git reset HEAD <file>` = Retira as alterações feitas do*commit*;

- `git reset <hash>` = Reverte alterações feitas no *commit* especificado e cria um novo informando a ação;

- `git stash` = Salva o trabalho atual para que seja acessado posteriormente;

- `git stash list` = Lista todos os *stashs* disponíveis;

- `git stash apply <stash_num>` = Aplica uma alteração específica no **HEAD**, a partir da *stash* especificada;

- `git stash drop <stash_num>` = Remove o *stash* especificado da lista;

- `git stash pop` = Aplica e remove a última alteração que foi adicionada na *stash*;
