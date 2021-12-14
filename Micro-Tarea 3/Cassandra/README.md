# Micro Tarea 3 - Ian Arias Schreiber y José Chavez
## Aspectos generales Cassandra
Cassandra es una base de datos distribuida NoSQL la cual es altamente escalable. Además, esta diseñada para poder manejar una gran cantidad de datos.

A diferencia de una base de datos relacional, Cassandra provee diferentes formas de almacenar datos y de una manera más simple.

### Características importantes
- Escalabilidad
- "Always on architecture", quiere decir que siempre está disponible.
- Desempeño rápido lineal, mantiene un tiempo de respuesta rápido.
- Almacenamiento flexible de la data, acepta data estructura, semi-estructurada y no estructurada.
- Distribución de data sencilla. 
- ACID (Atomicity, Consistency, Isolation, Durability)
- Lecturas y escrituras rápidas.

## Diseño
El objetivo de Cassandra es poder manejar big data a través de varios nodos sin tener fallas. La data es distribuida entre todos los nodos en un cluster.
### Características de un cluster Cassandra
- Todos los nodos son independientes y están conectados con otros. Además, todos cumplen el mismo rol.
- Cualquier nodo puede aceptar consultas de escritura o lectura, sin importar donde la data está ubicada en el cluster.
- Si un nodo cae, los otros harán su trabajo.

## Arquitectura
Cassandra tiene una arquitectura de anillo, en donde todos los nodos estan interconectados.
Una función fundamental de Cassandra es la replicación de la data en todos los nodos, en un cluster uno o más nodos actuan como replicas para cierta data.
Al haber varios nodos con la misma data, cuando se hace una consulta en la base de datos Cassandra retorna el valor actualizado recientemente y actualiza los otros nodos.

Una imagen representativa de la arquitectura:
![arquitecturaCassandra](../../imagenes/data_replication.jpg)

### Componentes principales de Cassandra
- Nodo: Lugar donde este guarda la data.
- Data center: Colección de nodos relacionados.
- Cluster: Componente que contiene uno o más data centers.
- Commit-log: Todas las operaciones de escritura se guardan en este log.
- Mem-table: Estructura de datos que permanece en memoria en todo momento, aqui se guarda la data de escritura.
- SSTable: Archivo en disco que guarda la data del Mem-table cuando esta llega a un cierto tamaño.
- Bloom filter: Algoritmos para revisar si un elemento está o no en un set.


![arquitecturaCassandr2a](../../imagenes/cassandra_architecture2.png)
