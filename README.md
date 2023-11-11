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
```

# Contenido :


si sabes lo que haces lo puedes editar segun tu preferencia.
si no sabes lo que haces no muevas nada 
```bash

# name: Zish

function _is_git_dirty
  echo (command git status -s --ignore-submodules=dirty 2> /dev/null)
end

function fish_prompt
  set_color -o red
  printf '┌─<'
  set_color -o blue
  printf '%s ' "ONYX"
  set_color $fish_color_autosuggestion[1]
  printf '「★」'
  set_color cyan
  printf '%s ' "Hackers"
  set_color $fish_color_autosuggestion[1]
  printf 'in '
  set_color -o green
  printf '%s' (prompt_pwd)
  set_color -o red
  printf 'ϟ'

  echo
  set_color -o red
  printf '└─<'
  set_color yellow
  printf '%s' (__fish_git_prompt)
  if [ (_is_git_dirty) ]
    set_color blue
    printf '* '
  end
  set_color -o red
  printf '>──'
  set_color yellow
  printf '» '
  set_color normal
end

```
