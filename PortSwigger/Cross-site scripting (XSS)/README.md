# Cross-Site Scripting (XSS) ❌

Cross-Site Scripting (XSS) é um tipo de ataque de injeção, no qual são injetados códigos maliciosos em sites. Ocorrem predominantemente quando o atacante utiliza do navegador para enviar códigos maliciosos para seu usuário alvo. Pode estar relacionado com um ataque de engenharia social, quando busca forçar a vítima a clicar em algum link ou acessar alguma página.

Quando se trata de XSS há uma variedade enorme de ataques, podem permitir a trasnferencia de arquivos, cookies e outras informações de sessão. Esta falha pode implicar de algumas formas seu alvo e por isso foi dividida em tres sub-grupos: Refletido, armazenado e baseado no DOM.

*Armazenado:*

Neste ataque o script fica armazenado no site e permanece injetado permanentemente no servidor, como em uma página de perfil. Desta forma, a vítima retorna o código malicioso do servidor quando solicitada o armazenamento. Contem em seu escopo outro tipo, blind Cross-Site Script, caracterizda pela carga útil estar armazenada no servidor e assim é refletida pelo backend das empresas.

*Refletido:*

Este ataque consiste no script que é refletido no servidor da WEB como uma mensagem de erro, resultado de pesquisa ou qualquer outra resposta. Estes ataques na sua maioria precisam de engenharia social, para convencer o alvo de clicar no link enviado.

*Baseado no DOM:*

Nesta categoria de XSS o ataque é realizado por meio de modificações no DOM e além disso não é possível notar a payload. Geralmente consiste em um ataque do lado do cliente, e a carga maliciosa nunca é enviada ao servidor, tornando-a mais avançada e crítica.
