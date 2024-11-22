## 🌟 Vision ile Hızlı Başlangıç

### Vision, Ruby on Rails tabanlı uygulamalarınıza hızlıca modern ve güçlü bir admin paneli eklemenizi sağlar. Sadece birkaç adımda dinamik bir yönetim paneline sahip olun!

 ## 🚀 Kurulum

1. İlk olarak, `vision` gem'ini Gemfile'ınıza ekleyin:
   ```ruby
   gem 'vision'
   ```
2. Gem'i yüklemek için terminalde aşağıdaki komutu çalıştırın:

   ```bash
   bundle 'install'
   ```
3. Yönetmek istediğiniz kaynak için bir admin paneli oluşturun. Örneğin:

   ```bash
   rails generate vision:resource Product
   ```
   Bu işlem, `app/admin/products.rb` dosyasını otomatik olarak oluşturur.

   ---
 ## 🌐 Admin Paneline Erişim

1. Rails sunucunuzu başlatın:

   ```bash
   rails server
   ```

2. Ardından tarayıcınızı açarak şu URL'ye gidin:

      [http://localhost:3000/admin/products](http://localhost:3000/admin/products)

      Tebrikler! Dinamik ve güçlü admin paneliniz hazır! 

      ---

 ## 💡 Sık Karşılaşılan Sorunlar ve Çözümleri
 
 1. "Undefined method" hatası alıyorum!

    * Gem'in doğru yüklenip yüklenmediğini kontrol edin:
    ```bash
    bundle show vision
    ```
    Eğer yüklenmediyse, Gemfile.lock dosyanızı temizleyin ve tekrar bundle install yapın.

 2. Admin rotasına erişemiyorum!

    * Rotaları kontrol edin:

    ```bash
    rails routes | grep admin
    ```
    Eğer rota yoksa, Vision'ın rota dosyalarını yüklediğinden emin olun.

