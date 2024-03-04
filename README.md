Olá, esse projeto ensina você a usar o Git.

No menu Terminal, clicar na opção 'Novo terminal'.
Com o terminal aberto, digita o comando (exceto o $):
$ git init (Enter)
    Inicia um '.git' vazio com 'master' inicial. (Nomes em vez de 'master': 'main', 'trunk' e 'development'). 
    → Criar a 1ª versão: git add
    Esse comando manda os arquivos para a área de 'espera'. Deve colocar o 'nome do arquivo' na frente: 
$ git add README.md (Enter)
    Depois pode visualizar:
$ git status (Enter)
    Precisa fazer um 'commit' para o git, para salvar localmente na máquina. Acrescentar uma mensagem (-m):
$ git commit -m "Primeiro commit desse repositório!" (Enter)
    Foi feito o commit no repositório.
    Agora pode verificar usando o git status novamente:
$ git status (Enter)
    Renomear o ramo principal de 'master' para 'main':
$ git branch -M "main" (Enter)
    Agora o 'master'(mestre) foi mudado para main'(principal).
    Para enviar o repositório da máquina para o GitHub, fará git remote add origin + link (copiar e colar):
$ git remote add origin https://github.com/Everton-D-Alves/ProjetoGit.git (Enter)
    → remote é a conexão do repositório local (Git) com o repositório remoto (GitHub);
    → add (adicionar) origin (nome que está colocando para o repositório do GitHub) + link.
    Ainda não têm arquivo no GitHub, apenas conexão do Git com o GitHub. Então acrescenta mais um comando:
$ git push -u origin main (Enter)
    Após isso, aparecerá uma caixa de texto para fazer um login no GitHub.
    Ao entrar no GitHub, atualizar a página para aparecer o repositório 'ProjetoGit'.
    Fazendo o versionamento (mudança):
    Isso é uma alteração.
    Criar também um outro arquivo, exemplo, 'Projeto.md'.
    Limpar a tela do terminal: clear (+ Enter)
$ git add . (Enter)
    O ponto adiciona todas as mudanças.
$ git status (Enter)
$ git commit -m "Criação do projeto" (Enter)
    Agora fará o 'push' sem o '-u':
$ git push origin main (Enter)
    O comando 'remote' só é adicionado 1 vez.
    Limpar a tela do terminal: clear (+ Enter)
    Criar uma branch:
$ git checkout -b "novo-botao"
    Agora o nome da branch é novo-botao.
    Ao criar o arquivo botao.md, digita no terminal:
$ git add . (Enter)
$ git commit -m "Novo botão." (Enter)
    Para adicionar ao GitHub na branch ao invés de main, fará:
$ git push origin novo-botao (Enter)
    Atualizar página do GitHub. Agora têm 2 branches: main e novo-botao.
    O 'novo-botao' é uma branch (ramo) que está na frente da branch principal 'main'.
    Se quizer voltar na branch principal 'main', fará:
$ git checkout main (Enter)
    Agora pode fazer mudanças no 'main'. Para voltar no 'novo-botao', fará:
$ git checkout novo-botao (Enter)
    Agora pode desenvolver em 'novo-botao'.
    Após finalizar a branch (ramo), para juntar à branch principal (main), fará um 'merge':
$ git checkout main (Enter)
    Agora que está no 'main', acontecerá o 'merge':
$ git merge novo-botao (Enter)
    Para finalizar, fará:
$ git push origin main (Enter)
    Atualizar a página do GitHub. Verificar as mudanças.