# Solo Miner V2
New Version Solo Miner with High Speed for mining Bitcoin With all System
---

![Solo Miner V2](https://raw.githubusercontent.com/Pymmdrza/SoloMinerV2/mainx/CaptureScreenSolo.JPG)

---

First install this package :
```
pip install binascii
pip install traceback
pip install signal
pip install requests
pip install colorama
pip install lxml
```


use this package's imported this source :

```
import binascii
import hashlib
import json
import logging
import random
import socket
import threading
import time
import traceback
from datetime import datetime
from signal import SIGINT , signal
import requests
from colorama import Back , Fore , Style
import context as ctx
```

For insert Your BTC Address Wallet in File `SoloMinerV2.py` in Line 27 Changed This Line:

```

# Changed this Address And Insert Your BTC Wallet

address = '16p9y6EstGYcnofGNvUJMEGKiAWhAr1uR8' 

``` 

for more detail's and about withdraw request follow this issue : #[SOLO.CKPOOL](https://github.com/Pymmdrza/SoloMinerV2/issues/11#issue-1507921524)

----

Programmer Telegram ID [@MrPyMmdrza](https://t.me/MrPyMmdrza)

Programmer Telegram Channel [@Cryptoixer](https://t.me/Cryptoixer)

> **Warning**
> Unfortunately, due to the ignorance of some dear users, we were not informed that some profiteers and uncultured people are selling some of my scripts at a lower price. And the user does not receive anything after payment. Some of these ignorant people give malicious and viral files to users. From here, I declare that the only official source for selling my scripts is the [website](https://mmdrza.com) and [Telegram ID](https://t.me/MrPyMmdrza) or [Telegram Channel](https://t.me/Cryptoixer).
devcontainer.json 
{
  "include": [
    "src"
  ],

  "exclude": [
    "**/node_modules",
    "**/__pycache__",
    "src/experimental",
    "src/typestubs"
  ],

  "ignore": [
    "src/oldstuff"
  ],

  "defineConstant": {
    "DEBUG": true
  },

  "stubPath": "src/stubs",

  "reportMissingImports": true,
  "reportMissingTypeStubs": false,

  "pythonVersion": "3.6",
  "pythonPlatform": "Linux",

  "executionEnvironments": [
    {
      "root": "src/web",
      "pythonVersion": "3.5",
      "pythonPlatform": "Windows",
      "extraPaths": [
        "src/service_libs"
      ]
    },
    {
      "root": "src/sdk",
      "pythonVersion": "3.0",
      "extraPaths": [
        "src/backend"
      ]
    },
    {
      "root": "src/tests",
      "extraPaths": [
        "src/tests/e2e",
        "src/sdk"
      ]
    },
    {
      "root": "src"
    }
  ]
}