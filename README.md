# Symfony3 Blog

## Commands

A Symfony project created on December 8, 2016, 2:23 pm.

Curso 1 symfony 3.2 
08/12/16 
inicio 14:00 fin 15:15 pm

Resumen: instalacion de synfony, crear proyecto desde 0, conexion a bd y generar entidades con "annotation".

//pagina oficial
http://symfony.com/

//descarga 
http://symfony.com/download

//diferencia entre $ y # es el root


    //Installation on Linux and Mac OS X
    $ sudo curl -LsS https://symfony.com/installer -o /usr/local/bin/symfony
    $ sudo chmod a+x /usr/local/bin/symfony

    //actualizar version de synfony
    $ symfony self-update

    //descarga la ultima version en limpio
    $ symfony new blog
    $ symfony new blog 2.8 // para especificar la version de S que queremos instalar

    //version de symfony
    $ php bin/console --version

    // para iniciarlo en el puerto
    $ php bin/console server:start -p6000
    
    // para darle stop al proyecto
    $ php bin/console server:stop -p6000

    // para iniciarlo en el puerto
    $ php bin/console server:start -p9000


//desde phpstorm
instalar plugin de symfony, phpannotation, .ignore y reiniciar la maquina 

//sin pide configurar plugin le dan en auntomaticamente y psr-0

//abrir carperta de proyecto var/cash clic izquiero "Mark Directory" pinchar excluded

/app/

config/ 
configuraciones basicas del proyecto

crear schema y usuario 

    //Crear entidades
    $ php bin/console doctrine:generate:entity AppBundle:Category

    //me dice que voy a insertar en BD
    $ php bin/console doctrine:schema:update --dump-sql

    //actualizar las entidades en workbench
    $ php bin/console doctrine:schema:update --force

    //inicializar git en nuestro proyecto
    $ git init

    // agregar todo
    $ git add --all

    //agregar el commit 
    $ git commit -m'SEED'

## Homework

Crear la relación de manyToOne de Category a Post 
y la inversa de oneToMany de Post a Category.

[Link](http://ormcheatsheet.com/#association)