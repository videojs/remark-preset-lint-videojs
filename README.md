<!--This file is generated, see build-presets in the remark-link package -->

# remark-preset-lint-videojs

A remark preset to configure remark-lint with standard rules for video.js project documentation..

## Install

npm:

```sh
npm install remark-preset-lint-videojs
```

You probably want to use it on the CLI through a config file:

```diff
 ...
 "remarkConfig": {
+  "plugins": ["remark-preset-lint-videojs"]
 }
 ...
```

Or use it on the CLI directly

```sh
remark -u remark-preset-lint-videojs readme.md
```

Or use this on the API:

```diff
 var remark = require('remark');
 var report = require('vfile-reporter');

 var file = remark()
+  .use(require('remark-preset-lint-videojs'))
   .processSync('_Emphasis_ and **importance**')

 console.error(report(file));
```

## Rules

This preset configures [remark-lint](https://github.com/wooorm/remark-lint) with the following rules:

| Rule                                                                                                                                            | Setting                      |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------- |
| [`blockquote-indentation`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-blockquote-indentation)                       | `['error', 2]`               |
| [`checkbox-character-style`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-checkbox-character-style)                   | `['warn']`                   |
| [`checkbox-content-indent`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-checkbox-content-indent)                     | `['error']`                  |
| [`code-block-style`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-code-block-style)                                   | `['error', 'fenced']`        |
| [`definition-case`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-definition-case)                                     | `['off']`                    |
| [`definition-spacing`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-definition-spacing)                               | `['error']`                  |
| [`emphasis-marker`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-emphasis-marker)                                     | `['error', '_']`             |
| [`fenced-code-flag`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-fenced-code-flag)                                   | `['error']`                  |
| [`fenced-code-marker`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-fenced-code-marker)                               | ``['error', '`']``           |
| [`file-extension`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-file-extension)                                       | `['error']`                  |
| [`final-definition`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-final-definition)                                   | `['error']`                  |
| [`final-newline`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-final-newline)                                         | `['off']`                    |
| [`first-heading-level`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-first-heading-level)                             | `['warn', 1]`                |
| [`hard-break-spaces`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-hard-break-spaces)                                 | `['off']`                    |
| [`heading-increment`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-heading-increment)                                 | `['error']`                  |
| [`heading-style`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-heading-style)                                         | `['error', 'atx']`           |
| [`link-title-style`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-link-title-style)                                   | `['warn', '"']`              |
| [`list-item-bullet-indent`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-list-item-bullet-indent)                     | `['error']`                  |
| [`list-item-content-indent`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-list-item-content-indent)                   | `['warn']`                   |
| [`list-item-indent`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-list-item-indent)                                   | `['error', 'space']`         |
| [`list-item-spacing`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-list-item-spacing)                                 | `['off']`                    |
| [`maximum-heading-length`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-maximum-heading-length)                       | `['off']`                    |
| [`maximum-line-length`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-maximum-line-length)                             | `['off']`                    |
| [`no-auto-link-without-protocol`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-auto-link-without-protocol)         | `['error']`                  |
| [`no-blockquote-without-marker`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-blockquote-without-marker)             | `['error']`                  |
| [`no-consecutive-blank-lines`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-consecutive-blank-lines)               | `['error']`                  |
| [`no-duplicate-definitions`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-duplicate-definitions)                   | `['error']`                  |
| [`no-duplicate-headings`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-duplicate-headings)                         | `['off']`                    |
| [`no-duplicate-headings-in-section`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-duplicate-headings-in-section)   | `['error']`                  |
| [`no-emphasis-as-heading`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-emphasis-as-heading)                       | `['error']`                  |
| [`no-empty-url`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-empty-url)                                           | `['error']`                  |
| [`no-file-name-articles`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-file-name-articles)                         | `['off']`                    |
| [`no-file-name-consecutive-dashes`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-file-name-consecutive-dashes)     | `['off']`                    |
| [`no-file-name-irregular-characters`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-file-name-irregular-characters) | `['warn', '\\.a-zA-Z0-9-_']` |
| [`no-file-name-mixed-case`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-file-name-mixed-case)                     | `['error']`                  |
| [`no-file-name-outer-dashes`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-file-name-outer-dashes)                 | `['error']`                  |
| [`no-heading-content-indent`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-heading-content-indent)                 | `['error']`                  |
| [`no-heading-indent`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-heading-indent)                                 | `['error']`                  |
| [`no-heading-like-paragraph`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-heading-like-paragraph)                 | `['error']`                  |
| [`no-heading-punctuation`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-heading-punctuation)                       | `['off']`                    |
| [`no-html`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-html)                                                     | `['off']`                    |
| [`no-inline-padding`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-inline-padding)                                 | `['error']`                  |
| [`no-literal-urls`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-literal-urls)                                     | `['off']`                    |
| [`no-missing-blank-lines`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-missing-blank-lines)                       | `['off']`                    |
| [`no-multiple-toplevel-headings`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-multiple-toplevel-headings)         | `['error']`                  |
| [`no-reference-like-url`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-reference-like-url)                         | `['error']`                  |
| [`no-shell-dollars`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-shell-dollars)                                   | `['error']`                  |
| [`no-shortcut-reference-image`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-shortcut-reference-image)             | `['off']`                    |
| [`no-shortcut-reference-link`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-shortcut-reference-link)               | `['off']`                    |
| [`no-table-indentation`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-table-indentation)                           | `['error']`                  |
| [`no-tabs`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-tabs)                                                     | `['error']`                  |
| [`no-undefined-references`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-undefined-references)                     | `['error']`                  |
| [`no-unused-definitions`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-no-unused-definitions)                         | `['error']`                  |
| [`ordered-list-marker-style`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-ordered-list-marker-style)                 | `['error', '.']`             |
| [`ordered-list-marker-value`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-ordered-list-marker-value)                 | `['error', 'one']`           |
| [`rule-style`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-rule-style)                                               | `['error', '***']`           |
| [`strong-marker`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-strong-marker)                                         | `['error', '*']`             |
| [`table-cell-padding`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-table-cell-padding)                               | `['warn', 'padded']`         |
| [`table-pipe-alignment`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-table-pipe-alignment)                           | `['warn']`                   |
| [`table-pipes`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-table-pipes)                                             | `['warn']`                   |
| [`unordered-list-marker-style`](https://github.com/wooorm/remark-lint/tree/master/packages/remark-lint-unordered-list-marker-style)             | `['warn', '*']`              |

