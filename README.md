# vr-inoshi

- [VRイノシシ](https://code4fukui.github.io/vr-inoshi/)
- [VRイノシシ背景付き](https://code4fukui.github.io/vr-inoshi/#bg)
- [VRイノシシ テクスチャーサイズ比較 256px vs 1024px](https://code4fukui.github.io/vr-inoshi/tx256.html)

## tool

### glTF-Transform

- [glTF-Transform](https://github.com/donmccurdy/glTF-Transform)

setup
```sh
npm install --global @gltf-transform/cli
```

convert
```sh
gltf-transform optimize inoshi1.glb inoshi1-opt-draco.glb --texture-compress webp
# 356kb (gzip -> 345kb)
gltf-transform optimize inoshi1.glb inoshi1-opt.glb --texture-compress webp --compress false
# 687kb (gzip -> 338kb gzip < draco+gzip!)
gltf-transform optimize inoshi1.glb inoshi1-opt.glb --texture-compress webp --compress false --texture-size 1024
# 490kb
gltf-transform optimize inoshi2.glb inoshi2-opt.glb --texture-compress webp --compress false --texture-size 1024
# 281kb
```

### gltfbeauty

- [gltfbeauty](https://github.com/code4fukui/gltfbeauty)

## オープンデータ

- 3Dデータ(USDZ/GLB) CC BY [PCN北はりま](https://kitaharima.pcn.club/)
