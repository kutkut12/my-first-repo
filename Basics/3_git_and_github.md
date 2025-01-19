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
- **Commit**:  
  Değişikliklerin kaydedilmesi işlemi.
- **Branch**:  
  Ana koddan ayrılıp bağımsız olarak bir değişiklik veya geliştirme yapmak için kullanılan yan dallar.  
- **Merge**:  
  Bir branch'teki değişiklikleri başka bir branch'e (genelde ana branch'e yani **main**e) birleştirme işlemi.
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
Git'in web sitesinden indirin.  
[Git İndirme Sayfası](https://git-scm.com/)  

**2. Yöntem**:  
Komut sistemiyle kurulum:  
```powershell
winget install --id Git.Git -e --source winget
```

### Kurulum Sonrası Git'in Yüklü Olup Olmadığını Kontrol Etmek Veya Versiyonunu Öğrenmek İçin:
```
git --version
```

---

### İlk Yapılacaklar
Git'i kullanmaya başlamadan önce ilk olarak kendimize isim, e-posta ve varsayılan editör tanımlamamız gerekir  
```powershell
git config --global user.name "Your Name"
```

```powershell
git config --global user.email "you@example.com"
```

```powershell
git config --global core.editor "code --wait"
```

Ben burada VS Code'u tanımladım ama siz istediğinizi tanımlayabilirsiniz.  

### Repo Oluşurmak İçin  
Repo oluşturmak istediğimiz yere geliriz.  
mkdir ile repo'ya istediğimiz ismi veririz.  
cd ile o repoya gireriz.    
ve sonrasında  
```
git init
```
ile repo'muzu oluştururuz.  

### Stage, Commit

stage durumunu öğrenmek için
```powershell
git status
```

stage durumunu kısa bir şekilde görmek için
```powershell
git status -s
```

```powershell
A  yeni eklenmiş ve aşama alanına eklenmiş
M  değiştirilmiş ve aşama alanına eklenmiş
 M değiştirilmiş ama aşama alanına eklenmemiş
MM değiştirilmiş ve aşama alanına eklenmiş ama bir daha değiştirilmiş
?? izlenmemiş
```



bütün dosyaları 
```powershell   
git add .
```

sonu .py ile biten dosyaları
```powershell
git add *.py
```

spesifik bir dosyayı
```powershell  
git add "dosya"
```

comnit mesajını yazmak zorundasın
```powershell  
git commit -m "commit mesajın" 
``` 

3 hal var:    
modified: değişiklik yaptığında. 
staged: değişiklikler kayıt edilmeye hazır olduğunda.  
committed: değişiklikler kayıt edildiğinde.  

tracked
untracked

githubta klasör oluşurmak için:  
Add new file -> Klasör ismini yaz -> Sonunda / koy -> .gitkeep yaz çünkü git boş klasörleri umursamıyor. ille de içinde bir şey olmalı.

dosyaları klasöre taşımak için:  
Dosyanı editle -> doyanın başına klasör ismini yaz ve "/" ekle -> commit
