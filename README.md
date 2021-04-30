<h2 align="center">
    <img alt="Logo" src="https://www.bocusedor-winners.com/data/classes/actualite/actu_278_vignette.jpg" height=300></img><br>
    CESAR → <em>The Radical Compressor</em> ←
</h2>


<p align="center">
<a href="https://github.com/Kraymer/cesar/blob/master/LICENSE"><img alt="License: MIT" src="https://github.com/Kraymer/public/blob/master/brack/license.svg"></a>
<a href="https://ko-fi.com/kraymer"><img alt="Donate" src="https://img.shields.io/badge/-%E2%99%A1%20Donate%20-ff69b4"></img></a>
</p>

> **/t͡sêsaːr/** :
>
>   1. *n.* french sculptor at the forefront of the Nouveau Réalisme movement with his radical compressions
>   2. *n.* git pre-commit hook to compress images

### Description

`cesar` performs compression by calling external tools : `pngcrush` for PNG files and `jpegoptim` for JPEG files.

### Installation

Copy [`/cesar`](https://raw.githubusercontent.com/Kraymer/cesar/master/cesar) to your `.git/hooks/` folder and rename it as `pre-commit`.

Or if you use [pre-commit](https://github.com/pre-commit/pre-commit) framework, add this to your `.pre-commit-config.yaml` :

```yaml
-   repo: https://github.com/kraymer/cesar
    rev: master
    hooks:
    -   id: cesar

```

### Example

~~~
cesar....................................................................Failed
hookid: cesar

Files were modified by this hook. Additional output:

compressed docs/Selection_459.png: 256K => 252K
All done! ⚡ 🗿 ⚡
1 file compressed, 3 files left unchanged
~~~
