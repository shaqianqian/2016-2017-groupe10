

#Rapport 

                                     

                              Authors LingMA QianqianSHA 
                                      fait le 03/02/2017
##Contenu

This week we began to programmer the website by pharo.  After learning the basic knowledge and grammar about Pharo . We knew this editor can use to build a website.  We used to learn HTML5
and CSS . So we decided to combine the old knowledge with this new tool.  We chose the project  Ecstatic, where we need to learn the usage of pillar. Pillar is a markup language to describe the page. It is written in pharo.
  We used these commands to run the .pillar 	and changed it to .html . This project gave us some themes ,and we opened them successfully. 



##step 1
To see a full list of available commands

>ecstatic --list

parallels@ubuntu:~/Desktop/Projet$ ls
ecstatic
parallels@ubuntu:~/Desktop/Projet$ mkdir mysite
parallels@ubuntu:~/Desktop/Projet$ cd mysite/
parallels@ubuntu:~/Desktop/Projet/mysite$ ../
ecstatic/ mysite/
parallels@ubuntu:~/Desktop/Projet/mysite$ ../ecstatic/ecstatic createsite
Website structure generated at: /home/parallels/Desktop/Projet/mysite
parallels@ubuntu:~/Desktop/Projet/mysite$ ls
index.pillar  pillar.conf  README.txt
parallels@ubuntu:~/Desktop/Projet/mysite$ ../ecstatic/ecstatic generate
Copying source files to /home/parallels/Desktop/Projet/mysite/_site ...OK
Generating html files...OK
Website successfully generated
parallels@ubuntu:~/Desktop/Projet/mysite$ ls
index.pillar  pillar.conf  README.txt  _site
parallels@ubuntu:~/Desktop/Projet/mysite$ ls _site/
index.html  index.pillar  pillar.conf  README.txt


###step 2
$../ecstatic/ecstatic theme candy
Theme candy installed successfully
$ ../ecstatic/ecstatic generate
Copying source files to /home/l3/sha/Bureau/Projet/mysite/_site ...OK
Generating html files...OK
Website successfully generated
$ ../ecstatic/ecstatic serve
Serving website at: http://localhost:8080/

  Then we opened the website in http://localhost:8080.  Every time we changed the theme and refresh the page we could get a new one . It was very interesting.

  After having a general knowledge of the pillar. We started to design our own website. We decided to make a blog where the people can put their articles .
  We painted the structure as our conception, and then chose our logo. 
  This week we will begin to write the codes of html and css. 



  For knowing about the pharo better , we stilled watched the videos in mooc 
