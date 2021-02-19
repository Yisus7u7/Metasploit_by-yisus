# Metasploit_by-yisus
Este instalador instalará Metasploit en termux solucionando el error de ruby 3.0.0 

Termux actualizo ruby a la versión 3.0.0, Metasploit funciona con ruby 2.7.2, 
Pero yo e encontrado solucion al problema, sigue 
estos pasos:

SIGUE LOS SIGUIENTES PASOS EN ORDEN :
!es recomendable usar Android 7 en adelante!

#ruby 2.7.2

primero eliminamos la versión 3.0.0 de ruby:

pkg uninstall ruby

Ahora añadiremos el repositorio de hbhacker
(Gracias abhacker por mantener una compilación
de ruby en tus repositorios!!)

pkg install curl 

bash -c "$(curl -fsSL https://bit.do/abhacker-repo)"

Nota (si estas usando fish o zsh cambia tu 
terminal a bash)

Luego actualizamos:

pkg update && pkg upgrade 

Ahora instalanos ruby 2.7.2 :

pkg install ruby2

# exelente

ahora comprobamos que tenemos ruby 2.7.2 :

ruby --version

Nos debe salir esto :

⋊> ~ ruby --version                                09:25:39
ruby 2.7.2p137 (2020-10-01 revision 5445e04352) [arm-linux-androideabi]

con que salga 2.7.2 ya todo va correcto

#instalación de Metasploit

Primero clone este repositorio 

cd $HOME

git clone https://github.com/Yisus7u7/Metasploit_by-yisus 

chmod +x ~/Metasploit_by-yisus/*

mv ~/Metasploit_by-yisus/Metasploit.sh $HOME

Ahora ejecute :

bash metasploit.sh

O

./metasploit.sh



