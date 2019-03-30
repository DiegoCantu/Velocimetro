import UIKit

enum Velocidades: Int {
    
    case
    Apagado = 0,
    VelocidadBaja = 20,
    VelocidadMedia = 50,
    VelocidadAlta = 120
    
}

Velocidades.init(rawValue: 0)

class Auto {
    
    var velocidad = Velocidades(rawValue: 0)
    
    init(){
        self.velocidad?.rawValue
    }
   
    func cambioVelocidad(actual : Int, velocidadEnCadena : String) -> (Int,String){
        var tupla: (velocidadActual: Int, velocidadEnCadena : String) = (actual,velocidadEnCadena)
        if (actual == 0){
            tupla.velocidadActual = 20
            tupla.velocidadEnCadena = "VelocidadBaja"
        } else if (actual == 20) {
            tupla.velocidadActual = 50
            tupla.velocidadEnCadena = "VelocidadMedia"
        } else if (actual == 50) {
            tupla.velocidadActual = 120
            tupla.velocidadEnCadena = "VelocidadAlta"
        } else if (actual == 120) {
            tupla.velocidadActual = 50
            tupla.velocidadEnCadena = "VelocidadMedia"
        }
        return tupla
    }
    
}

var auto = Auto()
var tupla: (velocidadActual: Int, velocidadEnCadena : String) = (0,"Apagado")
for _ in 0...19 {
    print(tupla)
    tupla = auto.cambioVelocidad(actual: tupla.velocidadActual, velocidadEnCadena: tupla.velocidadEnCadena)
    
}
