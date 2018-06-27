Kotlin : (Java -> Kotlin)
# kotlin-notepad 
Takeaways from this : https://classroom.udacity.com/courses/ud888 course 


**Some noticeable changes :**
- keyword fun 
- ? marks
- args and return type declarations are suffixe
- val (immutable- cannot be re-assigned)
- var can be re-assigned/ mutable
  eg:     var a : int? = null
  private var recycler: RecyclerView? = null

**whats more ??**
- no need of lengthy getters and setters
- lambda expression (interface with single methods converted to expression)
- switch statement changed to "when expression" -> can return value , also if , while, try-catches

**extension functions by using "apply plugin: 'kotlin-android-extensions" :** 
- It allows you to extend an existing class with new functionality
- all layout files changed to synthetic source files that contain exensions vals for every view that has id
- id becomes name of the val
- !! for nullability check not required as we are not using findViewById explicitly

**Kolin data class construct**
- It tells compiler to take care of identity, hashing copying for you.
- It takes all variables from class' constructors and use them to generate class' identity
- The way you get field wise copy constructors
- Data Classes generates (Copy constructors, hashcode, equals) BUT NOT Serialization logic 

**Check out Anko library**


**String interpolation :**
- embed Variables and expressions inside the string

**lateinit :**
To indicate compiler, I promise this variable will be initialized when I need to use it

**@JvmStatic :**
- Kotlin compiler avoid static variables wherever possible
- It nests it inside Companion or Insatnces objects
- @JvmStatic makes it represent such variables/methods java friendly

**apply : check this out**
