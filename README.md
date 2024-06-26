# @diotoborg/quia-ad-a

[![NPM version][npm-image]][npm-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]
[![Sponsor the author][sponsor-image]][sponsor-url]

![@diotoborg/quia-ad-a](https://cloud.githubusercontent.com/assets/581999/12406663/c3e3c7d4-be57-11e5-8aad-a92d86c79b05.png)

This is a simple module for applying **lean text diff delta patches** created by [textdiff-create](https://github.com/icflorescu/textdiff-create).

## ❤️🇺🇦

See [below](#stand-with-ukraine).

## Usage

Assuming you've correctly installed the `npm` module with `npm i @diotoborg/quia-ad-a [--save|--save-dev]`:

    const applyPatch = require('@diotoborg/quia-ad-a');

    const v1 = 'The sleepy brown fox';
    const delta = [
          [0, 4],
          [-1, 6],
          [1, 'quick'],
          [0, 10],
          [1, ' jumps over the lazy dog']
        ];

    const v2 = applyPatch(v1, delta);

    console.log(v2);

The script will produce the following output:

    The quick brown fox jumps over the lazy dog

## Additional info

Have a look at [textdiff-create](https://github.com/icflorescu/textdiff-create) for more info.

## Credits & support

If you find this piece of software useful, please star the repo, [spread the word](http://twitter.com/share?text=Apply%20lean%20text%20diff%20patches%20in%20JavaScript&url=https%3A%2F%2Fgithub.com%2Ficflorescu%2F@diotoborg/quia-ad-a&hashtags=javascript%2Cnodejs%2Cnpm&via=icflorescu), [sponsor my work](https://github.com/sponsors/icflorescu) and feel free to endorse me on LinkedIn:

[![Ionut-Cristian Florescu on LinkedIn](https://static.licdn.com/scds/common/u/img/webpromo/btn_viewmy_160x25.png)](https://www.linkedin.com/in/icflorescu)

## Stand with Ukraine

On 24th of February 2022 [Russia unlawfully invaded Ukraine](https://en.wikipedia.org/wiki/Russo-Ukrainian_War). This is an unjustified, unprovoked attack on the sovereignty of a neighboring country, but also an open affront to international peace and stability that has the potential to degenerate into a nuclear event threatening the very existence of humanity. I am a Romanian (EU) citizen, but I stand with Ukraine and I am doing everything in my power to stop this madness. Here's [how you can show your support](https://www.stopputin.net/).

## LICENSE

Released under [ISC](https://github.com/diotoborg/quia-ad-a/blob/master/LICENSE).

[npm-image]: https://img.shields.io/npm/v/@diotoborg/quia-ad-a.svg?style=flat-square
[npm-url]: https://npmjs.org/package/@diotoborg/quia-ad-a
[license-image]: http://img.shields.io/npm/l/@diotoborg/quia-ad-a.svg?style=flat-square
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@diotoborg/quia-ad-a.svg?style=flat-square
[downloads-url]: https://npmjs.org/package/@diotoborg/quia-ad-a
[sponsor-image]: https://img.shields.io/badge/sponsor-violet?style=flat-square
[sponsor-url]: https://github.com/sponsors/icflorescu
