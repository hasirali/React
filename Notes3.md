# JSX In Depth
 ```
const heading = React.createElement("h1",{id:child},"Namaste React")
```
it is same thing as but is lenghtier and get complicated when writing nested tag
so we use JSX

-JSX is not mean HTML in Javascript instead we can say that it is HTML or XML like Syntax
-We Can build application without the use of JSX but we use JSX as irt make our life easier

```
const heading=<h1 id="heading"> "Namaste react by JSX"</h1>
```



```
SO When we write this code:


const jsxheading=<h1 id="heading">Namaste react by JSX</h1>
```
1) what happen is that this code firstly get TRANSPIlE(converted) that React can understand, and this transpiling is done by Parcel 
with the help of Babel (module)



- work of Babel: Convert JSX into React Code or we can say it convert it into this kind of Format

2) After it gets conveted to ReactElment and REact element is a Javascsript object and this javascript object or react element is get rendered as HTML Element
```
 React.createElement("h1",{id:child},"Namaste React by JSX")
```

# EXTRA
- when use console.log(headingjsx) and console.log(heading)
you will get the same thing
