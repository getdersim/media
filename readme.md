# Ders.im Medya

İlgili url'e pdf url'inizi get isteği yaptığınızda sonucu console.log()'a basan html betiğidir.


*PDF TO GIF*
GET:
  https://media.ders.im/?pdf=[PDF_URL]


*PDF TO PNG*
GET:  
  https://media.ders.im/thumbnail.html?pdf=[PDF_URL]


# Kullanım

Kendi projenizde [npm pgif paketini](https://www.npmjs.com/package/pgif) kullanarak sizde aynı fonksiyonelliği sağlayabilirsiniz.

```javascript
const pgif = require('pgif')

pgif.pdf('https://gifi.cagatay.me/1.pdf').then(filename => console.log(filename))
pgif.thumbnail('https://gifi.cagatay.me/1.pdf').then(filename => console.log(filename))
```
