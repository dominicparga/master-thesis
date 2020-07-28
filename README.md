# Learning metrics for balancing load in street-networks

[![Tag][github/tags/badge]][github/tags]
[![License][github/license/badge]][github/license]
[![Last commit][github/last-commit/badge]][github/last-commit]

This master-thesis belongs to the [osmgraphing-repo][github/dominicparga/osmgraphing].


## Usage <a name="usage"></a>

You can build by simply executing `latexmk`.
The file `.latexmkrc` sets it up using `lualatex`.
The generated pdf-files (and other files) can be found in `core/build`.
For a fresh and clean build, simply remove this directory.

This setup is tested and used with `visual-studio-code` on `archlinux`.


## Feedback <a name="feedback"></a>

Compare [here][github/self/cmp/feedback] the branch `nightly` with the state from last feedback.

Besides that, every push starts a GitHub-workflow-run, that creates the respective pdf.
This pdf can be downloaded as artifact of the respective workflow in the register `Actions` of this repo.


[github/dominicparga/osmgraphing]: https://github.com/dominicparga/osmgraphing
[github/last-commit]: https://github.com/dominicparga/master-thesis/commits
[github/last-commit/badge]: https://img.shields.io/github/last-commit/dominicparga/master-thesis?style=for-the-badge
[github/license]: https://github.com/dominicparga/master-thesis/blob/master/LICENSE
[github/license/badge]: https://img.shields.io/badge/license-Apache--2.0-green?style=for-the-badge
[github/tags]: https://github.com/dominicparga/master-thesis/tags
[github/tags/badge]: https://img.shields.io/github/v/tag/dominicparga/master-thesis?sort=semver&style=for-the-badge
[github/self/cmp/feedback]: https://github.com/dominicparga/master-thesis/compare/tmp/feedback...nightly
