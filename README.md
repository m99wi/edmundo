# edmundo
mi primer repo
/ Importante: No modificar ni el nombre ni los argumetos que reciben las funciones, sólo deben escribir
// código dentro de las funciones ya definidas.

function menorMayor(numeros) {
  // La función llamada 'menorMayor' recibe como argumento un arreglo de números llamado 'numeros' y debe devolver un
  // arreglo que contenga el menor número del arreglo 'numeros' en la posición cero y el mayor número del arreglo
  // 'numeros' en la posición 1.
  // Ej:
  // menorMayor([4, 6, 1, 7, 15]) debe retornar [1, 15]
  // ya que 1 es el número más chico (menor) dentro del arreglo [4, 6, 1, 7, 15]
  // y 15 es el número más grande (mayor) dentro del arreglo [4, 6, 1, 7, 15]

  // Tu código aca:
  'menorMayor'(59, 84, 33, 77)
  return(33, 84)
  array(33, 59, 77, 84)
}

function stringMasLarga(strings) {
  // La función llamada 'stringMasLarga', recibe como argumento un arreglo de strings llamado 'strings'
  // y debe devolver el string más largo que hay en el arreglo (Es decir el de mayor cantidad de caracteres)
  // Ej:
  // stringMasLarga(['hi', 'hello', 'ni hao', 'guten tag']); debe retornar 'guten tag'
  // stringMasLarga(['JavaScript', 'HTML', 'CSS']); debe retornar 'JavaScript'

  // Tu código aca:
stringMasLarga([amigos, corazon, chocolate])
return(chocolate)
stringMasLarga(futboll, casa, tesoro)
return(futboll)
}

