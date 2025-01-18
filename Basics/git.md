# Git ve GitHub Nasıl Kullanılır

## Temel Kavramlar
- **Git**:  
  Dosyalarımızın takibini yapmamızı sağlayan bir versiyon kontrol sistemi.  
- **GitHub**:  
  Git'i kullanarak projelerimizi bulut üzerinde depolamamızı ve diğer insanlarla paylaşmamızı sağlayan en popüler platform.  
- **Repository (Repo)**:  
  Bir projenin veya dosyaların saklandığı Git deposu.  
- **Main, Master**:  
  Ana proje, kodun bulunduğu yer. Ana dal.
- **Branch**:  
  Ana koddan bağımsız olarak bir değişiklik veya geliştirme yapmak için kullanılan yan dallar.  
- **Merge**:  
  Bir branch'teki değişiklikleri başka bir branch'e (genelde ana branch'e yani **main**e) birleştirme işlemi.
- **Commit**:  
  Değişikliklerin kaydedilmesi işlemi. 
- **Clone**:  
  GitHub üzerindeki bir projeyi yerel bilgisayara indirme işlemi.  
- **Pull**:  
  Uzak repodaki (örneğin GitHub'daki) güncellemeleri yerel repo ile senkronize etme.
- **Pull Request**:  
  Yapılan değişikliklerin ana projeye dahil edilmesi için yapılan istektir
- **Push**:  
  Yerel repodaki değişiklikleri uzak repoya gönderme işlemi.  



## Git'in Kurulumu ve İlk Bakış

### Git'i Bilgisayarınıza Kurmak İçin:
**1. Yöntem**:  
GitHub'un web sitesinden indirin.  
[Git İndirme Sayfası](https://git-scm.com/)  

**2. Yöntem**:  
Komut sistemiyle kurulum:  
```powershell
winget install --id Git.Git -e --source winget
```

### Kurulum sonrası Git'in yüklü olup olmadığını kontrol etmek, Git'in versiyonunu öğrenmek için:
```
git --version
```

### İlk Yapılacaklar
Git kurulumundan sonra ilk olarak kendimize isim, e-posta ve bir varsayılan editör tanımlamamız gerekir:
```powershell
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global core.editor "code --wait"
```

Sonra repo oluşturabiliriz.
```powershell
git init   
git add . 
git add *.py   
git add "dosya"  
git commit -m "commit mesajın" 
``` 
comnit mesajını yazmak zorundasın

3 hal var:    
modified: değişiklik yaptığında. 
staged: değişiklikler kayıt edilmeye hazır olduğunda.  
committed: değişiklikler kayıt edildiğinde.  


githubta klasör oluşurmak için:  
Add new file -> Klasör ismini yaz -> Sonunda / koy -> .gitkeep yaz çünkü git boş klasörleri umursamıyor. ille de içinde bir şey olmalı.

dosyaları klasöre taşımak için:  
Dosyanı editle -> doyanın başına klasör ismini yaz ve "/" ekle -> commit
