Clases

classDiagram
  direction RL
  class Ejercicio5 {
    -p : String []
    -p1 : String []
    -p2 : String []
    -p3 : String []
    -p4 : String []
    -n1 : int
    -n2 : int
    -l2 : double
    -c : int
    -c2 : double
    -c3 : double
    -c4 : double
    -d : int
    -x : double
    -resultado : Double
  }
  
  
  Flujo
  
  graph TD
    A(Preguntamos al usuario) -->B(Operación aceptada)
    B -->|Si| C(Solicitamos valores)
    B -->|No| D(Error)
    D --> A
    C --> E{Triángulo}
    E -->|Si| F(Multiplicamos los valores y dividimos entre 2)
    F --> Z
    E -->|No| G{Rectángulo}
    G -->|Si| H(Multiplicamos los valores)
    H --> Z
    G -->|No| J{Pentágono}
    J -->|Si| I(Solicitamos valor para el lado y lo elevamos al cuadrado y multiplicamos por 1.72)
    I --> Z
    J -->|No| K{Hexágono}
    K --> L(Solicitamos valor para el lado para calcular perímetro y apotema para multiplicarlos entre si y dividirlos entre 2)
    L --> Z(Resultado)
