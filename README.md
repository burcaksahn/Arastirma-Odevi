
## İsim Alanı (namespace) Nedir?
Java’da olduğu gibi Kotlin’de de paket (package) yapısı bulunmaktadır. Paket yapısının amacı kodumuzu farklı isim alanlarına(name space) bölebilmemize olanak sağlayarak özellikle büyük projelerimizde kod okunabilirliğini arttırmaktır. Aynı amaca hizmet eden özellikleri, sınıfları ve fonksiyonları bir çatı altında toplarken, bu çatıya verdiğimiz isime isim alanı (namespace) denir.  Bir namespace içerisine birbiriyle alakalı sınıf ve foksiyonlar koyulmalıdır.Tools namespace yapılan tasarımda aynı isimli elementler içerilebilir. Bu tür durumlarla çakışmayı önlemek için namespace kullanılabilir. Bu sayede tasarımdaki son değişikler geliştirme yapılırken anında görülebilir.
## Namespace neden önemlidir?
Büyük projelerde, ekip halinde geliştirilen uygulamalarda isimleri standart halde tutmak ve kod okunabilirliğini sağlamak zordur.    Bu karmaşıklığı önlemek için, benzer özellikte işleve sahip kod blokları, bir namespace altında toplanmış ve kullanılmak istenilen sınıfa ait namespace kod sayfasına eklendikten sonra kullanılabilir hale gelmiştir.



```bash
  package geometri.sekiller
class Dikdortgen(val yukseklik: Int, val uzunluk: Int)
{ 
}

```
