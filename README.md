# creater-groupadd-useradd
#!/bin/bash
Echo "Iniciando la creacion del grupo y sus usuarios"


# Crear el usuario Armida
useradd -m -d /home/Arminda -s/bin/bash Arminda

# Crear el usuario Geovany
useradd -m -d /home/Geovany -s/bin/bash Geovany

# Crear grupo ComFamilia
groupadd ComFamilia

# Agregar usuario Arminda al grupo ComFamilia
Usermod -a -G ComFamilia Arminda

# Agregar usuario Geovany al grupo ComFamilia
Usermod -a -G ComFamilia Geovany 

 Echo "el grupo y usuarios creados con exito"
