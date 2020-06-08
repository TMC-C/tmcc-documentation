1. Kloonaa https://github.com/rage/tmc-vscode

2. Lisää tiedostoon tmc-vscode/src/config/constants rivit:

```export const TMC_API_URL = "http://tmc-server.westeurope.cloudapp.azure.com/api/v8/";```

```export const ACCESS_TOKEN_URI = "http://tmc-server.westeurope.cloudapp.azure.com/oauth/token";```

(korvaa näillä vanhat ```TMC_API_URL``` ja ```ACCESS_TOKEN_URI``` arvot)

3. Asenna [npm](https://nodejs.org/en/download/) jos koneellasi ei ole.

4. tmc-vscode -kansiossa ```npm install```

5. tmc-vscode -kansion sisältävässä kansiossa (yhden matalampi taso) ```code tmc-vscode```

6. vscoden sisällä F5 ja odota. Uusi vscode-ikkuna aukeaa ja lokaali versio tmc-pluginista pitäisi olla käytössä

7. Kirjaudu, lataa tehtävät jne.
