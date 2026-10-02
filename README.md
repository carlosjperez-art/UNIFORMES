# Uniformes Farmatodo

Seguimiento de pedidos de uniformes por familia de prendas: stock Cendis, SKUs en cero con sugerencia de compra, pedidos por unidad de RRHH y cronograma de entregas.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La página. Todos ven la misma; quien tenga la clave entra como administrador. |
| `datos.json` | Los datos compartidos (stock y pedidos). La página lo actualiza sola cuando un administrador hace cambios. |
| `.nojekyll` | Hace que GitHub publique los cambios más rápido. No lo borres. |

## Cómo se usa

- **Ver:** abre el enlace de GitHub Pages. La página revisa cada minuto si hay datos nuevos y se actualiza sola.
- **Editar:** pulsa **Entrar como administrador** y escribe la clave. Aparece la pestaña **Actualizar datos** para cargar el stockstatus y los pedidos en Excel.
- **Publicación automática:** se conecta una sola vez en *Actualizar datos > Publicación en GitHub* con un token de GitHub. Desde ahí cada cambio se guarda solo en `datos.json`.

## Token de GitHub (una sola vez)

1. En GitHub: foto de perfil > **Settings** > **Developer settings** > **Personal access tokens** > **Fine-grained tokens** > **Generate new token**.
2. Nombre: `uniformes`. Vencimiento: el máximo que permita tu cuenta.
3. **Repository access:** *Only select repositories* > elige este repositorio.
4. **Permissions** > **Repository permissions** > **Contents:** *Read and write*.
5. **Generate token**, cópialo y pégalo en la página. Se guarda cifrado con la clave de administrador.

Cuando el token venza, genera uno nuevo y vuelve a conectarlo.
