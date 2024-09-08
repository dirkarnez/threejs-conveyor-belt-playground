[threejs-conveyor-belt-playground](https://dirkarnez.github.io/threejs-conveyor-belt-playground)
================================================================================================
```js
      ( function roundedRect( ctx, x, y, width, height, radius ) {

        ctx.moveTo( x, y + radius );
        ctx.lineTo( x, y + height - radius );
        ctx.quadraticCurveTo( x, y + height, x + radius, y + height );
        ctx.lineTo( x + width - radius, y + height );
        ctx.quadraticCurveTo( x + width, y + height, x + width, y + height - radius );
        ctx.lineTo( x + width, y + radius );
        ctx.quadraticCurveTo( x + width, y, x + width - radius, y );
        ctx.lineTo( x + radius, y );
        ctx.quadraticCurveTo( x, y, x, y + radius );

      } )( roundedRectShape, 0, 0, 50, 50, 20 );
```
https://github.com/mrdoob/three.js/blob/dev/examples/webxr_vr_rollercoaster.html
