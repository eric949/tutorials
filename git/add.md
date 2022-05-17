[Voltar](../readme.md)

## add

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
Podemos ainda adicionar todos os arquivos com extenções parecidas, por exemplo, caso queira adicionar todos os arquivos com extenções .cs e .csproj, poderá usar o seguinte comando:
```
git add Folder/\*.cs*
```
Ou então podemos usar '*' para adicionar todos os arquivos que contenham uma palavra. Segue exemplo (neste exemplo serão adicionados todos os arquivos que começam com 'log-' com a extenção '.txt')
```
git add log-*.txt
```
Quando um arquivo ou pasta estão marcados como ignorado no .gitignore, podemos forçar eles a serem adicionados usando o parametro --force, segue exemplo:
```
git add --force *.cache
```