# Information Disclosure 🕵️

Information Disclousure, ou traduzindo diretamente para o português Divulgação e Informação, é uma vulnerabilidade encontrada predominantemente em aplicações WEB e consiste no vazamento de informações confidenciais do sistema.

Os danos causados por esta vulnerabilidade são diversos , já que a uma enorme possibilidade de dados vazados, ou seja, pode afetar os dois lados de uma instituição, seu sistema interno e os dados de clientes.

Sobre danos a clientes, vale destacar o vazamento em texto livre de banco de dados anexados a página e mal protegidos, listas de emails, senhas, informações de contato e credencias de login.

Quanto a infraestrutura do sistema, é importante ressaltar que os principais vazamentos estão relacionados com a disponibilização de chaves API e credenciais de sistemas de banco de dados e serviços na nuvem. Além disso, o vazamento do código fonte completo de uma funcionalidade pode conceder informação privilegiada para invasores e para concorrentes diretos da empresa.

![Untitled](Imagens/Untitled.png)

Para exemplificar esta vulnerabilidade irei utilizar o laboratório disponibilizado pela PortSwigger “**Information disclosure on debug page**”:

Inicialmente é importante compreender que a identificação desta categoria de vulnerabilidades é identificada principalmente na fase de reconhecimento e análise de um sistema. Por isso o desenvolvimento do laboratório será utilizando uma busca no código fonte da página.

Buscando o termo “.php” no código fonte da página foi possível identificar um hiperlink comentado, o qual tem um caminho para página de debug do PHP.

![Untitled](Imagens/Untitled%201.png)

Inserindo este diretório no fim do endereço da página foi possível acessar o conteúdo da página de Debug e buscando pelo termo “KEY” no código fonte é encontrado código para conclusão do laboratório.

![Untitled](Imagens/Untitled%202.png)

É possível notar que apesar de se tratar apenas de um laboratório de CTF, a busca por termos “key”, “api”, “psswd”, por exemplo, pode levar a informações no código fonte da página. Neste caso foi “esquecido” por algum responsável pelo código fonte da páina uma chave secreta em texto limpo.

![Untitled](Imagens/Untitled%203.png)
