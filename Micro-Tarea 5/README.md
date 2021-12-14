
# Micro Tarea 5 - Ian Arias Schreiber y José Chavez
## Creación de Nodo Minikube
Crear nodo donde se encontrarán los pods de estrés y prometheus para el monitoreo.
![Crear nodo](../imagenes/crearNodo.PNG)

## Instalar Prometheus
Instalación de prometheus usando HELM.
![promInstall](../imagenes/prometheusInstall.PNG)
Dashboard de prometheus después de hacer port-forward.
![promDash](../imagenes/promDashboard.PNG)
## Crear Pod de estrés
Creación de pod con consumo de 1 CPU usando la imagen stress-ng.
### Consumo de CPU
#### Imagenes del dashboard
![stress1](../imagenes/creacionStressTest.PNG)
![stress2](../imagenes/creacionStressTest2.PNG)
### Consumo de Memoria
Creación de pod con consumo de 250MB usando la imagen stress-ng.
#### Imagenes del dashboard
![stress3](../imagenes/yamlStress.PNG)
![stress2](../imagenes/creacionStressTest2.PNG)
## Monitoreo
Uso del CPU desde la creación del pod de estrés hasta su deleción.
### Consumo de CPU
![monitor1](../imagenes/monitoreoCPUSube.PNG)
![monitor2](../imagenes/monitoreoCPUBaja.PNG)
### Consumo de Memoria
Uso del CPU desde la creación del pod de memoria hasta su deleción.
![monitor3](../imagenes/memoryConsumptionSube.PNG)
![monitor4](../imagenes/memoryConsumptionBaja.PNG)

## Pensamientos finales
Creemos que Prometheus es una herramienta fácil de instalar y además útil y rápida al momento de hacer monitoreo. Provee una amplia cantidad de consultas de monitoreo a través de su lenguaje "PromQL" como uso de CPU, Memoria, Consultas HTTPS, entre otras. Por otro lado la posible integración de Grafana con Prometheus hace que la herramienta sea aún más útil y versatil.


