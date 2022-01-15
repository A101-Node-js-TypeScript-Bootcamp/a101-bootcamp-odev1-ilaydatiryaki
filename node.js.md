# NodeJS ile server ayağa kaldırmak

``` let  http = require('http');     // http modulü import edildi
const  server = http.createServer(function (req, res) {     // server oluşturuldu
res.write('Hello World!');
res.end();
})

server.listen(3000, () => {        // server localhost:3000'de ayağa kaldırıldı 
console.log("Server Ayağa kaldırıldı!")
})

```

# NodeJS ve Express kullanarak server ayağa kaldırmak

Terminalde npm i express komutu kullanılarak express modülü indirilir ve kurulur.

``` const express = require("express");  // express modülü import edildi
const app = express();               // express modülü app'e atandı

const port = 3000;   // server'in ayağa kaldırılacağı port atandı

app.get("/), (req, res) => {   // localhost:3000'e gelen GET isteği
res.send("Merhaba!")
})

app.listen(port, () => {     // server localhost:3000'de ayağa kaldırıldı
console.log(`Server ${port} portunda ayağa kaldırıldı`)
})

```













