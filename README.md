# softwaretestbook

Este repositorio é um prototipo de notebook para os conteudo da disciplina IF811 - Testes ministrada por Marcelo d'Amorim.

o conteúdo deste notebook é geradoa com o suporte do [Jupyter Books](https://jupyterbook.org)

## Arquivos de configuração da pagina
- `_config.yml` contem informacoes sobre titulo, autores e logo
- `_toc.yml` e a tabela de conteudo dos livros (table of contents), nela esta a estrurua de capitulos e secoes
- `/capitulos/` contem os diretorios numeros respectivamente com cada capitulo
- `/capitulos/numero_do_capitulo` contem um arquivo `conteudo.md` que tem as informacoes iniciais do capitulo
- `/capitulos/numero_do_capitulo/secao` contem arquivos com conteudo de cada secao

### Instruções para adição de conteúdo à página

- Primeiro execute o comando `pip3 install -r requirements.txt` para adicionar as dependências do projeto
- Após isso, basta alterar os arquivos presentes nos diretórios do padrão `/chapters/numero_do_capitulo/*.md` para modificar o conteúdo desejado no seu respectivo capítulo
- Feitas as alterações execute `jupyter-book build ./` para construir os indexes atualizados baseados no conteúdo atual



 