

#Rapport 

                                     

                              Authors LingMA QianqianSHA 
                                      fait le 20/01/2017
##Contenu
–--------------2.1--------------------
Il y 3 methodes pour minimize parentheses .
Cest un langage partique pour les enfants.

ordre: (Msg)>Unary>Binary>keywords
        begins with () then depends on the ordres

ex:
Unary 
1 class > smallinteger

false not>true

Data today
> 24 May 2009

Float pi
>3.141592653589793

there is no difference between sending a message to an object or to a class

1 class > smallinteger
Data today > 24 May 2009

ex :

1 log(unary)
Browser open (unary)
2 raisedTo:5(keyword)

10@20 setX:2
>2@20(we change the x value if the receiver (a point) No parentheses required)


#(‘Calvin’ ’hates’ ‘Suzie’) at:2 put :’loves’
>#(‘Calvin’ ‘loves’ ‘Suzie’)

#(…) creates an array
at:put:changes the value of the array element
arrays start at 1 in Pharo(first element is at index 1)

12 between:10 and:20
>true
the message between:and:is sent to an integer
Takes two arguments 10 and 20


Data today 27/June 2015





–--------------2.2--------------------
Comparee avec java
:
java(ArrayList<String> strings=new ArrayList<String>() ;)
In pharo (Strings:=OrderedCollection new.)

java(Thread regThread =new Thread(
    new Runnable(){
public void run(){
this.doSomething() ;
}
}
) ;

regThread.start() ;
}

))


in pharo


java
new Thread()→this.doSomething().start() ;

In pharo
[self doSomething] fork


Three kinds of Messages

Unary
5 factorial
Transcript cr


Binary
3+4
5 - >10

Keyword – based

Transcript show : “hello world”
2 between:0 and:5

In java
receive.keyword1keyword2(arg1,arg2)

In Pharo
anObject keyword1:arg1 keyword2:arg2

In java
postman.send(mail,recipient) ;
postman.send(mail.recipient) ;
postman send mail recipent
postman send mail to recipient



in java ,if,else,for,while.do … are langage keywords
in pharo ,conditional expressions are messages
booleans are objects

fullName isEmpty
 	ifTrue : [‘FirstnameLastname’]
 	ifFalse :[FullName]


4timesRepeat:[self doSomething]
- 0 to:100 do:[ : i |…]
- 0 to:100 by 3 do:[ : i |…]
aCollection do:[:each|…]


2.3
1000 factorial class name
(((1000 factorial )class )name)
lire de gauche a droite
ex :
2+3 squared
>2+9
>11


2.4

. est un seperator pas un terminator
when we give a message to a variable, we can just write one time the variable.

2.5
comment utiliser ‘finder’ dan l’editeur de pharo pour trouver  les methodes.

2.6 blocks[expressions…]
ex :
[2+4]value >6
[:x|x+2] values:2 >4
can use many times
[:x:y|x+y]value :5 value:7 >12

2.7 loops
1) loops timesRepeats
  4 timesRepeats:[self doSomething]  (repeter 4 fois)
2) loops :to:do
  1 to :100 do:
  [:1|...i...]
  to:by:do:
  1 to :100 by:3 do:
   whileTrue


2.8
Boolean

2.9 On peux utilsier les  parenthesesa  pour changer les ordres de caculeuts.
Using the cascade can avoid repeating same receiver many times, and it just
returns the last value.
2.10
self :return a new instance(receiver itself)
ex:
Weather isRaining
  ifTrue:[self takeMyUmbrella]
  ifFalse:[self takeSunglasses]


resume :
  Pharo est une langage trop simple , il a supprime beaucoup signaux et keywords
  dans Java ,et pres de une naturale langage ,cest tres pratique pour les informaticiens
  lisent et  codent par pharo. Faire la prgrammation de plus en plus simple est une
  tendance.

  Mais il ajoute les difficultes de rappeler les grammers. Comme un langage de Info,
  il est trop different, et on n'a pas beaucoup de livres ou ressoures a consulter.
  Et les fonctions de pharo cachent dans chaque button. Maîtriser pharo a besoin
  un nouveau moyen de reflechir.

  C'est un langage qui orienter les objects . Il a besoin un bonne base de Java.
   Pharo n’a pas le mathematical precedent .

   On va commencer de developer les websides par pharo. Ce sera un experience interessant ,
   c'est le premier fois pour nous d'utilser un nouvelle langage. Il va cout pluseurs temps
  pour Maîtriser ce langage. Et il peux nous aider de reviser coo de java aussi.

  Info est un scientifique qui developpe vite . Apprendre durablement est la qualite basique.
