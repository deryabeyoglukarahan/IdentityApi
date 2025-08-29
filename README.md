# 🔐 Identity & Data Protection - User Management API

Bu proje, **Entity Framework Core Code First** yaklaşımı ile **kullanıcı yönetimi** ve **veri koruma (Data Protection)** mekanizmalarını uygulamayı amaçlamaktadır.  
Proje kapsamında **User tablosu** oluşturulmuş, kullanıcı kayıtlarında **model validation** yapılmış ve şifreler güvenli şekilde **hashlenerek** veritabanında saklanmıştır.

---

## 📂 Proje Gereksinimleri

- **ORM Aracı**: Entity Framework Core  
- **Yaklaşım**: Code First  
- **Tablo**: `Users`  
- **Alanlar**:
  - `Email` (string) → Kullanıcının e-posta adresi (**[Required]** ile zorunlu alan)  
  - `Password` (string) → Kullanıcının şifresi (**hashlenmiş olarak saklanır**)  

- **Özellikler**:
  - Kullanıcı kaydı yapılabilmeli  
  - `Model Validation` kullanılmalı (`[Required]`, `[EmailAddress]` vb.)  
  - Şifreler **plain text** olarak değil, **hash** edilmiş olarak saklanmalı  
  - Identity API veya custom identity mekanizması ile veri koruma  
