# HungerGames
A hunger games simulator for an easy project to waste my time into. Done with flask.

---

## Estructura del programa

### Clases

* Participante:
   * **id**
   * nombre
   * faccion: Originalmente organizados por distritos
   * CON: Constitucion, stat para pasar checks, contador de alimentos
   * STR: Fuerza, stat para pasar checks
   * DEX: Destreza, stat para pasar checks
   * INT: Bonus generico para pasar checks.
   * items: Array con items
* Evento:
   * **id**
   * test: FUE/DEX/None Modificador que afecta para superarlo
   * dificultad: Numero entre 0 y 1 que indica lo que tienen que superar o igualar para superar el evento.
   * res_superar: Id de un objeto que puede salir 0, si nada o -1 si muere
   * res_fallar: Id de un objeto que puede salir 0, si nada o -1 si muere
* Evento Global (Evento): Afecta a todo el mundo, hay un x% de probabilidad de que ocurra
   * 