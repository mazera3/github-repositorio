# Gerenciar github pelo terminal linux
- Acessar o [github](https://github.com/) e criar uma conta de `usuario`.
- Após logado, criar um repositório. Procure pela opção "+ New repository".
- Na próxima página adicione o nome do seu repositório (exemplo: "teste"). As configurações deixe padrão. 
- Feito isso encontre a opção "Create repository" e clique.
- Anote a linha que contém: git remote add origin https://github.com/`usuario`/teste.git

# No terminal Linux
- No diretório "/home/`usuario`", rode os seguintes comandos: 
  - git config --global user.email "email-que-usou-pra-criar-a-conta-do-github"
  - git config --global user.name "nome-do-seu-usuario-de-login-do-github"
  - criaremos um diretório para alocar todos os repositórios do projetos: `mkdir PROJETOS-GIT`
  - Entre neste diretório:: `cd PROJETOS-GIT`
  - criaremos um diretório para alocar o repositório que tínhamos criado anteriormente no site: `mkdir TESTE`
  - Entre no diretório: `cd TESTE`

  #  Utilizando o Git 
  - Para gerar as configurações: `git init`
  - Para criar o README.md: `echo "teste" >> README.md`
  - Para adicionar um arquivo: `git add README.md` ou todos: `git add .`
  - Criar um "commit": `git commit -m "primeiro teste"`
  - O endereço do github: `git remote add origin https://github.com/usuario/teste.git`
  - Ver estado: `git status`
  - Enviar pra o repositório como master: `git push -u origin master`
    - Vai pedir o nome do usuário que usa pra logar no GitHub e a senha. 
    - Recarregue aquela página no navegador, e veja se aconteceu as alterações. 
  - Toda vez que adicionar ou alterar algo rode: `git status`

  # Administrar alterações
  - git status && git add . &&  git commit -m "qualquer-coisa" && git push -u origin master
