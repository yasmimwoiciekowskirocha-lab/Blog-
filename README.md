# Blog-
Alura 

<!DOCTYPE html> 
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Blog Tech - Yasmin</title>
    <style>
        header {
            background-color: rgb(188, 108, 247); 
            color: #FFFFFF;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
            padding: 16px;
        }

        main {
            background-color: #FFFFFF;
            color: #183C63;
            max-width: 800px;
            margin: 0 auto;
            padding: 16px; 
        }

        article {
            display: flex;
            align-items: center;
            gap: 16px;
            margin-bottom: 20px;
        }

        img {
            width: 80px;
            height: 80px;
        }

        .artigo-autor {
            font-weight: bold;
        }
        
        button {
            cursor: pointer;
            margin-right: 8px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Meu blog tech</h1>
        <p>Vou compartilhar conhecimentos sobre tecnologia e programação</p>
    </header>

    <main>
        <article>
            <img src="imagem-blog.png" alt="Logotipo conceitual de tecnologia e educacao: um livro aberto de onde emerge um cérebro digital brilhante, cercado por ícones de Wi-Fi, circuitos e lâmpada de ideia. Cores em tons de azul e branco.">
            <div>
                <h2>Meu primeiro post</h2>
                <p class="artigo-autor">Por: Marcelo Paludetto</p>
                <p>Boas-vindas ao meu novo blog! Aqui vou compartilhar dicas de programação e curiosidades da área de tecnologia.</p>
                <button>❤️ <span>0</span></button>
                <button>👍 <span>0</span></button>
            </div>
        </article>

        <article>
            <img src="imagem-blog.png" alt="Logotipo conceitual de tecnologia e educacao: um livro aberto de onde emerge um cérebro digital brilhante, cercado por ícones de Wi-Fi, circuitos e lâmpada de ideia. Cores em tons de azul e branco.">
            <div>
                <h2>Meu primeiro post</h2>
                <p class="artigo-autor">Por: Yasmin</p>
                <p>Boas-vindas ao meu novo blog! Aqui vou compartilhar dicas de programação e curiosidades da área de tecnologia.</p>
                <button>❤️ <span>0</span></button>
                <button>👍 <span>0</span></button>
            </div>
        </article>
    </main>

    <script>
        // Seleciona todos os botões da página
        const botoes = document.querySelectorAll("button");

        botoes.forEach(function(botao) {
            // Cada botão precisa ter seu próprio controle de "curtiu"
            let curtiu = false;

            botao.addEventListener("click", function() {
                let texto = botao.querySelector("span");
                
                if (curtiu === false) {
                    texto.textContent++;
                    curtiu = true;
                } else {
                    texto.textContent--;
                    curtiu = false;
                }
            });
        });
    </script>
</body>
</html>
