# Git Basics

## git add

### Descrição:
Este comando permite adicionar os arquivos que serão commitados na próxima etapa.

### Parâmetros

Normalmente usado com o parametro '.' para adicionar todos os arquivos que foram modificados naquela branch.
Além desse parâmetros podemos informar determinadas pastas, arquivos ou extensões. Segue respectivos exemplos:
```
git add Folder/
git add File.cs
git add *.cs
```
Podemos também adicionar todos arquivos com determidada extenção dentro de uma pasta, usando:
```
git add Folder/\*.cs
```
Ou então arquivos que contenham algo na palavra, como por exemplo:
```
git add log-*.txt
```
Quando um arquivo ou pasta estão marcados como ignorado no .gitignore, podemos forçar eles a serem adicionados usando o parametro --force, segue exemplo:
```
git add --force *.cache
```