# Documentacion de Recogida de Datos

**Alumno:** Nerea Pellés Ferrer

## Formato del CSV

Tu archivo `data/partidas.csv` debe tener **minimo** estas columnas:

| Columna | Descripcion | Ejemplo |
|---------|-------------|---------|
| `numero_ronda` | Numero de la ronda (1, 2, 3...) | 1 |
| `jugada_j1` | Jugada del jugador 1 | piedra |
| `jugada_j2` | Jugada del jugador 2 (oponente) | papel |

### Ejemplo de CSV minimo:

```csv
numero_ronda,jugada_j1,jugada_j2
1,piedra,papel
2,tijera,piedra
3,papel,papel
4,piedra,tijera
...
```

---

## Como recogiste los datos?

Marca con [x] el metodo usado y describe brevemente:

### Metodo de recogida:

- [x] **Programa propio**: Cree un programa para jugar y guardar datos
- [x] **Manual**: Jugue partidas y apunte los resultados a mano
- [ ] **Aplicacion/Web externa**: Use una app y exporte los datos
- [ ] **Otro**: _________________

### Descripcion del proceso:

```
He recogido diferentes datos.
Datos contra IA: Le pedí a una inteligencia artificial que jugara contra mí para recoger datos
Datos contra personas: He jugado manualmente contra personas 
He realizado esto para poder obtener datos desde difernetes puntos de vista y diferentes modos de juego, 
recopilando así datos reales de partidas jugadas a mano, datos reales de partidas jugadas en ordenador 
y datos contra una inteligencia artificial.

```
---

## Datos adicionales capturados

Si capturaste datos extra ademas de los basicos, marcalos aqui:

- [ ] `tiempo_reaccion_ms` - Tiempo que tardo el jugador en responder
- [ ] `timestamp` - Fecha/hora de cada jugada
- [ ] `sesion` - ID de sesion de juego
- [x] `resultado` - victoria/derrota/empate
- [ ] Otro: _________________

### Descripcion de datos adicionales:

```
Además de los datos básicos y el resultado de dicha ronda, he analizado otros datos extra como
jugadas anteriores, jugadas que se realizan tras ganar, tras perder, tras empatar,
el procentaje de cada tipo de jugada (es decir el porcentaje de piedras, papeles y tijeras), las rachas
de cada tipo de jugada, los cambios que se realizan tanto tras perder como tras ganar, patrones de alternancia
las tendecias más recientes, el numero de ronda actual para ver en que punto de la partida se está y el cambio
numérico de la jugada anterior a la actual. Todos estos datos se han recogido en un total de 39 features.

```

---

## Estadisticas del dataset     

- **Total de rondas:** 166
- **Numero de sesiones/partidas:** 4 
  - Contra la IA (100 rondas)
  - Contra Rubén (15 rondas)
  - Contra jugador 1 (25 rondas)
  - Contra jugador 2 (26 rondas)
- **Contra cuantas personas diferentes:** 4

### Tipo de IA:

- [x] **IA Especifica**: Entrenada para ganar a UNA persona concreta
  - Nombre/identificador del oponente: Nerea Pellés Ferrer (yo)
- [ ] **IA General**: Entrenada para ganar a cualquier oponente
