# Git ve Github Nasıl Kullanılır

git: dosyalarımızın takibi için kullandığımız program.  
github: bunu programı kullanan en popüler site.


git i bilgisayarına kurmak için.

1. github windows yaz uygun dosyayı inir

2. yöntem:
```powershell
winget install --id Git.Git -e --source winget
```

powershelle gel. git yaz çıkan şeylere bi göz gezdir.  

İlk yapmamız gereken şeylerden biri kendimize isim ve bir e-posta ayarlamak bunun için:
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

dosyaları klasöre taşımak için
Dosyanı editle -> doyanın başına klasör ismini yaz ve / ekle -> commit
