# Proyecto de ejemplo

Este es un proyecto de ejemplo para ilustrar el flujo de trabajo con ramas en Git.

## Ramas

- **main**: rama principal del proyecto.
- **rama1**: rama que se quiere unir a `main`.
- **rama2**: rama que parte de `rama1` y realiza modificaciones adicionales.

## Flujo de trabajo

1. Crear `rama1` a partir de `main`:
   ```bash
   git checkout -b rama1 main
   ```

2. Realizar cambios en rama1 y hacer commits:
```bash
Copiar código
git add .
git commit -m "Cambios en rama1"
```

3. Crear rama2 a partir de rama1:
```bash
bash
Copiar código
git checkout -b rama2 rama1
```

4. Realizar cambios en rama2 y hacer commits:
```bash
Copiar código
git add .
git commit -m "Cambios en rama2"
```

5. Fusionar rama2 en rama1:
```bash
Copiar código
git checkout rama1
git merge rama2
```

6. Fusionar rama1 en main:
```bash
Copiar código
git checkout main
git merge rama1
```


## Notas
- Este flujo permite que los cambios de rama2 se integren primero en rama1 y luego en main.

- Se pueden resolver conflictos durante los merges si es necesario.


## MODIFICACIONES
- Modificación realizada por rama1
- Quiero crear un conflicto desde rama2