# Carimbos de data/hora da discórdia
Os carimbos de data/hora do Discord podem ser úteis para especificar uma data/hora em vários fusos horários de usuários. Eles trabalham com o formato Unix Timestamp e podem ser postados por usuários regulares, bem como bots e aplicativos.

[O Epoch Unix Time Stamp Converter](https://www.unixtimestamp.com/) é uma boa maneira de gerar rapidamente um carimbo de data/hora. Para os exemplos abaixo, usarei o carimbo de data/hora `1543392060`, que representa `28 de novembro de 2018` às `09:01:00` horas para meu fuso horário local (GMT+0100 Central European Standard Time).

## Formatação

|Estilo|Entrada|Saída (relógio de 12 horas)|Saída (relógio de 24 horas)
|--|--|--|--
|Padrão|`<t:1543392060>`|28 de novembro de 2018 9h01|28 de novembro de 2018 09h01
|Tempo Curto|`<t:1543392060:t>`|9:01 AM|09:01
|Muito tempo|`<t:1543392060:T>`|9:01:00 AM|09:01:00
|Data abreviada|`<t:1543392060:d>`|28/11/2018|28/11/2018
|Data longa|`<t:1543392060:D>`|28 de novembro de 2018|28 de novembro de 2018
|Data/hora curta|`<t:1543392060:f>`|28 de novembro de 2018 9h01|28 de novembro de 2018 09h01
|Data/hora longa|`<t:1543392060:F>`|Quarta-feira, 28 de novembro de 2018 09:01|Quarta-feira, 28 de novembro de 2018 09:01
|Tempo Relativo|`<t:1543392060:R>`|3 anos atrás|3 anos atrás

Se sua saída é de 12 ou 24 horas, depende da configuração de idioma do Discord. Por exemplo, se você tiver o idioma do Discord definido como `Inglês, EUA 🇺🇸`, obterá uma saída de 12 horas. Se o seu idioma do Discord estiver definido como `Inglês, Reino Unido 🇬🇧`, você receberá uma saída de 24 horas.

Fontes:

[Portal do desenvolvedor do Discord](https://discord.com/developers/docs/reference#message-formatting-timestamp-styles)

[Ferramentas de Dan](https://www.unixtimestamp.com/)

## LEIA ANTES DE COMENTAR

Percebo que este se tornou o primeiro resultado de pesquisa no google quando você pesquisa "Discord Timestamps", então entendo todos os tipos de usuários que vêm aqui com perguntas.

No entanto, sou apenas um desenvolvedor novato e *não sou afiliado ao Discord de forma alguma*. Sugiro fazer sua pergunta no [Official Discord Developer Server] (https://discord.gg/discord-developers) se você for um desenvolvedor ou consultar a documentação do Discord.

Se você é um usuário regular do Discord procurando gerar um carimbo de data/hora, [sesh.fyi](https://sesh.fyi/) tem uma [ferramenta criada especificamente](https://sesh.fyi/timestamp/) para o que provavelmente é exatamente o que você está procurando.
