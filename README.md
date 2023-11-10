# ZSH

### اول از همه باید zsh رو نصب کنیم 

### Debian base
‍‍‍
```
sudo apt install zsh
```

### Arch base

```
sudo pacman -S zsh
```

### بعد از اتمام مراحل نصب دستور پایین رو اجرا میکنیم که از bashrc سویچ کنیم روی zsh 

```
chsh -s $(which zsh)
```

### حالا توی مسیر ~ cd ما یک فایل داریم به اسم zshrc. که میتونیم کافنیگ های خودمون برای zsh رو انجا قرار بدیم


## نصب کردن پلاگین برای zsh

### من این جا دوتا پلاگین خیلی پر استفاده رو به شما معرفی کنم که خیلی میتونن کار کردن با ترمینال رو برای ما ساده تر کنن اولی zsh-autosuggestions و دومی هم zsh-syntax-highlighting

### Install zsh-autosuggestions

### ابتدا دستور پایین رو توی ترمینال اجرا کنید:
```
sudo git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

### بعد از اجرا کردن دستور بالا کافیه برین توی zshrc. و zsh-autosuggestions رو به plugins اضافه کنین مثل پایین

plugins=(
  ...
  zsh-autosuggestions
)

### Install zsh-syntax-highlighting

### ابتدا دستور پایین رو داخل ترمینال اجرا کنید:

```
sudo git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

### بعد از اجرا کردن و نصب اون کافیه برین توی فایل zshrc. و بخش پلاگین ها و zsh-syntax-highlighting  رو اضافه کنید

plugins=(
  ...
  zsh-syntax-highlighting
)

### من فایل zshrc خودم رو هم قرار دادم که اگر دوس داشتین میتونین اون رو هم بخونین :)
