# UpdateNodeJS

- Sobre update no NodeJS (Unix) -

Globalmente:
sudo npm cache clean -f
sudo npm install -g n (esse n é um alias)
sudo n stable ou sudo n specificVersion

*** Para testar:
node -v


Via nvm(Node Version Manager)
nvm install version

Caso exista mais de uma versão do node instalada via nvm, você poderá alternar entre elas. Para isso, basta executar o comando nvm use version.

Cola do nvm:
- nvm ls-remote: lista as versões do node a partir do repositório remoto;

- nvm ls(list): lista as versões do node localmente para o usuário;

- nvm use version: alterna entre as versões instaladas através do gerenciador de versões do node;

- nvm alias default version: define uma versão com default. Interessante notar que, para propagar a versão default no MacOS Catalina, foi necessário fechar o terminal. Só então o terminal da IDE conseguiu rodar o script a partir da versão definida com default.

- nvm uninstall version: desinstala uma versão gerida pelo Node Version Manager.

*** Curiosidade:

Observei que ao fazer o update do node global via sudo npm install -g n (e os demais comandos listados no início deste pequeno artigo), ao concluir foi exibido a seguinte saída:

installed : v13.14.0 to /usr/local/bin/node
active : v13.14.0 at /Users/nomeUsuário/.nvm/versions/node/v13.14.0/bin/node
