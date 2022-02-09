# github-test

**initialize .git folder**\
``git init .`` *workspace e .git dosyası oluşturma EN ÖNEMLİ İŞLEM BU.*\

**set name, email**\
``git config user.name "fatih"`` *kullanıcı tanımlama*\
``git config user.name "yvzfth@yandex.com"`` *mail tanımlama*\
``git config -l`` *listeleme*\
``touch index.html`` *yeni dosya yaratma*\

**add**\
``git add index.html`` *sadece bir dosya*\
``git status`` *dosyaların add yapılıp yapılmadığını kontrol eder*\
``git rm --cached index.js`` *add i geri alma*\
``git rm -r --cached .`` *tüm add yapılanları geri alma*\
``git add .`` *şu anki klasördeki tüm dosyaları*\
``git add -A`` *workspace deki tüm dosyaları*\

**commit**\
``git commit -m "message"`` *açıklayıcı mesaj yaz*\
``git restore index.html`` *commit yaptıktan sonra dosyada değişiklik yapıldıysa commit durumuna geri döner*\
``git log`` *tüm comittleri görüntüleme*\
``git show <commit id>`` *girilen commit id deki değişiklikleri görüntüleme*\
``git diff`` *commitler arasındaki değişimi gösterir*\
``vi index.html`` *vim editörü açma, yazmak için* ``i`` *ye bas, çıkmak için ctrl+space +* ``:wq``, *kaydetmeden çıkmak için ctrl+space +* ``:qa!``\

**ssh key oluşturma**\
``ssh-keygen -t ed25519 -C "yvzfth@yandex.com"``\
``eval "$(ssh-agent -s)"``\
``ssh-add ~/.ssh/id_ed25519``\
``clip < ~/.ssh/id_ed25519.pub`` *bu kopyalama komutu, kopyalananı githubdaki ayarlar>ssh-key bölümünde yeni ssh key ekle*\

**push - pull**\
``git remote add origin  <REMOTE_URL>`` *REMOTE_URL=git@github.com:yvzfth/github-test.git*\
``git branch -M main`` *branch i main e çevirme*\
``git push -u origin main`` *sadece ilk defada -u origin main kullan daha sonra $git push yeterli*\
``git pull`` *githubdan değişiklikleri geri yükleme*\
