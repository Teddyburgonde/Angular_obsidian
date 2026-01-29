Exemple visuel 

<img width="453" height="204" alt="example_card" src="https://github.com/user-attachments/assets/06f03878-c26f-4aa9-9fab-a1d09fb0e660" />



## Placer vous dans components

```bash
ng generate component card
```

<br>

## html

```html
<mat-card class="example-card" appearance="outlined">
  <mat-card-header>
    <div mat-card-avatar class="example-header-image"></div>
    <mat-card-title>Titre</mat-card-title>
  </mat-card-header>
  <mat-card-content>
      <!-- Ici on place le contenu qui 
       s'aggrandira automatiquement en fonction de la taille du contenu -->
    <p>
     Je suis un contenu
    </p>
  </mat-card-content>
  <mat-card-actions>
    <!-- Ici on place les boutons -->
    <button matButton>Je suis un bouton</button>
  </mat-card-actions>
</mat-card>
```

<br>

## css


```css
.example-card {
  max-width: 400px;
}
```

<br>

## ts

```ts
import {MatCardModule} from '@angular/material/card';

imports: [MatCardModule],

```

## app.html

```html
<app-nomduSelector></app-nomduSelector>
```

<br>

## app.ts

```ts

import { nomdelaClasse } from 'Le chemin';
imports: [Card],

```

## Doc officiel 

https://material.angular.dev/components/card/overview
