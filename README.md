# :pencil2: zpp_color

# Informations
Librairie pour la colorisation de texte dans un terminal.<br>
Permet de modifier la couleur du texte, la couleur de fond et le style.<br>
Prise en charge de 256 couleurs.<br>
Sélection de la couleur avec le nom, l'id ou une combinaison RGB<br>

## <ins>Prérequis</ins>
- Python 3
<br>

# Installation
```console
pip install zpp_color
```

# Utilisation
### Conseil d'importation du module
Depuis Pypi
```python
from zpp_color import fg, bg, attr
```
Depuis le code source
```python
from color import fg, bg, attr
```

<br>

### <ins>Modification de la couleur du texte</ins>
##### Avec le nom
```python
print(f"{fg('blue')}Ceci est un texte en bleu{attr(0)}")
```
##### Avec l'id
```python
print(f"{fg(3)}Ceci est un texte en bleu{attr(0)}")
```
##### Avec un code RGB
```python
print(f"{fg('0,0,255')}Ceci est un texte en bleu{attr(0)}")
```
> **_NOTE:_**  Toujours rajouter attr(0) à la fin du texte, sinon la couleur s'appliquera pour les lignes suivantes.

<br>

### <ins>Modification de la couleur de fond</ins>
##### Avec le nom
```python
print(f"{bg('red')}Ceci est un texte avec un fond rouge{attr(0)}")
```
##### Avec l'id
```python
print(f"{bg(1)}Ceci est un texte avec un fond rouge{attr(0)}")
```
##### Avec un code RGB
```python
print(f"{bg('255,0,0')}Ceci est un texte avec un fond rouge{attr(0)}")
```

<br>

### <ins>Modification du style du texte</ins>
##### Avec le nom
```python
print(f"{attr('italic')}Ceci est un texte en italic{attr(0)}")
```
##### Avec l'id
```python
print(f"{attr(3)}Ceci est un texte en italic{attr(0)}")
```

<br>

### <ins>Lister les possibilités</ins>
##### Lister les couleurs possibles
```python
zpp_color.list_fg()
```
```python
zpp_color.list_bg()
```
##### Lister les styles possibles
```python
zpp_color.list_attr()
```
