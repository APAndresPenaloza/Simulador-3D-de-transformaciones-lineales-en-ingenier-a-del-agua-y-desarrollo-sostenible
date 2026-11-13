# Simulador 3D de transformaciones lineales en ingeniería del agua

Simulador web interactivo que modela tres sistemas hídricos como transformaciones lineales T(x) = Ax:

1. **Red de distribución** – matriz de incidencia nodo‑tubería (núcleo = ciclos, rango = conectividad).
2. **Embalse** – cadena de Markov (autovector de λ = 1 = estado estacionario).
3. **Planta de tratamiento** – matriz de mezcla y transferencia (autovalores < 1 = atenuación).

Cada módulo incluye vista 3D (Three.js), editor de matriz, panel de propiedades con interpretación física, escenarios de sostenibilidad (ODS 6) y exportación CSV/JSON.

## Archivos

- `index.html` – simulador completo (HTML + CSS + JavaScript).
- `three.min.js` – biblioteca Three.js r128 (licencia MIT). Debe estar en la misma carpeta que `index.html`.

## Publicar en GitHub Pages

1. Cree un repositorio público (o use uno existente) y suba `index.html`, `three.min.js` y este `README.md` a la raíz (*Add file → Upload files*).
2. En **Settings → Pages**, seleccione *Deploy from a branch*, rama `main`, carpeta `/ (root)` y guarde.
3. En uno o dos minutos el simulador queda en `https://<usuario>.github.io/<repositorio>/`.

Para incluirlo dentro de un repositorio que ya tiene otro `index.html`, suba los archivos a una subcarpeta (por ejemplo `algebra-lineal/`); la dirección será `https://<usuario>.github.io/<repositorio>/algebra-lineal/`.

## Uso sin conexión

Abra `index.html` directamente en el navegador. No requiere instalación ni servidor.

## Validación

Al cargar, la función `validar()` comprueba 17 resultados de los tres casos base contra valores de referencia calculados de forma independiente y muestra el resultado en la parte superior.
