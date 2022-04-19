
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

## Lateinit nedir?
Bir değişken oluşturmanız gereken ancak değişkenin bildirilmesi/oluşturulması sırasında değerini belirmek istemediğiniz durumlarda null hatası almamak için lateinit kullanılmaktadır. Bu sayede değişkenin değeri kullanım sırasında atanabilir. 
## Lateinit Neden Kullanılır?
Lateinit sadece var olan değişkenlerde kullanılır.Lateinit tanımlanan değişkenler Non-Null bir değişkendir. Hem Non-Null olarak tanımlanır hem de değer ataması yapılmaz. Bu değişkeni herhangi bir yerde, tanımlama yapmadan kullanmaya çalışırsak Kotlin  “UninitializedPropertyAccessException” hatası verecektir. Lateinit sayesinde Kotlin bu değişkeni Non-Null olarak görmektedir.  Bu şekilde Nullsafe yapılmış olunur ve hata oranını azaltır.
Aşağıdaki örnekte olduğu gibi variable lateinit olarak tanımlanmış, değeri atanmamıştır. Daha sonra değeri verilmesine rağmen, lateinit olarak tanımlandığı için null hatası alınmamıştır.Aksi takdirde kodumuzda null hatası alınacaktı. 

```bash
lateinit var person1:Person
fun main(args: Array<String>) {
    person1 = Person("Ted",28)
    print(person1.name + " is " + person1.age.toString())
}


  
```
