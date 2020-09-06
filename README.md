# Jira-Project


## Açıklama

Havelsan bünyesinde gerçekleştirmiş olduğum stajım dahilinde, çok güzel ve faydalı, mentörlüğümü yapan
ekibin de işlerini kolaylaştıran bir proje geliştirdim. Geliştirdiğim bu proje Asp Net Core Web API 
mimarisi üzerine kurulmuş olup, veritabanı olarak PostgreSQL kullanılmıştır.

Projenin ana mantığı, atlassian jira rest servislerine RestSharp kütüphanesi ile erişerek, ihtiyaç duyulan verinin çekilmesi, 
backendde ayıklanması ve veritabanına kaydedilmesi üzerine kuruludur. Frontendde ise kendi yazdığım
rest servislere istek atarak istatistiksel verileri kullanıcıya listeledim.

Frontend tarafında React.js kullandım. Backend tarafında ise, projeyi katmanlı mimari üzerine kurarak
bu standarda uymaya çalıştım. 20 işgünlük staj süresi sona erdiğinde proje tamamen bitmiş ve teslim edilmiş haldeydi.

Geliştirdiğim Projenin Kaynak Kodlarına Buradan Ulaşabilirsiniz. Proje .NET Core Platformunda, ASP .NET Core Web API mimarisi üzerine yazılmaktadır.


## Veritabanı

Veritabanını lokal bilgisayarınızda kurmak için solution içerisindeki Entities projesine girip, içerisindeki migrations
isimli klasörü siliniz. Sonrasında Asp Net Core projesinin başlangıç projesi olarak seçili olduğundan emin olduktan
sonra, package manager console'u açınız, ve entity katmanı için;

> Add-Migration InıtıalCreate

> Update-Database 


Komutlarını Giriniz. Veritabanı bilgisayarınızda kurulacaktır.


## Backend

Projenin Backend Kısmında, .Net Core SDK 3.1 Sürümü Kullanılmıştır. 

Projede Kullanılan Paket ve Kütüphaneler

- Microsoft.EntityFrameworkCore.Tools(3.1.7)
- Microsoft.EntityFrameworkCore.Design(3.1.7)
- Npgsql.EntityFrameworkCore.PostgreSQL(3.1.4)
- Microsoft.VisualStudio.Web.CodeGeneration.Design(3.1.4)
- Microsoft.AspNetCore.Cors(2.2.0.)
- Newtonsoft.Json(12.0.3)
- RestSharp(106.11.4)


## Frontend


Projenin Frontend tarafında JavaScript Kütüphanesi Olarak React.js Kullanılmıştır. Github'a pushlanmış olan
JiraReactApp dosyasını indirip Visual Code veya Başka Bir Editörde Açılması Gerekmektedir.

Bilgisayarınızda Node.js kurulu olduğundan emin olunuz.

### React.js Kurulumu

JiraReactApp Dosyasını İndirip, Visual Code İle Açılmalıdır. Yeni Bir Terminal Oluşturup, Aşağıdaki Komutları Çalıştıralmalıdır.

> $ npm install

Bu Komut ile React.js ve Projede Kullanılmış Olan Paketler Kurulacaktır. Sonrasında Proje Çalıştırılabilir.

> $ npm start

Bu Komut İle Proje Yayına Alınır. Localhost 3000 Portundan Projeye Erişebiliriz.
