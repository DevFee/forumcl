## Notas:

- 1 - **Copie apenas o arquivo html porque você vai ter que criar os arquivos de css para renderiza-los dps**

- 2 - **Crie uma pasta public e dentro dela um arquivo de foto com o nome de "fotouser.jpg", para renderizar a foto de usuarios**

- 3 - **Importante alterar os valores do head do html (caminho do arquivo de saida css etc..)**

- 4 - **Faça o processo de iniciar o tailwind abaixo para que o navegador leia o css! Caso não queira, copie o arquivo "styles.css" na pasta src.**

- 5 - **Caso copie o arquivo de css importante deixar ele no mesmo caminho do html "./src/styles.css".**

## Tecnologias:

> - HTML
> - TailwindCSS
> - Typescript
> - Prisma ( **_Vai ser adicionado ainda_** )

## Iniciar renderização tailwind:

- 0 - caso não tenha o node instale-o na sua máquina
  > nodejs.org/en/
- 1 - No terminal do vscode instale o tailwind
  > npm i tailwindcss
- 2 - No terminal do vscode inicie o tailwind
  > npx tailwindcss init
- 3 - Config do arquivo do tailwind:
  > /\*_ @type {import('tailwindcss').Config} _/
  >
  > module.exports = {
  >
  > content: **["Aqui você coloca o caminho do seu index.html"]**,
  >
  > theme: {
  >
  > extend: {},
  >
  > },
  >
  > plugins: [],
  >
  > }
- 4 - Crie um arquivo chamado **"input.css"** e cole o seguinte código:
  > @tailwind base;
  >
  > @tailwind components;
  >
  > @tailwind utilities;
- 5 - Feito isso vamos rodar o comando para que o tailwind interprete o arquivo de input e crie um novo. Troque o nome dos valores do comando abaixo pelo oque se indica nele:
  > npx tailwindcss -i **caminho/arquivo/input.css** -o **./caminho/do/arquivo/de/saida.css** --watch
- 6 - Por fim apenas linke o arquivo de saida css no head do html.
  > link href="caminho/do/arquivo/de/saida.css"