function buscarAmigo(amigos, nombre) {
  // La funcion llamada 'buscarAmigo' recibe como argumento un array llamado 'amigos' que contiene
  // en cada posición del arreglo un objeto que tiene como propiedades 'nombre' y 'edad'. También
  // recibe un string llamado 'nombre'.
  // Debe devolver el objeto cuya propiedad 'nombre' coincida con el string 'nombre' recibido por argumento.
  // Ej:
  //  var amigos = [{ nombre: 'toni', edad: 33 } , { nombre: 'Emi', edad: 25 }];
  //  buscarAmigo(amigos, 'toni') debe devolver { nombre: 'toni', edad: 33 };

  // Tu código aca:
  'buscarAmigo', function() {
    var amigos = [{ nombre: 'toni', edad: 33 } , { nombre: 'Emi', edad: 25 }];

    ('should return "{ nombre: "toni", edad: 33 }"', function() {
      expect(buscarAmigo(amigos, 'toni').nombre).toBe('toni');
    });
    it('should return "{ nombre: "toni", edad: 33 }"', function() {
      expect(buscarAmigo(amigos, 'Emi').nombre).toBe('Emi');
    });
}

function sumArray(array, n) {
  // La función llamada 'sumArray' recibe como argumento un arreglo de números ordenados llamado 'array' y un número
  // entero llamdo 'n' y debe devolver true si alguna combinación de dos números cualesquiera del arreglo sumados
  // dan n, y devuelva false si ninguna combinación de dos números sumados da como resultado el número n.

  // Ej:
  // sumArray([2,5,7,10,11,15,20], 13)  debería devolver true ya que 2 + 11 = 13
  // sumArray([2,5,7,10,11,15,20], 14)  debería devolver false ya que no es posible sumar 14 con dos números del arreglo
  // Pista: Podes usar bucles/ciclos anidados
  // Aclaración: No es válido sumar el mismo número dos veces
  // Ej:
  // sumArray([2,5,7,10,11,15,20], 4)  Si bien 2 + 2 = 4 no está permitido sumar el mismo número dos veces
  // por lo tanto también debería devolver false en este caso

  // Tu código aca:
  'sumArray', function() {
    it('should return true with [2,5,7,10,11,15,20], 2 + 11 = 13', function() {
      expect(sumArray([2,5,7,10,11,15,20], 13)).toBe(true);
    });
    it('should return false.', function() {
      expect(sumArray([2,5,7,10,11,15,20], 14)).toBe(false);
    });
    it('should return false (cant sum the same number with itself)', function() {
      expect(sumArray([2,5,7,10,11,15,20], 4)).toBe(false);
    });

};

function pluck(array, propiedad) {
  // La función llamada 'pluck' recibe como argumento un array de objetos llamado 'array' y el nombre de una
  // propiedad.
  // La función debe devolver un nuevo arreglo con solo los valores dentro de la propiedad recibida
  // Ej:
  // var productos = [{ name: 'TV LCD', price: 100}, { name: 'Computadora', price: 500 }]
  // productos.pluck(productos, 'name') debería devolver ['TV LCD', 'Computadora']
  // Pista: es una buena oportunidad para usar map.

  // Tu código acá:
  'pluck', function() {
    var productos = [{ name: 'TV LCD', price: 100}, { name: 'Computadora', price: 500 }]
    it('should return ["TV LCD", "Computadora"]', function() {
      expect(pluck(productos, 'name')).toEqual(['TV LCD', 'Computadora']);
    });
    it('should return [100, 500]', function() {
      expect(pluck(productos, 'price')).toEqual([100, 500]);
    });
}

// =======================================================================


function crearClasePersona() {
  class Persona {
    constructor(nombre, edad, hobbies, amigos) {
      // El constructor de la clase Persona recibe nombre (string), edad (integer), hobbies (array de strings), amigos (array de objetos)
      // Inicializar las propiedades de la persona con los valores recibidos como argumento

      // Tu código aca:
      'Clase', function() {
        describe('crearClasePersona', function() {
          it('should return a user constructor that correctly builds user objects', function() {
              const Persona = crearClasePersona();
              const persona = new Persona('toni', 23, ['futbol'], [{nombre: 'martin', edad: 31}]);
              expect(persona.nombre).toBe('toni');
              expect(persona.edad).toBe(23);
              expect(persona.hobbies).toEqual(['futbol']);
              expect(persona.amigos).toEqual([{nombre:'martin', edad: 31}])
    }

    addFriend(nombre, edad) {
      // El método 'addFriend' recibe un string 'nombre' y un entero 'edad' y debe agregar un objeto:
      // { nombre: nombre, edad: edad} al arreglo de amigos de la persona.
      // No debe retornar nada.

      // Tu código aca:
      'should add a friend with addFriend', function() {
        const Persona = crearClasePersona();
        const persona = new Persona('toni', 23, ['futbol'], [{nombre: 'martin', edad: 31}]);
        persona.addFriend('Leo', 45);
        expect(persona.amigos[1]).toEqual({ nombre: 'Leo', edad: 45});
    
    }

    addHobby(hobby) {
      // El método 'addHobby' recibe un string 'hobby' y debe agregarlo al arreglo de hobbies de la persona.
      // No debe retornar nada.

      // Tu código aca:
      'should add a hobbie with addHobby', function() {
        const Persona = crearClasePersona();
        const persona = new Persona('toni', 23, ['futbol'], [{nombre: 'martin', edad: 31}]);
        persona.addHobby('hobbie');
        expect(persona.hobbies[1]).toBe('hobbie');
    
    }
    getFriends() {
      // El método 'getFriends' debe retornar un arreglo con sólo los nombres del arreglo de amigos
      // de la persona.
      // Ej:
      // Suponiendo que la persona tiene estos amigos: [{nombre: 'martin', edad: 31},{nombre: 'toni', edad: 33}]
      // persona.getFriends() debería devolver ['martin', 'toni']

      // Tu código aca:
      'should get all friends with getFriends', function() {
        const Persona = crearClasePersona();
        const persona = new Persona('toni', 23, ['futbol'], [{nombre: 'martin', edad: 31},{nombre: 'toni', edad: 33}]);
        expect(persona.getFriends()).toEqual(['martin','toni']);
      });
    }

    getHobbies() {
      // El método 'getHobbies' debe retornar un arreglo con los hobbies de la persona
      // Ej:
      // persona.getHobbies() debe devolver ['correr', 'dormir', 'nadar']

      // Tu código aca:
      ('should get all hobbies with getHobbies', function() {
        const Persona = crearClasePersona();
        const persona = new Persona('toni', 23, ['futbol'], [{nombre: 'martin', edad: 31}]);
        expect(persona.getHobbies()).toEqual(['futbol']);
      });
    }

    getPromedioEdad() {
      // El método 'getPromedioEdad' debe retornar el promedio de edad de los amigos de una persona
      // Ej:
      // Si la persona tuviera estos amigos:
      // {
      //   amigos: [{
      //     nombre: 'toni',
      //     edad: 33,
      //   }, {
      //     nombre: 'Emi',
      //     edad: 25
      //   }]
      // }
      // persona.getPromedioEdad() debería devolver 29 ya que (33 + 25) / 2 = 29

      // Tu código aca:

    }'should get age average with getPromedioEdad', function() {
      const Persona = crearClasePersona();
      const persona = new Persona('toni', 23, ['futbol'], [{
          nombre: 'toni',
          edad: 33,
        }, {
          nombre: 'Emi',
          edad: 25
        }]);
      expect(persona.getPromedioEdad()).toBe(29);
    });
  };

  return Persona;
}

/* ====================== EXTRA CREDIT ===================== */
// Este ejercicio no cuenta en el puntaje del checkpoint
// pero si llegas hasta aca y lo haces quiere decir que venis super bien!

function filtrar(funcion) {
  // Escribi una función filtrar en el prototipo de Arrays,
  // que recibe una funcion (callback) que devuelve true o false.
  // filtrar los elementos de ese arreglo en base al resultado de esa funcion
  // comparadora, devolver un nuevo arreglo con los elementos filtrados.
  // NO USAR LA FUNCION FILTER DE LOS ARREGLOS.
  // ej:
  // var productos = [{
  //   price: 100,
  //   name: 'tv'
  // }, {
  //   price: 50,
  //   name: 'phone'
  // }, {
  //   price: 30,
  //   name: 'lamp'
  // }]
  // productos.filtrar(function(p) {
  //   return p.price >= 50;
  // }) => [{price: 100, name:'tv'}]

};

// No modifiques nada debajo de esta linea
//
module.exports = {
  sumArray,
  menorMayor,
  stringMasLarga,
  buscarAmigo,
  pluck,
  crearClasePersona,
  filtrar
}
