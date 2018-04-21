# Yemekspeti İsim ile Filtreleme (Tampermonkey eklentisi)

Sadece seçtiğiniz anahtar kelimelere sahip restoranların görüntülenmesi sağlar. Bazı kelimeleri ise kara listeye alabilirsiniz.

## Yükleme adresi

[https://greasyfork.org/en/scripts/40895-yemeksepeti-i-sim-ile-filtreleme/](https://greasyfork.org/en/scripts/40895-yemeksepeti-i-sim-ile-filtreleme/)

Tarayıcınızda [Tampermonkey](https://tampermonkey.net/) ya da [Greasemonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) eklentisi kurulu olmalıdır.

## Kullanılışı

5 ve 6'ncı satırlar, scriptin hangi sayfalarda çalışacağını belirler. Bunları kendi ihtiyacınıza göre düzenleyin.
```js
// @include        http://www.yemeksepeti.com/istanbul/hisarustu
// @include        https://www.yemeksepeti.com/istanbul/hisarustu
```

15 ve 16'ncı satırları da kendinize göre düzenleyin.
```js
var MUST_CONTAIN= ["Hisarüstü", "Etiler", "Waffle"]; // Checks for at least one of them.
var MUST_NOT_CONTAIN= ["Levent"]; // This is the black list. Both lists are case sensitive.
```

## Not

Yemeksepeti ile resmi bağlantısı bulunmamaktadır.