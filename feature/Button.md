## Exemple visuel


<img width="298" height="52" alt="Capture d’écran 2025-10-05 à 02 31 01" src="https://github.com/user-attachments/assets/f0804786-8403-4187-990e-5e88f2c9860b" />

<br>

## Créer un dossier components et placer vous àl'interieur. 



```bash
src/
├── app/
│   ├── components/
```
<br>

## Créer un button

```bash
ng generate component nomducomposant
```

<br>

## html

```bash
<button matButton="filled">
	montextesurlebouton
</button>

<button mat-raised-button mat-flat-button type="button" >
  mon autre bouton
</button>

```

<br>

## ts 

```bash
import { MatButtonModule } from '@angular/material/button';

imports: [MatButtonModule],
```
<br>

## Dans app.html 

```bash
<nomdu-selector></nomdu-selector>
```
<br>

## Dans app.ts

```bash
import {NomdelaClass} from 'lechemin';

imports: [NomdelaClass],

```

<br>

## Doc officiel

https://material.angular.dev/components/button/overview


