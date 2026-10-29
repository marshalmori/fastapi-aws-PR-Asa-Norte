# fastapi-aws

## Comando para executar o projeto

uvicorn api.main:app --reload

• main: É o nome do seu arquivo Python (ex: main.py).

• app: É o nome da variável dentro do arquivo que recebe a instância do FastAPI (ex: app = FastAPI()).

• --reload: Indica que o servidor deve reiniciar automaticamente sempre que um arquivo for alteração.

## Como fazer o push em sua conta do GitHub

### Passo 1 — Verificar o repositório remoto atual

git remote -v

O resultado provavelmente será semelhante a:

origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git (fetch)
origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git (push)

### Passo 2 — Criar um repositório vazio no GitHub do aluno

Você deve acessar o GitHub e criar um novo repositório. Preferencialmente, sem inicializá-lo com README, .gitignore ou licença.

### Passo 3 — Alterar o endereço remoto

git remote set-url origin https://github.com/USUARIO-ALUNO/REPOSITORIO-ALUNO.git

Substitua o endereço pelo repositório criado pelo aluno.

### Passo 4 — Enviar o projeto

git push -u origin main

Se a branch principal tiver outro nome, como master, o comando deverá usar esse nome. 2. Alternativa: remover o vínculo original
Se preferir, o aluno pode remover o endereço remoto original e cadastrar o novo:

git remote remove origin

git remote add origin https://github.com/USUARIO-ALUNO/REPOSITORIO-ALUNO.git

git push -u origin main

Isso mantém os arquivos e o histórico de commits existentes, mas altera o destino dos próximos envios.
