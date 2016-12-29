# jqueryValidate
Ideal para validar formulários, e utilizar em aplicações web como e-commerce, portais entre outros.

# Como Utilizar

1° Adicionar entre as tags <body></body> no final de todos os códigos html do seu site, para melhor versionamento e carregamento.

    <script src="js/jquery-3.1.1.min.js"></script>
    <script src="js/jquery.validate.min.js"></script>
    
2° Acrescentar a tag name="" nos inputs que irão ser captados os valores digitados pelo usuário.

    <input type="password" name="senha" id="senha" class="form-control" placeholder="Digite sua senha">

3° Inicializar o documento Jquery na tag <script></script>

   $(function(){
        $("#form-cadastro").validate({
            rules : {
                senha : {
                    required : true,
                    minlength : 6
                }
            },
            messages : {
                senha : {
                    required : "Informe uma senha.",
                    minlength : "A senha deve possuir pelo menos 6 caracteres."
                }
            }
        });
    });
    
4° Debugar e efetuar testes com a biblioteca.    
    
    
    
