# js8callapi
Unofficial reference for js8call API

## События

**PING** - формируется каждые 15 секунд
|параметр|комментарий|
| ----------- | ----------- |
|_ID|id события|
|NAME|JS8Call|
|VERSION|2.2.0|
|UTC|метка времени|

---
**RIG.FREQ** - формируется при смене диапазона

---
**LOG.QSO**

---
**RX.ACTIVITY**

---
**RX.DIRECTED**

---
**RX.DIRECTED.ME**

---
**RX.SPOT**

---
**RIG.PTT**

---
**TX.FRAME**

---
**STATION.STATUS**


## Команды

**RIG.GET_FREQ** - запрос текущей частоты
|параметр|комментарий|
| ----------- | ----------- |
|_ID|id запроса|

**RIG.FREQ** - ответ на команду **RIG.GET_FREQ**

|параметр|комментарий|
| ----------- | ----------- |
|_ID|id запроса|
|FREQ|частота несущей+смещение канала, Гц|
|DIAL|частота несущей, Гц|
|OFFSET|смещение канала, Гц|

---
**RIG.SET_FREQ** - смена текущей частоты
|параметр|комментарий|
| ----------- | ----------- |
|_ID|id запроса|
| DIAL | частота несущей, Гц *|
| OFFSET | смещение канала, Гц *|

---
**STATION.GET_CALLSIGN** - запрос текущего позывного
|параметр|комментарий|
| ----------- | ----------- |
|_ID|id запроса|

**STATION.CALLSIGN** - ответ на команду **STATION.GET_CALLSIGN**
|значение|ПОЗЫВНОЙ|
| ----------- | ----------- |

|параметр|комментарий|
| ----------- | ----------- |
|_ID|id|

---
**STATION.GET_GRID**

**STATION.GRID** - ответ на команду **STATION.GET_GRID** 

---
**STATION.SET_GRID**

**STATION.GRID** - ответ на команду **STATION.SET_GRID**

---
**STATION.SET_INFO**

**STATION.INFO** - ответ на команду **STATION.SET_INFO**

---
**STATION.GET_STATUS**

**STATION.STATUS** - ответ на команду **STATION.GET_STATUS**

---
**STATION.SET_STATUS**

**STATION.STATUS** - ответ на команду **STATION.SET_STATUS**

---
**RX.GET_CALL_ACTIVITY**

**RX.CALL_ACTIVITY** - ответ на команду **RX.GET_CALL_ACTIVITY**

---
**RX.GET_CALL_SELECTED**

**RX.CALL_SELECTED** - ответ на команду **RX.GET_CALL_SELECTED**

---
**RX.GET_BAND_ACTIVITY**

**RX.BAND_ACTIVITY** - ответ на команду **RX.GET_BAND_ACTIVITY**

---
**RX.GET_TEXT**

**RX.TEXT** - ответ на команду **RX.GET_TEXT**

---
**TX.GET_TEXT**

**TX.TEXT** - ответ на команду **TX.GET_TEXT**

---
**TX.SET_TEXT**

**TX.TEXT** - ответ на команду **TX.SET_TEXT**

---
**TX.SEND_MESSAGE**

---
**MODE.GET_SPEED**

**MODE.SPEED** - ответ на команду **MODE.GET_SPEED**

---
**MODE.SET_SPEED**

**MODE.SPEED** - ответ на команду **MODE.SET_SPEED**

---
**INBOX.GET_MESSAGES**

**INBOX.MESSAGES** - ответ на команду **INBOX.GET_MESSAGES**

---
**INBOX.STORE_MESSAGE**

**INBOX.MESSAGE** - ответ на команду **INBOX.STORE_MESSAGE**

---
**WINDOW.RAISE**
