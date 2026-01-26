C'est une interface qui permet le front et le back de communiquer.
Elle expose ensemble des endpoints (URLs) disponibles.

**Un endpoint** est composé d'une methode http et d'une url. 

```java
@GetMapping("/api/users") // <- Endpoint 
public List<User> getUsers() { 	// <- Logique 
	// code ici 

}
```


#### controller


