# Give an example where call apply bind is. required?
Ans :- 
function greet() {
  return `Hello ${this.name}`
}
const person = {
  name: "Lawrence Eagles"
};


greet.call(person); // returns Hello Lawrence Eagles
greet.apply(person); // returns Hello Lawrence Eagles


const greet2 = greet.bind(person) // returns a new copy of greet with this binding
greet2() // Hello Lawrence Eagles

# Call vs Apply vs Bind

const Data = "Lawrence Eagles";
function showName() {
  console.log(`my name is ${this.Data}`);
}
showName.call();  // my name is Lawrence Eagles

////////////////////////////////////////////////////////////////

'use strict';
const Data = "Lawrence Eagles";
function showName() {
  console.log(`my name is ${this.Data}`);
}
showName.call();  // my name is undefined

<img src="https://miro.medium.com/max/1264/1*cdojlfAvRpyX85lGUvd0SA.png"/>

# What is the difference between readFile and readFileSync?
readFileSync() is synchronous and blocks execution until finished. These return their results as return values. 
readFile() are asynchronous and return immediately while they function in the background. You pass a callback function which gets called when they finish.

# What does process in node.js mean?

Ans :- The process object in Node. js is a global object that can be accessed inside any module without requiring it. There are very few global objects or properties provided in Node. js and process is one of them. It is an essential component in the Node.


# Explain what node.js is?
Ans :- Node. js (Node) is an open source development platform for executing JavaScript code server-side. Node is useful for developing applications that require a persistent connection from the browser to the server and is often used for real-time applications such as chat, news feeds and web push notifications.

# What is the difference of JS from browser to JS on node.js
Ans:- 
Unlike the browser where Javascript is sandboxed for your safety, node. js has full access to the system like any other native application. This means you can read and write directly to/from the file system, have unrestricted access to the network, can execute software and more.


# Write three different ways to reverse a string in Javascript? a. using inbuilt method, b. iteratively, c. recursively

 a. using inbuilt method:

function reverseString(str) {
    return str.split("").reverse().join("");
}
reverseString("hello");
b. iteratively:

function reverseString(str) {
    var newString = "";
    for (var i = str.length - 1; i >= 0; i--) {
        newString += str[i];
    }
    return newString;
}
reverseString('hello');
c. recursively:

function reverseString(str) {
  if (str === "")
    return "";
  else
    return reverseString(str.substr(1)) + str.charAt(0);
}
reverseString("hello");

// or

function reverseString(str) {
  return (str === '') ? '' : reverseString(str.substr(1)) + str.charAt(0);
}
reverseString("hello");


# Write a program to check two objects are equal ( deep equal )

function checkObjEqual(obj1,obj2){
for(let key in obj1){
  if(!(key in obj2 )) return false;
  if(obj1[key]!==obj2[key])return false;
}
return true;
}

console.log(checkObjEqual({maroon:'#800000',purple :'#800080'},{purple :'#800080',maroon:'#800000'})) //true

// or

const obj1 = {
        name: 'Ram',
        age: 21
    };
  
    const obj2 = {
        name: 'Ram',
        age: 21
    };
  
    const haveSameData = function (obj1, obj2) {
        const obj1Length = Object.keys(obj1).length;
        const obj2Length = Object.keys(obj2).length;
  
        if (obj1Length === obj2Length) {
            return Object.keys(obj1).every(
                key => obj2.hasOwnProperty(key)
                    && obj2[key] === obj1[key]);
        }
        return false;
    }
    console.log(haveSameData(obj1, obj2));


   # What is shallow equal?

   Ans:- => A function for performing a shallow comparison between two objects or arrays. Two values have shallow equality when all of their members are strictly equal to the corresponding member of the other.

OR

React-Redux uses shallow equality checking to determine whether the component it's wrapping needs to be re-rendered. To do this, it assumes that the wrapped component is pure; that is, that the component will produce the same results given the same props and state.

# Using classes write a program to build a Parking Lot.


<script>

    class Spot {
  constructor({ size, vehicle } = {}) {
    this.size = size
    this.vehicle = vehicle
  }

  addVehicle(vehicle) {
    if(this.isOccupied()) return false
    this.vehicle = vehicle
    return true
  }

  isOccupied() {
      return !!this.vehicle
  }

  getVehicle() {
    return this.vehicle
  }

  releaseVehicle() {
    const currentVehicle = this.vehicle
    this.vehicle = null

    return currentVehicle
  }
}

class ParkingLotManager {
  constructor({ size: { numOfSmallSpot, numOfMediumSpot, numOfLargeSpot } }) {
    this.emptySpots = Array.from({ length: 3 }, (_, i) => {
        if(this._getSizeIndex(1) === i) return Array.from({length: numOfSmallSpot}, () => (new Spot({size: 1})))
        if(this._getSizeIndex(2) === i) return Array.from({length: numOfMediumSpot}, () => (new Spot({size: 2})))
        if(this._getSizeIndex(3) === i) return Array.from({length: numOfLargeSpot}, () => (new Spot({size: 3})))
    })

    this.vehicles = new Map()
  }

  placeVehicle(vehicle) {
      if(this.hasVehicle(vehicle.licenseId)) throw new Error('duplicate vehicle found')
    const sizeIndex = this._getSizeIndex(vehicle.size)
    for (let i = sizeIndex; i < this.emptySpots.length; i++) {
      if (this.emptySpots[i].length > 0) {
        const spot = this.emptySpots[i].pop()
        spot.addVehicle(vehicle)
        this.vehicles.set(vehicle.licenseId, spot)
        return true
      }
    }

    return false
  }

  _getSizeIndex(size) {
    return size - 1
  }

  hasVehicle(licenseId) {
      return this.vehicles.has(licenseId)
  }

  removeVehicle(vehicle) {
    if (!this.hasVehicle(vehicle.licenseId)) return false
    const spot = this.vehicles.get(vehicle)
    spot.releaseVehicle()
    this.vehicles.delete(vehicle)
    this.emptySpots[this._getSizeIndex(this.spot.size)].push(spot)

    return true
  }
}

class Vehicle {
  constructor(id) {
    this.licenseId = id
  }
}

class Motorcycle extends Vehicle {
  constructor(id) {
    super(id)
    this.size = 1
  }
}

class Car extends Vehicle {
  constructor(id) {
    super(id)
    this.size = 2
  }
}

class Truck extends Vehicle {
  constructor(id) {
    super(id)
    this.size = 3
  }
}

const parkingLotManager = new ParkingLotManager({
    size: {
        numOfSmallSpot: 2,
        numOfMediumSpot: 2,
        numOfLargeSpot: 2
    }
})

const car1 = new Car('car1')
const car2 = new Car('car2')
const car3 = new Car('car3')

parkingLotManager.placeVehicle(car1)
parkingLotManager.placeVehicle(car2)
parkingLotManager.placeVehicle(car3)

const car4 = new Truck('car4')
const car5 = new Truck('car5')

parkingLotManager.placeVehicle(car4)



console.log(parkingLotManager);

</script>