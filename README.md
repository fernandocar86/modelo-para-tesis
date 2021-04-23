# Descripción
Este repositorio contiene un modelo para armar una tesis o libro de lingüística con LaTeX. El proyecto contiene varios paquetes que pueden ser de utilidad para trabajos lingüísticos y varias opciones configuradas de antemano, para ahorrar el trabajo de armar un proyecto LaTeX desde cero. Para quienes precisen, en <a href="https://sites.google.com/view/grupodepln/cursos-de-extensi%C3%B3n/cursada-2019/cronograma-de-clases-y-materiales-curso-latex-2019?authuser=0">este link</a> hay materiales de un curso de LaTeX.

## Carpeta tramites

Esta carpeta está pensada para guardar allí todos los documentos ligados a las instancias burocráticas asociadas a una tesis o libro y que resulta útil conservar en el mismo repositorio.

## Carpeta Biblio-y-paquetes

Esta carpeta está pensada par contener los estilos bibliográficos (en extensión bst), la base de datos bibliográfica (en extensión bib) y los paquetes especiales (en extensión sty). Actualmente, esta carpeta contiene algunos archivos de modelo y el paquete avm, que es útil para construir diagramas de atribución de valores.

## Carpeta capitulos

Esta carpeta contiene los archivos tex de cada capítulo. 

## Carpeta Imagenes
Esta carpeta está pensada para guardar en ella las imágenes. Recordar que si se usa la compilación LaTex + Bib(la)tex + LaTeX(x2) + dvips+ pvs2pdf + ver pdf, requerida para incluir gráficos con tikz, las imágenes deben estar en formato eps

## Documento tesis-main

Contiene la estructura básica de la tesis/libro.

## Script remove-aux-files.sh

El archivo remove-aux-files contiene un script de bash para borrar todos los archivos auxiliares de crea LaTex en el directorio principal y en sus subdirectorios (pero no en los directorios que contengan las subcarpetas de la principal), en caso de que se quiera limpiar la copia local del repositorio. El script no elimina los archivos en pdf, tex, bib, bst, png, eps, jpg, entre otros.

