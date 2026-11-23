# mytop-project/.github

What every repository of the Droidtop organisation shares by default.

- **Issue forms** (`.github/ISSUE_TEMPLATE/`): a repository with no forms of its own uses these. Problems with
  droidtop or Enginehost themselves go to [mytop-project/tracker](https://github.com/mytop-project/tracker), where every finding
  is kept in one place.
- **Starter workflows** (`workflow-templates/`): GitHub offers them under Actions > New workflow in any repository of
  the organisation. They are thin callers of the reusable workflows in
  [mytop-project/droidtop-platforms](https://github.com/mytop-project/droidtop-platforms), pinned by commit, so a plugin
  repository builds, signs, checks its commits and checks its copied tools the same way as every other:
  - `droidtop-plugin-bundle.yml`: build, sign and release a plugin bundle (`droidtop-plugin-bundle.yml`);
  - `commit-hygiene.yml`: the commit rules (`commit-hygiene.yml`);
  - `template-drift.yml`: the plugin's copies of [the plugin template](https://github.com/mytop-project/droidtop-plugin-template)'s
    tools are the template's own at a tag (`plugin-template-drift.yml`).

A new plugin starts from [mytop-project/droidtop-plugin-template](https://github.com/mytop-project/droidtop-plugin-template),
which already carries these. When a reusable workflow changes in droidtop-platforms, the pins here move with it.

Licensed under the GNU General Public License v3.0 (`LICENSE`).
