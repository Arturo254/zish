# zish
Una pequeña confirmación de iconos para el tema "Zish" de oh my fish
### Previsualización:

![Screenshot_20231111131028](https://github.com/Arturo254/zish/assets/87346871/c4332e5f-decc-451b-83ab-0cdad43539ef)

### En caso de no tener instalado fish y oh my fish :

```bash

apt install fish -y

apt install which -y

sleep 2

curl https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install | fish

sleep 2

omf install zish
```

### Después clona el repositorio:

```bash
git clone https://github.com/Arturo254/zish

cd zish
```

Despues:

```bash

rm -d -f $HOME/.local/share/omf/themes/zish/functions/*


mv fish_prompt.fish  $HOME/.local/share/omf/themes/zish/functions/

