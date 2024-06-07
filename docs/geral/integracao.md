# Integração
O presente documento tem como objetivo explicitar como ocorrerá a integração entre os subsistemas. Para isso, foi dividido nas seguintes seções: Estrutura e Eletrônica, Estrutura e Energia, Energia e Eletrônica, e, por fim, Software e Eletrônica.


# Estrutura e energia

# Estrutura e eletrônica

# Energia e eletrônica

# Software e eletrônica

Como definido na arquitetura, a comunicação entre o Software e eletrônica está sendo feito a partir da entrada serial. Com isso, a aplicação em Electron se comunicará com o Arduíno pela entrada USB conectada diretamento no computador, sendo a conexão bidirecional, isto é, tanto o arduíno recebe sinais da aplicação, como a aplicação também recebe sinais do Arduíno.

Assim, a comunicação é dividida em dois pontos, a inicialização do processo de escaneamento e a comunicação das medições do Sensor infravermelho.

## Inicialização
Para que o arduíno possa começar a fazer o processo de medição, ele precisará receber um sinal da aplicação, chamando assim, o loop de escaneamento.

Com isso o código para a comunicação é dividido no envio da mensagem pela aplicação e no recebimento dessa informação:

- Envio da mensagem: A aplicação deve instânciar um Port, definindo o baudRate, em seguida, chama um port.write com a mensagem a ser mandada ao Arduíno.

-Recebimento da mensagem: Após instânciar o Serial, faz a leitura dessa mensagem até identificar o fim da mensagem, ao receber a mensagem de início, se chama o código para leitura;

## Medição do Sensor
Para fazer o processo de escaneamento e processamento da nuvem de pontos, os dados coletados pelo arduíno devem ser transmitidos para a aplicação, esse processo é mais simples, sendo necessário apenas que a aplicação leia o que o Arduíno está implimindo na entrada serial, usando o Serial.println(), na aplicação, após instânciar o port, podemos usar o parser-readline para ler os dados da entreda serial, assim recebendo os dados e processando-os como necessário na aplicação.


# Tabela de versionamento
|Versão| Data | Responsável | Descrição|
|------|------|-------------|----------|
| 0.1 | 07/06/2024| Carla R. Cangussú | Esqueleto do documento|
| 0.2 | 07/06/2024| Artur de Sousa | Adicionado integração software e eletrônica|