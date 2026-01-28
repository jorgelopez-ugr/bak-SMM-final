CLASE 2 DE PRACTICAS:

El boton y el propio frame, ambos son seleccionables, son "generadores"

cada generador tiene definidas muchas acciones, cada accion puede tener un comportamiento

para tocar cosas sobre el estilo tenemos que tocar en donde pone Form arriba del todo del arbol

cambiamos el listener generation style de anonymous a inner

el estilo de la clase anonima es mas limpio y se ve menos codigo pero es mas dificil de entender

seleccionas el generador > eventos > el evento que nos interese, en este caso clic en el mouse, nos genera un codigo automaticamente
pues lo que metamos en ese metodo sera el comportamiento que ocurre.

el manejador se llama FormListener, es ina private class y tiene 5 metodos

si cambias de generador te crea una clase nueva?

para el dragged usa la misma clase que antes y le pone un nuevo implements y eso fuerza a poner en codigo
los dos metodos de la interfaz que serian el dragged y el moved que son los que pertenecen a lo que acaba de implementar

al ser un evento distintos necesita un listener nuevo por eso si vamos donde los listeners sale uno nuevo

no se permite herencia multiple en java por eso no puedes heredar de uno y heredar de otro. Es por eso que ha usado la opcion de implements

diferencia entre el clicked y el action performed:
    - el accion es el hecho de actuar sobre ese boton, independientemente de como. Ya sea con el raton, con el teclado, con lo que sea
    actuar sobre el lanza el codigo de accion. Primero se lanza la accion y luego el comportameinto, por ejemplo, asociado al mouse clicked
    
método paint. Es el que dibuja los objetos, padres llaman al paint de hijos
esta implicito pero nosotros podemos overridearlo si queremos obtener comportamientos especiales

    @Override 
    public void paint(Graphics g){
        super.paint(g);
    }
    
en principio eso seria similar a lo que ya hay, llamar al paint del padre
siempre el paint lo hacemos igual. siempre lo empezamos llamando al del padre

importante llamar al del padre el principio para que se dibuje la ventana en si, luego 
con el objeto g de graphics podemos dibujar cualquier cosa, por ejemplo un óvalo.




