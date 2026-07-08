Proyecto desarrollado en Java enfocado en la implementación de una estructura de datos tipo lista enlazada.

Se creó una estructura propia utilizando nodos conectados mediante referencias, permitiendo administrar elementos dinámicamente sin depender de estructuras integradas del lenguaje.

El proyecto incluye operaciones para agregar elementos al inicio y final de la lista, eliminar elementos por índice o valor, modificar datos, consultar elementos específicos, obtener el tamaño de la lista y recorrer sus elementos mediante un iterador personalizado.


# List


//-------CODIGO PLANTUML------------------------------------
@startuml

title LinkedList - Class Diagram


+class uaslp.objetos.list.linkedlist.LinkedList {
  -Node head;
  -Node tail;
  -int size;
 
  +addAtTail (String data)
  +addAtFront(String data)
  +remove(index)
  +removeAll()
  +setAt(index, data)
  +getAt(index):String
  +removeAllWithValue(String data)
  +getSize();
  +getIterator(): LinkedListIterator
 

}

~class uaslp.objetos.list.linkedlist.Node{
   ~String data;
   ~Node next;
   ~Node previous;
}

+class uaslp.objetos.list.linkedlist.LinkedListIterator{
   +hasNext(): boolean;
   +next(): String;
}


@enduml
