![imagen](https://user-images.githubusercontent.com/23361386/136965783-b69aa7ae-cd76-49b8-954e-6ec6d7356a85.png)

```plantuml
@startuml
left to right direction
actor Player
actor Time
usecase Move
usecase Shoot
usecase MoveMario
usecase MoveEnemy
Player --> MoveMario
Player --> Shoot
Time --> MoveEnemy
MoveMario .> Move : <<include>>
MoveEnemy .> Move : <<include>>
@enduml
```

![imagen](https://user-images.githubusercontent.com/23361386/136963199-fbed5fc7-24e9-48ac-8357-8c99ea95aafd.png)


## Preguntas
* Si al activar el caso de uso `Move` hay una colision que impide el movimiento, formaria parte del propio caso de uso `Move` ya que forma parte de la misma conversacion, ¿verdad?
 * Que los enemigos se muevan, las monedas giren, ¿serian casos de uso del actor tiempo? 

