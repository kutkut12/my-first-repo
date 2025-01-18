conda'yı indir  

conda terminaline gel  
search -> anaconda (anaconda, miniconda ayrımı yok)
```
conda
```
çeşit çeşit komut çıkacak

conda ortamını oluşturmak istediğim klasöre git:
```
$ (base) C:\>cd C:\Users\kutay\Desktop
```

yeni klasör oluştur:
```
$ (base) C:\Users\kutay\Desktop>mkdir playground
```
o klasörün içine gir:
```
$ (base) C:\Users\kutay\Desktop>cd playground
```

conda ortamını oluştur (şuan o klasörün içindeyiz):
```
$ conda create --prefix ./env istediğim paketler
```

paket örnekleri:  
pandas numpy matplotlib scikit-learn jupyter

bir paketi eklemeyi unuttuysan: 
```
$ conda install paket
```

ortamı aktivite etmek için:  
```
$ conda activate C:\Users\kutay\Desktop\playground\env
```
sonuna \env eklemelisin.  
ortamı aktive ettiğin zaman (base) den çıkıp ortamına girersin

ortamı deaktive etmek için:  
```
$ conda deactivate
```

jupyter notebooku açmak için:  
```
$ jupyter
```


