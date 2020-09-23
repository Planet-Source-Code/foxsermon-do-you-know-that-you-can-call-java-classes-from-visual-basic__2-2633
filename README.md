<div align="center">

## Do you know that you can call Java classes from Visual Basic ??


</div>

### Description

Do you know that you can call Java classes from Visual Basic ??

well, that's not a fair tale anymore, it's possible.

let me guide you through this adventure.

Firts at all, we need a Java class,

Here you will find an example:

Java Code

//

----

public class MyTest {

public int myfunction(int value1, int value2) {

return value1+value2;

}

}

//

----

Compile it

i.e. javac MyTest.java

and when you get MyTest.class file, you must register it

for this you will need Microsfot SDK for Java

you can download from this link

http://www.microsoft.com/java/download/dl_sdk40.htm

when you have downloaded and installed.

include it on Path variable enviroment

just do it using Command Ms-DOS

set path=%path%;C:\Program Files\Microsoft SDK for Java 4.0\bin\

(this path could change)

then you must register our MyTest.class file.

you should do it using javareg.exe file from Microsoft SDK for Java

i.e. javareg /register /class:MyTest /progid:MyTest

if everything is well-done then you should see a MessageBox displayed with

Succesfull register Class message.

Otherwise, you must check the correct spelling on the command line.

Now, the next step, copy the new Java class file that was generated.

MyTest.class

and paste in C:\Winnt\Java\Trustlib\ folder

if you have windows 98, this folder may change.

And the last step, open a New Project on Visual Basic.

And paste this brief code on the Form Load event for example and run it.

Set x = CreateObject("MyTest")

MsgBox x.myfunction(1, 1)

Congratulations !!!

you can use Java Class from Visual Basic.

Please do not forget to vote for this article. =)
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[foxsermon](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/foxsermon.md)
**Level**          |Intermediate
**User Rating**    |4.4 (57 globes from 13 users)
**Compatibility**  |Java \(JDK 1\.1\), Java \(JDK 1\.2\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__2-57.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/foxsermon-do-you-know-that-you-can-call-java-classes-from-visual-basic__2-2633/archive/master.zip)





### Source Code

```
Do you know that you can call Java classes from Visual Basic ??
well, that's not a fair tale anymore, it's possible.
let me guide you through this adventure.
Firts at all, we need a Java class,
Here you will find an example:
Java Code
//**************************************************
public class MyTest {
public int myfunction(int value1, int value2) {
return value1+value2;
}
}
//***************************************************
Compile it
i.e. javac MyTest.java
and when you get MyTest.class file, you must register it
for this you will need Microsfot SDK for Java
you can download from this link
http://www.microsoft.com/java/download/dl_sdk40.htm
when you have downloaded and installed.
include it on Path variable enviroment
just do it using Command Ms-DOS
set path=%path%;C:\Program Files\Microsoft SDK for Java 4.0\bin\
(this path could change)
then you must register our MyTest.class file.
you should do it using javareg.exe file from Microsoft SDK for Java
i.e. javareg /register /class:MyTest /progid:MyTest
if everything is well-done then you should see a MessageBox displayed with
Succesfull register Class message.
Otherwise, you must check the correct spelling on the command line.
Now, the next step, copy the new Java class file that was generated.
MyTest.class
and paste in C:\Winnt\Java\Trustlib\ folder
if you have windows 98, this folder may change.
And the last step, open a New Project on Visual Basic.
And paste this brief code on the Form Load event for example and run it.
 Set x = CreateObject("MyTest")
 MsgBox x.myfunction(1, 1)
Congratulations !!!
you can use Java Class from Visual Basic.
Please do not forget to vote for this article. =)
```

