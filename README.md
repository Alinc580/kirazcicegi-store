# Kiraz Çiçeği — Web Sitesi

Bu depo Kiraz Çiçeği Store için oluşturulan mobil uyumlu, statik **önizleme sitesini** içerir.

## Durum

- **Private GitHub deposu.** Siteyi herkese açık olarak sunmak için Cloudflare Pages üzerinden ayrıca yayınlamak gerekir.
- `index.html` tek başına çalışır; CSS, JavaScript ve örnek ürün fotoğrafları HTML içine gömülüdür.
- Görseller yapay zekâyla üretilmiş temsili fotoğraflardır, gerçek ürün fotoğrafları değildir.
- Gerçek fiyat/teslimat garantisi veya ödeme alma sistemi bulunmaz.

## Cloudflare Pages

1. Cloudflare panelinde **Workers & Pages → Create application → Pages → Connect to Git** yolunu izleyin.
2. `Alinc580/kirazcicegi-store` deposunu seçin.
3. Production branch: `main`, framework: `None`, build command: boş veya `exit 0`, output directory: `.`
4. **Save and Deploy** ile yayına alın. Gerçek `*.pages.dev` adresini Cloudflare sağlar.

**Önemli:** GitHub depomuz private olsa bile Cloudflare Pages sitesi, ayrı erişim kontrolü kurulmadıkça herkese açık olur. Demo için `_headers` ve `robots.txt` üzerinden arama motorlarında indeksleme kısıtı vardır; bu bir kimlik doğrulama koruması değildir.

## Gerçek işletme sitesine geçmeden önce

Gerçek ürün fotoğrafları, işletme bilgileri, fiyat/teslimat açıklamaları, hukuki sayfalar ve iletişim bağlantılarını doğrulayın. Canlı halka açık yayın için `noindex` ayarlarını yeniden değerlendirin.
