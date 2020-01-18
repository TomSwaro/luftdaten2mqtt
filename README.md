# luftdaten2mqtt

Script sends json sensor values coming from esp8266 luftdaten sensor via Apache web servere to a mosquitto mqtt server.
Script is based on "mqttpublish.php"   https://gist.github.com/zekizeki/3075653 
many thanks Rob : https://github.com/zekizeki

In esp8266 sensor configuration the own API has to be enabled. ("An eigene API senden") e.g. /sensor/luftdaten.php 

attached json file example:
{
"esp8267id": "123456", 
"software_version": "NRZ-2020-129", 
"sensordatavalues":[
  {"value_type":"SDS_P1","value":"7.07"},
  {"value_type":"SDS_P2","value":"3.30"},
  {"value_type":"temperature","value":"3.80"},
  {"value_type":"humidity","value":"99.90"},
  {"value_type":"samples","value":"4371736"},
  {"value_type":"min_micro","value":"32"},
  {"value_type":"max_micro","value":"20039"},
  {"value_type":"signal","value":"-74"}]
}
