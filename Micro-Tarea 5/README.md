
# Micro Tarea 5
## Creación de Nodo Minikube
Crear nodo donde se encontrarán los pods de estrés y prometheus para el monitoreo.
![Crear nodo](imagenes/crearNodo.png)

## Instalar Prometheus
Instalación de prometheus usando HELM.
![promInstall](imagenes/prometheusInstall.PNG)
Dashboard de prometheus después de hacer port-forward.
![promDash](imagenes/promDashboard.PNG)
## Crear Pod de estrés
Creación de pod con consumo de 1 CPU usando la imagen stress-ng.
### Consumo de CPU
![stress1](imagenes/creacionStressTest.PNG)
![stress2](imagenes/creacionStressTest2.PNG)
Creación de pod con consumo de 250MB usando la imagen stress-ng.
### Consumo de Memoria
![stress3](imagenes/yamlStress.PNG)
![stress2](imagenes/creacionStressTest2.PNG)
## Monitoreo
Uso del CPU desde la creación del pod de estrés hasta su deleción.
### Consumo de CPU
![monitor1](imagenes/monitoreoCPUSube.PNG)
![monitor2](imagenes/monitoreoCPUBaja.PNG)
### Consumo de Memoria
Uso del CPU desde la creación del pod de memoria hasta su deleción.
![monitor3](imagenes/memoryConsumptionSube.PNG)
![monitor4](imagenes/memoryConsumptionBaja.PNG)



