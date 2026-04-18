# Generador de Contraseñas Seguras

Este proyecto es una herramienta sencilla hecha en Node.js que permite generar contraseñas seguras de manera rápida desde la terminal.

Está pensado para usuarios que necesiten crear claves seguras para proteger información.

---

## ¿Qué hace este programa?

El programa genera una contraseña automática según las opciones que el usuario defina, como:

- Longitud de la contraseña
- Uso de números
- Uso de símbolos

También permite guardar la contraseña en un archivo de texto.

---

## Requisitos

Antes de usar este programa necesitas:

- Tener instalado Node.js (versión 16 o superior)

Puedes verificar tu versión con este comando:

```bash
node -v
```

---

## Instalación

Sigue estos pasos para usar el proyecto:

1. Descarga o clona el repositorio:

```bash
git clone https://github.com/xxxxx/generador-pass-node.git
```

2. Entra a la carpeta del proyecto:

```bash
cd generador-pass-node
```

3. Instala las dependencias:

```bash
npm install
```

> Este paso es importante porque el proyecto usa una librería llamada `chalk` para mostrar colores en la terminal.

---

## Cómo ejecutar el programa

Para iniciar el programa escribe:

```bash
npm start
```

---

## Opciones que puedes usar

Puedes personalizar la contraseña usando los siguientes parámetros:

- `--longitud`: Define cuántos caracteres tendrá la contraseña  
- `--simbolos`: Indica si quieres incluir símbolos (true o false)  
- `--numeros`: Indica si quieres incluir números (true o false)  

---

## Ejemplo de uso

```bash
npm start -- --longitud=12 --simbolos=false --numeros=true
```

Esto generará una contraseña de 12 caracteres, sin símbolos y con números.

Ejemplo de resultado:

```
Tu nueva clave es: aB3dE8fG9hI1
```

---

## Guardar la contraseña en un archivo

Si quieres guardar la contraseña en un archivo, agrega el parámetro:

```bash
--guardar
```

Ejemplo:

```bash
npm start -- --longitud=12 --simbolos=true --numeros=true --guardar
```

Esto creará un archivo llamado:

```
mis_claves.txt
```

Donde se guardará la contraseña generada.

---

## Pruebas del sistema

El programa tiene una función para verificar que no se repitan contraseñas.

Para ejecutarla usa:

```bash
npm run test
```

---

## Recomendaciones

- Usa contraseñas de al menos 12 caracteres
- Incluye números y símbolos para mayor seguridad
- No compartas el archivo `mis_claves.txt`

---

## Licencia

Este proyecto es de uso libre bajo licencia MIT.

---

## Nota final

Este proyecto fue desarrollado como una herramienta práctica para mejorar la seguridad en la generación de contraseñas.