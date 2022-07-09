# The Collision Detector
This uses VueJS's two-way binding for the interface. We have a HTML dashboard and a display space to show two rectangular objects. The `v-model` attribute implements the binding.

## Data
- `v`: a Boolean value that denotes if `objA` collides with `objB` vertically.
- `h`: a Boolean value that denotes if `objA` collides with `objB` horizontally.
- `collided`: a Boolean value that denotes if `objA` collides with `objB` on both vertical and horizontal planes.
- `objA` and `objB`:
    - `left`: the x-value of the top left corner
    - `top`: the y-value of the top left corner
    - `width`
    - `height`

## Methods
- `getCollision()`: displays "Yes" or "No" depending on the values of `v`, `h` and `collided`.
- `detectCollision()`: calculates `v` and `h`, and derives `collided` from those values.
