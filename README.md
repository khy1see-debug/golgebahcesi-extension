# Gölge Bahçesi Mihon/Tachiyomi Eklentisi (Fixed)

Gölge Bahçesi (`golgebahcesi.com`) için Mihon/Tachiyomi eklentisi.

## Yapılan Düzeltmeler (Image Fix)
1. **`imageUrlRequest` hatası çözüldü**: Mihon okuyucusunda `UnsupportedOperationException` fırlatan hatalı `imageUrlRequest` kaldırıldı, `imageRequest` GET metodu tanımlandı.
2. **Göreli CDN URL'leri düzeltildi**: API'nin döndürdüğü `/series/...` URL'leri `https://c2.skycdn.online` önekiyle tam URL haline getirildi.
3. **Cloudflare & WebView Oturum Çerezleri**: `network.cloudflareClient` kullanılarak WebView üzerinden geçilen Turnstile/Cloudflare oturum çerezlerinin Mihon okuyucusunda geçerli olması sağlandı.
4. **Headers**: CDN için gerekli `Referer: https://golgebahcesi.com/` ve `Origin: https://golgebahcesi.com` başlıkları eklendi.
5. **Versiyon**: `versionCode = 2` olarak güncellendi.
