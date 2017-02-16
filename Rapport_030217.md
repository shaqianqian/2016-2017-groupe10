

#Rapport 

                                     

                              Authors LingMA QianqianSHA 
                                      fait le 03/02/2017
##Contenu
Cette semaine, nous avons appris les chose ci-desous

####The Basics
-often we want small adaptations
-we want to extend existing behavior and state, 
-solution: class ingeritance,for example, there is a rectangle,if we want to coloredRectangle, we creat a subclass herite the class rectangle to avoiding repeat the methods
(a class extends the definition of its superclass)
#####Root of interitance hierarchy
-Object is the root of the mosts classes
for exemple, ProtoObject which is the superclass of Object,is uesed fro special purposes
#####inheritance
it is  static for state and also dynamic for behabior
######The Inheritance of Instance variables
happens during class definition
computed form the class own instance variables and the ones of its superclasses
for exemple, the color() from color
###### inheritance of Behavior
happens at the runtime 
te method os searched
starting from the receiver's class
then going to the superclass
####t The usage of Intheritance
It allows a class to refine state and behavior.a class has one and only one superclass.and eventyally inherits from object.Inheritance of state is static but that of behavior is dynamic

####Look up
#####message sending 
it is a two-step process
1 look up the method matching the message
2 execute this method on the receiver
#####method lookup
starts in the class of the receiver then
-if the method is defined in the class.it is returned
-otherwise the search continues in the superclass

#####semantics of self
self always represents the receiver,send act as a hook: code of subclasses may be invoked
#####super
super refers to the receiver of the message,like self,the method lookup
starts in the superclass of the class containing the super expression,super changes the lookup: a super send starts the lookup in the class above it.
#####doesNotUnderstand: aMessage
it is a message, any class can implement tge correspongding method,used for automatic delegation,proxy,distribution.
it is also a debugger,when no class redefineds doesNotUnderstand, it is excuted in Object,the method raises a MessageNotUnderstood exception,and when not handled,this exception opens a debugger.

when no method is found in the hierarchy: doesNotUnderstand: is sent ot the receiver,the initial message is passed as a parameter
