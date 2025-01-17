# Git ve Github Nasıl Kullanılır

githubu bilgisayarına kurmak için.

1. github windows yaz uygun dosyayı inir

2. yöntem:
```powershell
winget install --id Git.Git -e --source winget
```

powershelle gel. git yaz çıkan şeylere bi göz gezdir.


Kendimize isim ve bir e-posta ayarlamamız gerekiyor:
```powershell
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

git init  
git add .
git add "dosya"
git commit -m "commit mesajın"
comnit mesajını yazmak zorundasın


githubta klasör oluşurmak için:
Add new file -> Klasör ismini yaz -> Sonunda / koy -> .gitkeep yaz çünkü git boş klasörleri umursamıyor. ille de içinde bir şey olmalı.

dosyaları klasöre taşımak için
Dosyanı editle -> doyanın başına klasör ismini yaz ve / ekle -> commit
