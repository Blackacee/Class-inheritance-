# Class-inheritance-

class SuperClass {
 constructor() {
 this.logger = console.log;
 }
 log() {
 this.logger(`Hello ${this.name}`);
 }
}
class SubClass extends SuperClass {
 constructor() {
 super();
 this.name = 'subclass';
 }
}
const subClass = new SubClass();
subClass.log(); // logs: "Hello subclass"
