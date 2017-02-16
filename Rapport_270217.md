#Rapport 

                                     

                              Authors LingMA QianqianSHA 
                                      fait le 27/01/2017
##Contenu

Ce semaine nous avons apris le week trois de pharo. 

{\rtf1\ansi\ansicpg936\cocoartf1504\cocoasubrtf810
{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 Week3 \
3.1\
objects :Understanding of message passing / the beauty of pharo.\'92s implementation.\
Context: Booleans \
	&,|,not\
        or, and\
        ifTrue:ifFalse: ifFalse:ifTrue:\
       false not\
        ->true\
       true not\
       ->false\
  The solution uses three classes:\
  true is the singleton instance of True\
  false is the singleton instance of False\
  \
In OPP ,choice is expressed\
By defining classes with compatible methods\
By sending a message to an instance of such class\
\
Example \
  x open\
\
x can be a file, a window, a tool\
The method is selected based on x\'92s class\
true |  anything ->true\
 \
3.3 variable\
     local variables start with lowercase(temps,instance,variables,arguements)\
     shared variables start with uppercase (class, class variables)\
     special variables can\'92t be changed(true, false,nil(undefinedObject),self,super,thisContext)\'97\'97just 6\
\
3.4 simple http application\
  Class name starts with an uppercase\
  new is a message sent to the class Znclient\
  url: and get are both sent to the instance of ZnClient\
\
ZnClient new\
  url:\'92 http://localhost;8181/books/1\'92\
  get\
\
Configuring a Server\
 |books teapot|\
 books:=Dictionary new .\
 teapot :=Teapot configure:\{ #defaultOutput->#json. #port ->8181.#debugMode->true\}.\
\
 3.6 class method\
  1. in pharos ,everything is an object\
  2. objects can receive messages\
  3. classes are objects too \
  ex : FileLocator workingDirectory\
         ZnEasy getPng:\'92http://pharo.org\'92\
         ZnServer startDefaultOn: 8080\
 \
3.7  Collections\
OrderedCollection(dynamically growing)\
Array(fixed size,direct access)\
Set\
Dictonary\
\
Array new: 4\
>#(nil nil nil nil)\
(OrderedCollection new:1000)\
\
\
Arrays 1.Fixed size collection 2.Direct access:at and at; 3. put Has literal syntax \
\
\
\
\
}
