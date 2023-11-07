# Apache_Solr_Sorgu
### Apache Solr da Belli Bir Tarih Aralıgındaki Verileri Getiren Sorgu
Apache Solr'da belirli bir tarih aralığındaki verileri getirmek için updatedAt alanını kullanarak bir Solr sorgusu oluşturabiliriz. Aşağıda, 2020 yılının Ocak ayından sonraki verileri getirecek bir Solr sorgusu örneği bulunmaktadır:
```
http://example/solr/core/select?q=updatedAt:[2020-01-01T00:00:00Z TO *]

```
Bu sorgu, "updatedAt" alanındaki 2020 yılı Ocak ayından sonraki tüm kayıtları getirecektir. İşte sorgunun açıklaması:

http://example/solr/core/select: Solr sorgusu için varsayılan URL.
q=updatedAt:[2020-01-01T00:00:00Z TO *]: Bu kısım, "updatedAt" alanındaki 2020 yılının Ocak ayından sonraki tarihleri içeren belgeleri seçer. [2020-01-01T00:00:00Z TO *] ifadesi, Ocak 2020'nin sonundan sonraki herhangi bir tarihi ifade eder.
Bu sorgu Solr sunucusuna gönderildiğinde, Solr bu kritere uyan belgeleri döndürecektir. Bu sorgu, belirli bir tarih aralığını sorgulamak için kullanılabilecek temel bir örnek.
