let a:string=`
<div>yo,${name}</div>>
`
let b:number=1;
let c:string[]=['xiaoming','xiaohong','xiaogang'];
let d:number[]=[1,2,3];
let e:boolean=true;
let f:[number,string]=[1,'hello'];
let g:any=1;
let i:void;
function fun():void {
    alert('11')
}


let obj={a:1,b:2};
let add=({a,b}:{a:number,b:number})=>a+b;
console.log(add(obj));

class Person {
    name:string;

    constructor(name:string)
    {
        this.name=name;
    }
    greet(){
        console.log(this.name)
    }
}

class Student extends Person {
    major: string;

    studentGreet() {
        return `${this.major}xide${this.name}wenhao`
    }

    constructor(name: string, major: string) {
        super(name);
        this.major = major;
    }
}

let person1=new Person('ren');
person1.greet();

let student=new Student('xiaoming','zhexue');
console.log(student.studentGreet())