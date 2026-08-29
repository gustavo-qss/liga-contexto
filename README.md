# Engenharia de contexto — liga-api

Material da disciplina de agentes de IA (UniFil, 2026). O aluno informa a
matrícula, recebe uma das dez variantes de três artefatos deliberadamente
inchados — o **prompt** da tarefa, o **AGENTS.md** do projeto e uma **skill** —
e decide, trecho a trecho, o que cortar, o que manter e o que reescrever,
justificando cada decisão.

O projeto descrito nos artefatos é a `liga-api`: uma API de campeonato de
e-sports em Node puro, sem dependências. A tarefa dos artefatos é a
classificação do campeonato, que de propósito ainda não existe no código.

## O que este site é

Uma página estática. Não há servidor, não há banco e nada sai do navegador:
o trabalho de cada aluno fica no `localStorage` da máquina em que ele digita, e
a entrega sai como um arquivo `.md` que o aluno baixa e envia pelo Classroom.

O trabalho feito na aula presencial veio junto, em `dados/sementes.js`: quem
começou lá continua exatamente de onde parou ao informar a mesma matrícula.

## Sobre os dados da turma

Nenhuma matrícula é publicada. A lista traz apenas um resumo de 8 dígitos
derivado do número (FNV-1a) e o nome com os sobrenomes reduzidos a inicial —
o bastante para o aluno se reconhecer na confirmação, e nada além disso.
O `robots.txt` e a meta `noindex` mantêm a página fora dos buscadores.

## Como republicar

Na pasta da aula, com as respostas novas em `site/respostas/`:

    node publicar.js          # remonta esta pasta a partir da versão da sala
    git -C publicacao commit -am "atualiza"
    git -C publicacao push
