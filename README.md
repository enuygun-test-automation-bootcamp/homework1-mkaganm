# Homework1

-
    1) Sınıfları kullanırken implement ve extend ile çağırabiliyoruz. İkisini aynı anda kullanınca hangisi önce
       yürütülür ?
-
    2) Internal ne olduğu araştırılacak.
-
    3) Abstraction ne olduğu araştırılacak ve abstractiona örnek bir kod yazılacak.

## 1

### :pushpin: Hem Extend Hem Implement Etmek

Bir class sadece bir class'ı extend edebilir.
Ancak aynı anda bir class’ı extend edip bir veya
daha fazla interface'i implement edebilir.
Çünkü ’extends’ keywordünün aksine, 'implements'
demek yoluyla bir class'ın aldığı hiç bir şey yoktur.
Sadece bazı method’ları
implement etmeyi taahüt etmektedir.
Bir A class’ı hem B classını extend edebilir hem
de C inetrface'ni implement edebilir.

``` Java
    public class A extends B implements C{
        // ...
    }
```

Bunu yaparken extend'i implement'ten önce tanımlamak
gerekir.
Herhangi bir sayıda interface implement edilebilir
fakat virgül ile ayrılmalıdır.

Bu durumda extend daha önce yürütülür.

## 2

### :pushpin: Internal

Javada internal in olmadığını gördüm. Ancak benzer
kullanım için aşağıya bulduğum örneği bırakıyorum.

[ÖRNEK](http://www.javacamp.org/javavscsharp/internal.html)

## 3

### :pushpin: Abstract

Inheritance ile bir üst class tanımlayabiliyorduk,
burda özelliklerimiz ve metodlarımız olabiliyordu.
Alt classları burdan türeterek bu özellikleri ve
metodları miras alabiliyorduk.
Interface ile gövdesiz metodlarımızı yazıyorduk ve
bunu implement eden tüm alt classlarda bunları
kendimize göre yazabiliyorduk.

**Abstract classlar inheritance ve interface
classların birleşimi gibi düşünülebilir. Abstract
classlarda özelliklerimizi, metodlarımızı
yazabiliyoruz. Ve aynı zamanda gövdesiz metodlarımızı
yazabiliriz.**