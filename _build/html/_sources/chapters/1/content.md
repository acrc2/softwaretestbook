# softwaretestbook

Este repositorio é um prototipo de notebook para os conteudo da disciplina IF811 - Testes ministrada por Marcelo d'Amorim.

o conteúdo deste notebook é geradoa com o suporte do [Jupyter Books](https://jupyterbook.org)

## Arquivos de configuração da pagina
- `_config.yml` contem informacoes gerais da página 
- `_toc.yml` arquivo onde são definidos os diretorios com os conteúdos de cada página como também a disposição delas no menu

### Formato de configuração do `_toc.yml` 

Na pasta chapters estão os arquivos '.md' onde serão adicionados os arquivos que irão compor cada página

Para configurar a navegação da página usamos os prefixos
```
   - file: 
   para criar uma pagina advinda de um arquivo
   - file: chapters/2/content
   - file: chapters/3/content
     sections: 
     - file: chapters/3/sections/newSubject
     - file: chapters/3/sections/otherSubject
```
- `/capitulos/` contem os diretorios numeros respectivamente com cada capitulo
- `/capitulos/numero_do_capitulo` contem um arquivo `conteudo.md` que tem as informacoes iniciais do capitulo
- `/capitulos/numero_do_capitulo/secao` contem arquivos com conteudo de cada secao

<<<<<<< HEAD
## Instruções para adição de conteúdo à página
=======
### Instruções para adição de conteúdo à página
>>>>>>> 21a8f3628f51e73e981343d3a0791e8853e6f11c

- Primeiro execute o comando `pip3 install -r requirements.txt` para adicionar as dependências do projeto
- Após isso, basta alterar os arquivos presentes nos diretórios do padrão `/chapters/numero_do_capitulo/*.md` para modificar o conteúdo desejado no seu respectivo capítulo
- Feitas as alterações execute `jupyter-book build ./` para construir os indexes atualizados baseados no conteúdo atual
<<<<<<< HEAD
 
=======
>>>>>>> 21a8f3628f51e73e981343d3a0791e8853e6f11c
