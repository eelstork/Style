### Why do we ever need style guides when we have compilers?
Imposing a style avoids whitespace noise in commits.
### Why not use an existing style guide?
I created this guide to assist contributions to repositories I manage. I am unaware of a style guide I would like to use, or even repurpose.
### Naming
```
usePositiveFormulations; // correct
avoidNegativeFormulations; // incorrect
```
### Documenting fields
Favour short lines of code: avoid trailing comments.
```
public bool myVar = false; // the trailing comment unnecessarily extends the length of this line of code.
```
Document members using `/** ..*/` one line above.
```
/** short lines of code */
public bool myVar = false; 
```
### Control characters
Add a blank line after the opening bracket and before the closing bracket of a function or class definition.
```
function foo(){

  // fun starts here.

}
```
Do *not* add a blank line after the opening bracket and before the closing bracket of an accessor definition or control flow.
```
int foo{
  get{ 
    if(bar){
      return 0;
    }else{
      return 3;
    }
  }
}
```
### Decorated brackets
Put brackets on the same line as the associate declaration.
```
void Start(){
  // correct
}

void Start()
{
  // avoid
}
```
Where there is online one line of code between the brackets, the following is allowed.
```
void Start(){ reallyConcise(); }
```
That's all folks, thanks for reading.
