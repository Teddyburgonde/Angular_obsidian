## Exemple visuel 

<img width="296" height="84" alt="Capture d’écran 2025-10-05 à 11 15 18" src="https://github.com/user-attachments/assets/c3eb0a86-f7a9-48b8-9e95-7edfbbd29837" />

## Checkbox simple 

html

```html
<mat-checkbox>Check box simple</mat-checkbox>
```
<br>

ts

```ts
import {MatCheckboxModule} from '@angular/material/checkbox';
imports: [MatCheckboxModule],
```

## Checkbox avec formulaire réactif

ts 

```ts

import { Component, inject } from '@angular/core';
import { FormBuilder, FormGroup, ReactiveFormsModule } from '@angular/forms';

imports: [ReactiveFormsModule, MatCheckboxModule],

private fb = inject(FormBuilder)
form: FormGroup = this.fb.group ({
	accepTerns: [false]
});
```

html

```html
<form [formGroup]="form">
  <mat-checkbox formControlName="acceptTerms">J'accepte</mat-checkbox>
</form>

```

## Doc officiel 

https://material.angular.dev/components/checkbox/overview
