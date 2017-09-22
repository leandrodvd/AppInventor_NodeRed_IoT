# AppInventor_NodeRed_IoT
Um projeto de exemplo que mostra como construir uma aplicação Android usando o MIT AppInventor, NodeRed e Watson IoT Platform

O objetivo da aplicação é ler os dados de temperaturas enviados por um device através da Watson IoT Platform e enviar comandos para ligar ou desligar um led no device

De forma geral este projeto serve como base para qualquer projeto em que se queira receber e enviar dados de/para um dispositivo através da Watson IoT Platform.

Uma característica interessante deste projeto é que todos os módulos são construídos visualmente com o NodeRED e o MIT App Inventor, de forma que não é necessário sólido conhecimento em programação.


# Executando esta solução

1. Cadastra-se gratuitamente no [bluemix.net](http://bluemix.net) caso ainda não possua um cadastro
2. Cria uma instância no Bluemix do boilerplate [Internet of Things Platform Starter](https://console.bluemix.net/catalog/starters/internet-of-things-platform-starter/) (
3. Acesse sua instância de node-red e importe o conteúdo do arquivo [nodered/iot_flow.json](https://github.com/leandrodvd/AppInventor_NodeRed_IoT/blob/master/nodered/iot_flow.json)
4. (opcional) acesse o nó de Twitter e configure com suas credenciais do Twitter
5. Acesse o [MIT App Inventor](http://ai2.appinventor.mit.edu) e selecione a opção de importar um projeto ( Import project (.aia) from my computer ) e importe o arquivo [appinventor/IoTConnect.aia](https://github.com/leandrodvd/AppInventor_NodeRed_IoT/blob/master/appinventor/IoTConnect.aia)
6. Atualize a propriedade URL dos components WebGetTemperatura e WebPostLed para a URL da sua aplicaçao criada no passo 2. Exemplo:
    
    WebGetTemperatura = https://NOMEDASUAAPP.mybluemix.net/temperatura
    WebPostLed = https://NOMEDASUAAPP.mybluemix.net/temperatura

7. Selecione a opção Build> App (Provide QR code for .apk) e use o QR Code gerado para baixar e instalar a aplicação em um dispositivo Android.
8. Publique dados de temperatura no tópico /temperatura da sua organização criada na IoT Platform
9. Receba eventos "on" e "off" no tópico /led

# Exemplo de código para dispositivo NodeMCU
O arquivo [nodemcu/nodemcu_iot.ino](https://github.com/leandrodvd/AppInventor_NodeRed_IoT/blob/master/nodemcu/nodemcu_iot.ino) contém o código para ser executado em um dispositivo nodemcu com um sensor de temperatura conectado. Para utilizá-lo, atualize as credencias da sua organização IoT Platform e carregue este código em um dispositivo nodemcu.

## Referências

IBM Watson IoT Platform: https://internetofthings.ibmcloud.com/

Internet of Things Platform Starter https://console.bluemix.net/catalog/starters/internet-of-things-platform-starter/

MIT App Inventor: http://appinventor.mit.edu

Node Red Starter @ IBM Bluemix: https://console.bluemix.net/catalog/starters/node-red-starter

Node Red: https://nodered.org/


