# BRVARIO

Repositório oficial de distribuição do firmware e do aplicativo BRVARIO.

O BRVARIO é um variômetro sonoro compacto para voo livre, com conectividade
Bluetooth e configuração pelo aplicativo oficial.

## Downloads oficiais

- [Firmware mais recente para OTA](https://github.com/randalrenye/firmwarebrvario/releases/latest/download/novobrvario.ino.bin)
- [Todas as versões do firmware](https://github.com/randalrenye/firmwarebrvario/releases)
- [Aplicativo Android](BRVARIO-arm64-v8a.apk)

> O firmware OTA publicado aqui é destinado ao **BRVARIO Normal**. O BRVARIO
> E-PAPER possui firmware e processo de atualização próprios.

## Recursos principais

- Variômetro sonoro com ajuste dos limiares de subida e descida.
- Filtro Kalman ou filtro exponencial configurável.
- Pré-termal e alerta de descendência forte.
- VARIO DINÂMICO para indicar a entrada em uma nova subida.
- Modo silencioso e opção de desligar o som de descida.
- Bluetooth Low Energy com integração LK8EX1.
- Compatibilidade com XCTrack, FlySkyHy, XCSoar, Gaggle e SeeYou Navigator.
- Configuração e atualização OTA pelo aplicativo BRVARIO.
- Indicador de bateria e recursos automáticos de economia de energia.

## Versão atual

**Firmware 3.7**

O aplicativo consulta automaticamente a Release marcada como mais recente e
baixa o arquivo `novobrvario.ino.bin`.

## Atualização OTA

1. Carregue o BRVARIO acima de 30%.
2. Ligue o equipamento e conecte o BRVARIO Normal ao aplicativo.
3. Abra a opção de atualização de firmware.
4. Mantenha o telefone próximo até a conclusão e reinicialização.

Se o BLE desligar após 20 minutos sem nenhuma conexão, reinicie o BRVARIO antes
de iniciar a atualização.

## Código e propriedade intelectual

O BRVARIO é um produto proprietário e de **código fechado**. Este repositório
é utilizado somente para distribuir arquivos oficiais, documentação pública e
notas de versão. Nenhum código-fonte do firmware ou do aplicativo é publicado
aqui.

Todos os direitos são reservados. A disponibilização dos binários não concede
permissão para copiar, modificar, descompilar, redistribuir ou criar trabalhos
derivados, salvo quando autorizado expressamente pelo responsável do BRVARIO
ou permitido pela legislação aplicável.

## Documentação

- [Histórico de versões](CHANGELOG.md)
- [Política de Privacidade](PRIVACY.md)

## Contato

- Instagram: [@brvario](https://www.instagram.com/brvario/)
- E-mail: randalrenye@hotmail.com
