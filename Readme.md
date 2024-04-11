# Corewar

Ce projet clôture la fin de ma première année pour la partie algorithmique.

Il est réalisé en C, essaye de répliqué le comportement d'une machine virtuelle et un assembleur

Il permet de réalisé des combats de champion au seins d'une VM, ou les champions utilisé sont compilé par l'assembleur

## Résultat

### Assembleur

<div style="display: flex; flex-wrap: wrap">
    <img src="/images/asm/asm.png" width=500 height=786 />
</div>

### Machine Virtuelle

<div style="display: flex; flex-wrap: wrap">
    <img src="/images/vm/vm.png" width=300 height=42 />
    <img src="/images/vm/vm_memory.png.png" width=500 height=450 />
</div>

### Partie Graphique

### Application Mobile + Serveur Python

<div style="display: flex; flex-wrap: wrap">
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
Des fichiers de test sont disponnible dans: tests/asm/functional/tests/

VM:
```bash
make
./corewar/corewar -h
./corewar/corewar file_name[.cor] file_name[.cor]
```
Des fichiers de test sont disponnible dans: tests/corewar/cor_binary/

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