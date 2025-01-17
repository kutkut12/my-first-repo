condayı indir  

conda terminaline gel  
search -> conda

conda ortamını oluşturmak istediğim klasöre git:
```
$ (base) C:\>cd C:\Users\kutay\Desktop
```

yeni klasör oluştur:
```
$ (base) C:\Users\kutay\Desktop>mkdir my_conda_env
```
o klasörün içine gir:
```
$ (base) C:\Users\kutay\Desktop>cd my_conda_env
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
$ conda activate C:\Users\kutay\Desktop\my_conda_env\env
```

ortamı aktive ettiğin zaman (base) den çıkıp ortamına girersin

ortamı deaktive etmek için:  
```
$ conda deactivate
```




