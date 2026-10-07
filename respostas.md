# Respostas · Avaliação Prática de Docker · ViaSerra Transportes (Turma C)

Nome: Bernardo Henrique Silva Corte
Matrícula: 26174736
Usuário do GitHub: bh2731
Usuário do Docker Hub: bh2731

Responda com as suas palavras e com o que aconteceu na SUA máquina. Resposta curta e certa vale mais
do que texto longo copiado. Resposta que contradiz o seu próprio Dockerfile vale zero.

## Parte 1 · Dockerfile do portal

1. Qual imagem base você usou e qual o tamanho final da imagem do portal (saída de `docker images`)?

Usei nginx. Já o tamanho final da imagem do portal foi 21 MB em CONTENT SIZE.

2. Em qual pasta do container o Nginx procura os arquivos do site? Mostre o comando que você usou para
   conferir que o `index.html` está lá dentro.

O nginx procura os arquivos em "/usr/share/nginx/html/" e o comando é: "docker exec teste-portal ls -l /usr/share/nginx/html/"

## Parte 2 · Docker Hub

3. Nome completo da imagem publicada e link público do repositório no Docker Hub.
bh2731/viaserra-portal:1.0-26174736 e https://hub.docker.com/r/bh2731/viaserra-portal


4. Se você mudar o HTML, quais comandos precisa rodar para que a versão nova chegue ao Docker Hub?
Depois de salvar a alteração no html, preciso reconstruir a imagem e mandar novamnete ao docker hub com: "docker build -t bh2731/viaserra-portal:1.0-26174736 ./portal" e "docker push bh2731/viaserra-portal:1.0-26174736"

## Parte 3 · Página de manutenção

5. Preencha uma linha por defeito encontrado. Defeito inexistente listado aqui desconta pontos.

| # | Instrução | O que estava errado | O que você viu acontecer | Como corrigiu |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |

6. Qual a diferença entre `-p 7042:80` e `-p 80:7042` no `docker run`? Qual dos dois números é a porta do container?

## Parte 4 · Primeiro docker-compose

7. Escreva os dois comandos `docker run` que fariam o mesmo que o seu `docker-compose.yml`.

8. Qual comando derruba os dois containers de uma vez?

## Verificador

9. Código de conclusão impresso pelo verificador:

```
(cole aqui)
```
