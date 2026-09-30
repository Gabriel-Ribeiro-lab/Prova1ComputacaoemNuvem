# Prova 1 de Computação em Nuvem

Gabriel Ribeiro de Oliveira

RA: a4dcc893a8bccc186920

## O que fiz
Executei uma página web em um contêiner Docker chamado reservas.
Usei a imagem nginx:alpine e a porta 8086 do ambiente.

## Verificação do conteinêr

CONTAINER ID   IMAGE          COMMAND                  CREATED          STATUS          PORTS                                     NAMES
b5f1a8a070ed   nginx:alpine   "/docker-entrypoint.…"   48 seconds ago   Up 48 seconds   0.0.0.0:8086->80/tcp, [::]:8086->80/tcp   reservas

## Teste da Página

<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Reservas</title>
/head>
<body>
<h1>Reservas abertas</h1>
</body>
</html>

## Explicação

Explicando cada um:

imagem nginx:alpine é o modelo usado para criar o contêiner, com o Nginx em uma versão leve do Alpine Linux.
Contêiner reservas é a instância em execução criada a partir dessa imagem, onde a minha página está sendo executada.
mapeando a porta 8086 do computador para a porta 80 do contêiner. Assim, ao acessar localhost:8086, eu chego ao serviço na porta 80 dentro do contêiner
