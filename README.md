# PC Book - Java

![The complete gRPC course](https://dev-to-uploads.s3.amazonaws.com/i/11r59di6zlyxf6g8o4s9.png)


O aplicativo PC book
PC book é um aplicativo para gerenciar e pesquisar configurações de laptop. Ele fornece 4 APIs de gRPC:

Crie um novo laptop: gRPC unário

Esta é uma API RPC unária que permite ao cliente criar um novo laptop com algumas configurações específicas.

A entrada da API é um laptop e retorna o ID exclusivo do laptop criado.

O ID do laptop é um UUID e pode ser definido pelo cliente ou gerado aleatoriamente pelo servidor, se não for fornecido.

Pesquise laptops com algumas condições de filtragem: gRPC de streaming de servidor

Essa é uma API RPC de streaming de servidor que permite ao cliente procurar laptops que atendam a algumas condições de filtragem, como preço máximo, núcleos mínimos, frequência mínima da CPU e RAM mínima.

A entrada da API são as condições de filtragem e retorna um fluxo de laptops que satisfazem as condições.

Carregar um arquivo de imagem de laptop em pedaços: gRPC de streaming de cliente

Esta é uma API RPC de streaming de cliente que permite ao cliente fazer upload de 1 arquivo de imagem de laptop no servidor. O arquivo será dividido em vários pedaços de 1 KB e serão enviados ao servidor como um fluxo.

A entrada da API é um fluxo de solicitação, que pode ser:

Metadados da imagem (apenas a 1ª solicitação): que contém o ID do laptop e o tipo de imagem (ou extensão de arquivo) como .jpgou .png.
Ou um pedaço de dados binários da imagem.
O tamanho total da imagem não deve exceder 1 MB.

A API retornará uma resposta que contém o ID da imagem carregada (UUID aleatório gerado pelo servidor) e o tamanho total da imagem.

Classifique vários laptops e recupere a classificação média de cada um deles: gRPC com transmissão bidirecional

Essa é uma API RPC de fluxo bidirecional que permite ao cliente avaliar vários laptops, cada um com uma pontuação entre 1 e 10, e recuperar a pontuação média de classificação para cada um deles.

A entrada da API é um fluxo de solicitações, cada uma com um ID de laptop e uma pontuação.

A API retornará um fluxo de respostas, cada uma contendo um ID de laptop, o número de vezes que o laptop foi classificado e a pontuação média classificada.

O curso completo do gRPC
Se você está criando APIs para seus microsserviços ou aplicativos móveis, definitivamente deseja experimentar o gRPC. É super rápido, de tipo forte e você não precisa mais escrever muitos códigos padrão para a comunicação de serviços. Graças ao impressionante HTTP / 2 e ao Protocol Buffer!

Este é um curso 4 em 1, no qual você aprenderá não apenas o gRPC, mas também o desenvolvimento de buffer de protocolo e back-end com Go e Java. Os códigos deste curso são de nível de produção, com estrutura e testes de unidade bem organizados.

O que você aprenderá:
O que é gRPC, como funciona, por que devemos usá-lo e onde é adequado.
O incrível protocolo HTTP / 2 no qual o gRPC se baseia.
Compare o gRPC com o REST.
Escreva e serialize mensagens de buffer de protocolo usando Go + Java.
Defina serviços gRPC com buffer de protocolo e gere códigos Go + Java.
Implemente 4 tipos de gRPC usando Go + Java: unário, streaming de servidor, streaming de cliente e streaming bidirecional.
Lidar com prazo de contexto, erros de gRPC e códigos de status Escreva aplicativos de nível de produção com interfaces e testes de unidade para serviços de gRPC.
Existem requisitos ou pré-requisitos do curso?
Você só precisa ter habilidades básicas de programação em Go ou Java.
ESCOLA TECNOLÓGICA - Do noob ao profissional
Na Tech School, acreditamos que todos merecem uma educação boa e gratuita. O objetivo da Tech School é dar a todos a chance de aprender TI, oferecendo tutoriais gratuitos e de alta qualidade e cursos de codificação no Youtube.

Novos vídeos são enviados toda semana. Os tópicos de vídeo são abrangentes e adequados para diversos níveis de conhecimento técnico: do novato ao profissional. O mais importante é: todo o conteúdo criado pela Tech School é gratuito e sempre será gratuito.

Se você gosta dos vídeos e deseja nos apoiar com essa visão, compartilhe, assine ou faça uma doação . Isso nos daria muita motivação para criar coisas mais úteis para a comunidade. Obrigado!