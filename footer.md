% This defines the footer of the site, and is not parsed as a regular "page"
% We point to it with the following in `myst.yml`:
% site:
%   parts:
%     footer: footer.md

% Here we use `grid` to add a basic grid structure to the HTML,
% but the formatting column sizes are defined manually in css/footer.css
% see the `grid-template-columns` line.
:::::{grid} 3 3 5 5
:class: outer-grid col-screen

<!-- Left spacer -->
::::{div}
::::

<!-- Project description -->
::::{div}

# Landing Pages

```{image} https://jupyterbook.org/en/stable/_images/logo-square.svg
:width: 50px
:align: left
```

This is a description of our project. And a [link to its homepage](https://github.com/jupyter-book/example-landing-pages).
::::

<!-- Spacer between project description and links columns -->
::::{div}
::::

<!-- Link columns -->
% This a *second* grid embedded within the first one, to create nicer
% responsive design experience. This grid will have a single column on narrow screens,
% and fan out into three columns on wide screens. However, it always remains within
% its parent grid column.
::::{grid} 1 1 3 3

:::{image} notebooks/images/logos/NSF-NCAR_Lockup-UCAR-Dark_102523.svg :height: 256px :::
:::{div}

- [About](https://mystmd.org/overview/ecosystem)
- [Guide](https://mystmd.org/guide)
- [Sandbox](https://mystmd.org/sandbox)
:::

:::{div}

- A second column!
- With multiple entries
:::

:::{div}

- And what about a third

footer_logos:

:::


::::



<!-- Right-most spacer -->
::::{div}
::::

:::::