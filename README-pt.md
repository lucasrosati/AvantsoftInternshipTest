
# Avantsoft Processo Seletivo de Estágio

Avantsoft Internship Test, which consisted of consuming an API with PHP and displaying a frontend paginated table with 5 pages, each one containing 10 users.

## Funcionalidades
- Consumir uma API que retorna um arquivo .JSON e exibi-lo em uma tabela paginada em HTML.
- Temas dark e light

**index.php**

O arquivo index.php é responsável por exibir uma lista de usuários e implementar a paginação. Ele faz o seguinte:

1) Obtém os dados dos usuários de uma API externa usando a função file_get_contents() e json_decode(). Os dados são armazenados na variável $data.
2) Verifica se existem dados na variável $data usando !empty($data).
3) Se houver dados disponíveis, a variável $users é definida com a matriz de usuários obtidos.
4) Define a quantidade de usuários por página e calcula o número total de páginas com base no número total de usuários.
5) Verifica a página atual usando $_GET['page'] ou define a primeira página como padrão.
6) Calcula os índices de início e fim para exibir os usuários corretos na página atual.
7) Usa a função array_slice() para obter apenas os usuários da página atual.
8) Exibe os usuários em uma tabela HTML usando um loop foreach.
9) Exibe os links de paginação para navegar entre as páginas.




**style.css**

O arquivo style.css contém as regras de estilo CSS para a aparência da página. Ele define várias regras de estilo, incluindo:

1) Alinhamento de texto centralizado para o cabeçalho e células da tabela.
2) Configuração do corpo (body) para ocupar a largura e altura total da tela e usar flexbox para centralizar o conteúdo verticalmente.
3) Estilos para o botão de alternar tema escuro, incluindo a aparência do botão e a mudança de cores do tema.
4) Estilos para a tabela, incluindo bordas, cores de fundo e cores de texto.
5) Estilos para a paginação, incluindo margem superior e aparência dos links.






## Instalação

Como usar:

Para usar o código fornecido, você precisará ter um ambiente de desenvolvimento local configurado com um servidor web (por exemplo, Apache) e PHP instalados.

Para baixar e instalar o Apache Server, você precisa instalar o XAMPP, para isto, use o site oficial deles: https://www.apachefriends.org/

1) Crie um novo diretório no seu servidor web local.
2) É recomendável usar o /XAMPP/htdocs/"diretoriocriado"
3) Salve o arquivo index.php no diretório recém-criado.
4) Crie um novo arquivo chamado style.css e copie o código CSS fornecido para esse arquivo.
5) Salve o arquivo style.css no mesmo diretório que o arquivo index.php.
6) Inicie o servidor web local.
7) Abra um navegador da web e acesse o endereço local correspondente ao diretório onde você salvou os arquivos (por exemplo, http://localhost/meudiretorio/).

8) Ao seguir essas etapas, você deverá ver a página de usuários com a lista de usuários e a paginação exibidas corretamente. Você também poderá alternar entre o tema claro e o tema escuro clicando no botão de alternância de tema.
    
## Autor

- [@lucasrosati](https://www.github.com/lucasrosati)

