#### 3 types : 

1. Signal (le signal normal)
Elle sert à stocker une valeur réactive.
Quand cette valeur change, Angular met automatiquement à jour l'interface qui l'utilise.
Créé avec signal() 
Tu peux: 
- Lire la valeur
- La modifier (set, update)
Rôle: représenter un état. ( booléen, compteur, message etc...)

```ts
count = signal(0);

increase() {
  count.set(1);
}
```


2. Computed signal
Valeur calculée à partir d'autres signals
Crée avec computed()
Rôle: dériver un état.( total, statut, texte formaté, condition (isLoggedIn))

```ts
doubleCount = computed(() => count() * 2);
```


3. Effect
Réagit aux changements de signals
Crée avec effect()
Sert à executer du code quand un signal change.
Rôle: effet secondaire.(console.log, appel Api)

```ts
effect(() => {
  console.log(count());
});

```

