# Corewar

Ce projet clôture la fin de ma première année pour la partie algorithmique.

Il est réalisé en C, essaye de répliquer le comportement d'une machine virtuelle et un assembleur.

Il permet de réaliser des combats de champion au sein d'une VM, ou les champions utilisé sont compilé par l'assembleur.

## Résultat

### Assembleur

<div style="display: flex; flex-wrap: wrap">
    <img src="/images/asm/asm.png" width=500 height=786 />
</div>

### Machine Virtuelle

<div style="display: flex; flex-wrap: wrap; flex-direction: column">
    <img src="/images/vm/vm.png" width=300 height=42 />
    <img src="/images/vm/vm_memory.png" width=500 height=450 />
</div>

### Partie Graphique

https://github.com/Noa-Trachez/Corewar/assets/74274767/4da7047d-3064-4b97-9ce9-af08ca48e9e9

### Application Mobile + Serveur Python

<div style="display: flex; flex-wrap: wrap; flex-direction: column">
    <img src="/images/app/server.png" width=300 height=60 />
    <img src="/images/app/app.png" width=400 height=760 />
</div>

## Essayer le projet

### Prérequis

ASM - VM:
```
- C
- make
```

Graphique:
```
- C
- CSFML
- make
```

Mobile:
```
- Flutter
- Python
```

### Lancer le projet
ASM:
```bash
make
./asm/asm -h
./asm/asm file_name[.s]
hexdump -C file_name[.cor]
```
Des fichiers de test sont disponibles dans : tests/asm/functional/tests/

VM:
```bash
make
./corewar/corewar -h
./corewar/corewar file_name[.cor] file_name[.cor]
```
Des fichiers de test sont disponibles dans : tests/corewar/cor_binary/

Graphique:
```bash
cd bonus/corewar_graphic
make
./gcore
```
Si vous voulez tester vos champions, mettez les dans le dossier champions/

Mobile:
```bash
cd bonus/corewar_app
BUILD Flutter app on your phone
./server/run.sh
```
