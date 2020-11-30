## Lazy Loading Nedir?

Lazy Loading, sayfada yer alan bir ögenin ihtiyaç duyulmadığı takdirde çağrılmaması prensibi ile çalışır yani bir nesne örneğinin gerçekten ihtiyaç duyulacağı ana kadar alınmaması ve bekletilmesi amacıyla kullanılır. Bu yöntemde veriler sorguya bağlı olarak çekilir ve veri setinin içindeki tüm dataları yüklemek yerine kullanılacağı an tekrar sorgu atar ve veriyi çeker.

### Avantaj/Dezavantajları

Lazy loading ile birbiriyle ilişkili olan entityler ihtiyaç oldukça çekilir. Bu da bize içinde bulunduğumuz case’e göre performans açısından yarar sağlayabilir. Eager loading’e göre veritabanına çok daha fazla kez bağlanır ve sorgu atar bunun da program için bir maliyeti vardır. Eager loading ise tek sorguda gerekli bilgileri elde eder.
Lazy loading ve Eager loading arasındaki çalışma hızı farkını değerlendirecek olursak, lazy loadingin tekrar tekrar database’e bağlanması sebebiyle hızı kayıt sayısı arttıkça eager loadingin üzerine çıkıyor.

## SQLite Nedir?
SQLite kullanımı ve kurulumu oldukça basit olan bir veritabanı kütüphanesidir.
* SQLite’ın çalışması için herhangi bir sunucuya ihtiyacı olmadığı için, kurulum ve ya konfigürasyon adımları yoktur.
* Her veritabanı için sadece bir dosya vardır. Bu da veritabanının yedeklenmesini ve kopyalanmasını kolaylaştırır.
* Platform bağımsızdır.
* SQLite kompakttır. Tüm kütüphanenin boyutu 225kb’dır. Bazı özellikler çıkartılarak, bu boyut 170kb’a kadar indirilebilir. Bu sayede embedded ve ya symbian gibi platformlar için uygundur.
