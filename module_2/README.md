# 2.Tēma

## 9. Salīdzināt lokālā un github commit hash  
Hash abiem commit ir vienādi: c33b67681ca047e3fb559a2bdb963bcefd01eb65


Lokālais commit hash:  
> > $ git show  
> > commit c33b67681ca047e3fb559a2bdb963bcefd01eb65 (HEAD -> main, origin/main, origin/HEAD)  
> > Author: valtgun <valtgun1@outlook.com>  
> > Date:   Thu Apr 28 07:40:42 2022 +0300  
> > MD2 p.11 Iekopēti faili no MD1  

Github commit hash:
![Github hash](atteli/github_hash.png)  

## 13. Hash salīdzīnāšana pārkopētiem failiem.  

Tika salīdzināts fails 01-HelloWorld.py  
Faili ir ar vienādiem hash, t.i. git neredz atšķirību stap šiem failiem.

Katalogā module_1:  
> > $ git cat-file -p main^{tree}:module_1  
> > 100644 blob aa5be9a16125124e9248e3d363b0add8df5a58e1    01-HelloWorld.py

Katalogā module_2:
> > $ git cat-file -p main^{tree}:module_2  
> > 100644 blob aa5be9a16125124e9248e3d363b0add8df5a58e1    01-HelloWorld.py

