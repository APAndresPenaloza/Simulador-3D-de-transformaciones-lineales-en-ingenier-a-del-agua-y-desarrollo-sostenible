# Simulador 3D de transformaciones lineales en ingeniería del agua y desarrollo sostenible

Simulador web interactivo que modela tres sistemas hídricos como transformaciones lineales **T(x) = Ax**, con su informe de proyecto en normas APA 7 y su manual de usuario.

| | Enlace |
|---|---|
| Simulador | https://apandrespenaloza.github.io/Simulador-3D-de-transformaciones-lineales-en-ingenier-a-del-agua-y-desarrollo-sostenible/ |
| Informe del proyecto (APA 7) | https://apandrespenaloza.github.io/Simulador-3D-de-transformaciones-lineales-en-ingenier-a-del-agua-y-desarrollo-sostenible/informe.html |
| Manual de usuario | https://apandrespenaloza.github.io/Simulador-3D-de-transformaciones-lineales-en-ingenier-a-del-agua-y-desarrollo-sostenible/manual.html |

## Módulos

1. **Red de distribución** – matriz de incidencia nodo‑tubería. El núcleo son las circulaciones en los ciclos y el rango refleja la conectividad.
2. **Embalse** – cadena de Markov de niveles de almacenamiento. El autovector de λ = 1 es el estado de largo plazo.
3. **Planta de tratamiento** – matriz de mezcla y transferencia. Si todos los autovalores cumplen |λ| < 1, la planta atenúa cualquier pulso.
4. **Informe con QR** – genera un informe imprimible (PDF o HTML) con los resultados actuales y un código QR que reabre exactamente la misma simulación.

Cada módulo incluye vista 3D (three.js), editor de matriz con recálculo inmediato (acepta punto o coma decimal), panel de propiedades con interpretación física, escenarios de sostenibilidad ligados al ODS 6 y exportación en CSV y JSON. Al abrir la página, una validación interna repite 17 cálculos de referencia.

## Novedades de la versión 2.0

- Pestaña **Informe con QR**: datos del autor, selección de sistemas y contenidos, vista previa, impresión o PDF, descarga en HTML, QR en PNG y enlace copiable.
- Enlaces reproducibles: el escenario completo viaja en el fragmento de la URL (`#sim=1&m=...`). Al abrir el enlace o escanear el QR, el simulador carga los mismos valores y muestra un aviso con la opción de volver a los casos base.
- Edición de matrices y vectores en vivo, con coma o punto decimal y avance con Enter.
- Informe del proyecto y manual de usuario publicados en el sitio, con versiones en PDF y Word.

## Archivos

| Archivo | Contenido |
|---|---|
| `index.html` | Simulador completo |
| `informe.html` | Informe del proyecto (versión web) |
| `manual.html` | Manual de usuario (versión web) |
| `documentos.css` | Estilos del informe y del manual |
| `three.min.js` | three.js r128 (licencia MIT) |
| `qrcode.js` | qrcode-generator 1.4.4 de Kazuhiko Arase (licencia MIT) |
| `img/` | Capturas, figuras y códigos QR |
| `informe_transformaciones_lineales_agua.pdf` / `.docx` | Informe en normas APA 7 |
| `manual_usuario_simulador.pdf` | Manual de usuario para imprimir |

## Uso sin conexión

Descargue el repositorio (**Code → Download ZIP**), descomprímalo y abra `index.html`. Los archivos `three.min.js` y `qrcode.js` deben quedar en la misma carpeta. Los códigos QR apuntan siempre a la dirección pública del sitio.

## Publicar una copia propia

1. Haga un *fork* del repositorio.
2. En **Settings → Pages** elija **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
3. El sitio quedará en `https://<usuario>.github.io/<repositorio>/`. Los QR de su copia usan automáticamente esa dirección.

## Privacidad

Todos los cálculos y los informes se generan en el navegador; el sitio no tiene servidor ni base de datos. El código QR contiene solo la dirección del simulador y los valores numéricos de la simulación, no el nombre del autor ni sus observaciones.

## Cómo citar

Peñaloza Fernández, A. M. (2026). *Simulador 3D de transformaciones lineales en ingeniería del agua y desarrollo sostenible* (Versión 2.0) [Software]. GitHub. https://apandrespenaloza.github.io/Simulador-3D-de-transformaciones-lineales-en-ingenier-a-del-agua-y-desarrollo-sostenible/

«QR Code» es una marca registrada de DENSO WAVE INCORPORATED.
