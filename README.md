**RESUMO**

O projeto envolveu a criação de um bot do Telegram para ler e armazenar mensagens de um grupo. O principal objetivo era aplicar conhecimentos em AWS e computação em nuvem. O Google Colab foi utilizado para escrever os códigos e várias ferramentas da AWS foram empregadas na implementação do projeto.

O bot do Telegram foi configurado para ler as mensagens do grupo e o armazenamento das mensagens foi realizado através do API Gateway. As mensagens foram armazenadas no S3 à medida que chegavam. Após a limpeza dos dados, as mensagens foram novamente armazenadas no S3, desta vez separadas por dias em arquivos Parquet.

Para realizar o armazenamento e a limpeza dos dados, o Lambda foi utilizado, onde códigos específicos para cada tarefa foram implementados. Para automatizar o processo e garantir que os códigos fossem executados sempre no mesmo horário, o EventBridge foi utilizado.

Um dos principais desafios enfrentados durante a implementação deste projeto foi trabalhar com arquivos Parquet, um formato com o qual não havia experiência prévia. No entanto, após estudo e prática, o desafio foi superado.

Embora a análise de dados não fosse o foco principal do projeto, uma análise simples dos dados coletados foi realizada. Isso incluiu a quantidade de mensagens por dia, a quantidade de mensagens por usuário por dia, a média do tamanho das mensagens por usuário por dia e a quantidade de mensagens por hora por dia da semana.
