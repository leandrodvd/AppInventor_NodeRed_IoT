# AppInventor_NodeRed_IoT
Um projeto de exemplo que mostra como construir uma aplicação Android usando o MIT AppInventor, NodeRed e Watson IoT Platform

O objetivo da aplicação é ler os dados de temperaturas enviados por um device através da Watson IoT Platform e enviar comandos para ligar ou desligar um led no device

De forma geral este projeto serve como base para qualquer projeto em que se queira receber e enviar dados de/para um dispositivo através da Watson IoT Platform.

Uma característica interessante deste projeto é que todos os módulos são cosntruídos visualmente com o NodeRED e o MIT App Inventor, de forma que não é necessário sólido conhecimento em programação.


# Executando esta solução

1. Cria uma instância no Bluemix do boilerplate [Internet of Things Platform Starter](https://console.bluemix.net/catalog/starters/internet-of-things-platform-starter/)
2. Acesse sua instância de node-red e importe o conteúdo do arquivo [nodered/iot_flow.json](https://github.com/leandrodvd/AppInventor_NodeRed_IoT/blob/master/nodered/iot_flow.json)
3. (opcional) acesse o nó de Twitter e configure com suas credenciais do Twitter
4. Acesse o [MIT App Inventor](http://ai2.appinventor.mit.edu) e selecione a opção de importar um projeto ( Import project (.aia) from my computer ) e importe o arquivo [appinventor/IoTConnect.aia](https://github.com/leandrodvd/AppInventor_NodeRed_IoT/blob/master/appinventor/IoTConnect.aia)

## Referências

MIT App Inventor: http://appinventor.mit.edu

Node Red Starter @ IBM Bluemix: https://console.bluemix.net/catalog/starters/node-red-starter

Node Red: https://nodered.org/
IBM Watson IoT Platform: https://internetofthings.ibmcloud.com/
