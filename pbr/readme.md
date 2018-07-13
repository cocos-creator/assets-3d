### More PBR resources

[IBL light probes](http://www.hdrlabs.com/sibl/archive.html)

[Materials](https://freepbr.com/)

### Convert equirectangular light probes into seperated cubemaps
Seperated cubemap is the only supported format for IBLs(for now), and you can convert between common formats using photoshop and [HDRShop](http://www.hdrshop.com/).

### Convert HDR textures into the supported RGBE pngs
PBR pipeline really shines when using HDR textures, and for now we only support HDR textures stored in RGBE png format, which you can convert into using [hdrpng.js](https://enkimute.github.io/hdrpng.js/).

And finally we provide a standalone converter which takes a equirectangular HDR light probe and directly output all the RGBE pngs needed for IBL(environment maps, convoluted diffuse maps and 7 levels of specular mipmaps):

[IBL converter](https://github.com/YunHsiao/ibl_convert)

The standalone converter is used to generate the IBLs in this folder, and as the baseline test for PBR materials.
