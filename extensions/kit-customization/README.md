## Hierarchy
- Layout
- Blocks
- Components
- Elements
- Utils

## Tasks
- [ ] Create a mockup of the kit customization page.
- [ ] Create snippets for the components of the kit customization page.
    - [ ] Core UI
    - [ ] Stylish
    - [ ] Implement Javascript for the components.
- [ ] Create snippets for the utils used in the kit customization page.
    - [ ] Core UI
    - [ ] Stylish
    - [ ] Implement Javascript for the utils.

### Notes
  - En los snippets si importamos el archivo CSS luego no se lee al hacer un render dentro de otro snippet o block porque shopify unicamente lee el CSS de los block porque los inserta en el head del HTML. Por eso estamos usando para componentes chicos el CSS de los snippets dentro de las etiquetas `<style>`.
  - Los snippets van a ser los distintos componentes choose player, choose size, choose equipment, etc.
  - Los blocks se van a usar para agrupar los snippets como si fuese un layout establecido por los snippets, por ejemplo un block (layout) de kit customization para la PDP y otro block (layout) para la home page. (Lo hacemos asi para asegurar que el block (layout) contenga todos los snippets y estos funcionen en conjunto y con el template que deseamos).

### Snippets
#### Components
- [] Kit Media (Render)
- [] Kit Customization 
    - [] Kit Equipment (Products)
        - [] Equipment Item
        - [] Mock Products
    - [] Kit Sizes
        - [] Size Item
        - [] Mock Sizes
        - [] Modal Sizes Guide
    - [] Kit Personalization
        - [] Player list
        - [] Custom Player
        - [] Mock Player Options
    - [] Kit Competitions
        - [] Mock Competitions
    - [] Kit Add to Cart
#### Utils
- [] Titles (H1, H2, H3, H4, H5, H6) 
- [] Toggle Switch 
    - [] Default Radio Selector 
        - [] Disabled Style and Bell Icon
    - [] Personalization Double Options 
- [] Selector
- [] Input text
- [] Input number
- [] Price Text (option format example: "132,98 €", "+20€")