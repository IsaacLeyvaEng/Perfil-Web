GUIA DE CONTRIBUCION

Reglas para trabajar en este repositorio. Son pocas y se aplican siempre.

Ramas:
main: versión publicada. Solo recibe releases etiquetados.
develop: integración del trabajo terminado.
feature/N-nombre-corto: una rama por issue, creada desde develop. Ejemplo: feature/6-hello-world.
Nunca se hacen commits directos en main ni en develop.

Commits:
Formato: tipo: descripción, en inglés, en imperativo, en minúscula y sin punto final. Un commit por cada cambio lógico.
Tipos: feat, fix, docs, style, refactor, chore, ci.
style es solo formato del código, no los estilos CSS de la página.
Ejemplo: feat: add hero section markup

Pull Requests:
Base: develop.
Título: tipo: descripción (#N), donde N es el número del issue.
Descripción: Closes #N para cerrar el issue, o Refs #N para solo enlazarlo.
Integrar con merge commit y borrar la rama después.

Antes de subir cambios:
npm run format
npm run lint

El CI vuelve a comprobarlo en cada Pull Request.

Nomenclatura CSS (BEM):
Bloque: card
Elemento: card__title
Modificador: card--featured

html
<article class="card card--featured">
  <h3 class="card__title">Título</h3>
</article>
