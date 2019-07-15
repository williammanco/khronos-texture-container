# khronos-texture-container

Ported from
[babylon.khronosTextureContainer - Babylon.js](https://threejs.org/examples/jsm/loaders/KTXLoader.js)
[KTXLoader - Three.js](https://threejs.org/examples/jsm/loaders/KTXLoader.js)

## Install

```sh
yarn add khronos-texture-container
```

## Example

```js
import KhronosTextureContainer from 'khronos-texture-container'

const ktx = new KhronosTextureContainer( buffer, 1 );

console.log({
  mipmaps: ktx.mipmaps( loadMipmaps ),
  width: ktx.pixelWidth,
  height: ktx.pixelHeight,
  format: ktx.glInternalFormat,
  isCubemap: ktx.numberOfFaces === 6,
  mipmapCount: ktx.numberOfMipmapLevels
});

```

## Build

```sh
yarn build
```

# License

MIT