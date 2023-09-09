<div align="center"><img src="https://raw.githubusercontent.com/blocs/blocs/main/logo.svg" width="400" /></div>

# The PHP Template engine for Laravel
Laravelのためのテンプレートエンジン

[![Latest stable version](https://img.shields.io/packagist/v/blocs/blocs)](https://packagist.org/packages/blocs/blocs)
[![Total downloads](https://img.shields.io/packagist/dt/blocs/blocs)](https://packagist.org/packages/blocs/blocs)
[![GitHub code size](https://img.shields.io/github/languages/code-size/blocs/blocs)](https://github.com/blocs/blocs)
[![GitHub license](https://img.shields.io/github/license/blocs/blocs)](https://github.com/blocs/blocs)
[![Laravel awesome](https://img.shields.io/badge/Awesome-Laravel-green)](https://github.com/blocs/blocs)
[![Laravel version](https://img.shields.io/badge/laravel-%3E%3D7-green)](https://github.com/blocs/blocs)
[![PHP version](https://img.shields.io/badge/php-%3E%3D7.4-blue)](https://github.com/blocs/blocs)

[**Website**](https://blocs.jp/)
| [**Document**](https://blocs.jp/reference/)
| [**English**](https://blocs.jp/en/readme.html)

# 導入方法
composerで導入してください。

```sh
laravel-app % composer require blocs/autoinclude    
Using version ^1.0 for blocs/autoinclude
./composer.json has been created
Running composer update blocs/autoinclude
Loading composer repositories with package information
Info from https://repo.packagist.org: #StandWithUkraine
Updating dependencies
Lock file operations: 2 installs, 0 updates, 0 removals
  - Locking blocs/autoinclude (v1.0.0)
  - Locking blocs/blocs (v1.1.28)
Writing lock file
Installing dependencies from lock file (including require-dev)
Package operations: 2 installs, 0 updates, 0 removals
  - Installing blocs/blocs (v1.1.28): Extracting archive
  - Installing blocs/autoinclude (v1.0.0): Extracting archive
Generating autoload files
```

# Datepicker

```html
<!-- data-include="auto" -->

<input type="text" name="datepicker" class="ai-datepicker" />
```

# Phone

```html
<!-- data-include="auto" -->

<input type="text" name="phone" class="ai-phone" />
```

# Select2

```html
<!-- data-include="auto" -->

<select name="multipleSelect[]" class="ai-select2" multiple="multiple" style="width:100%" />
  <option value="1">Test1</option>
  <option value="2">Test2</option>
</select>
```

# Tooltip

```html
<!-- data-include="auto" -->

<!-- data-attribute="title" data-val="Tooltip<br />テストです" -->
<a data-bs-toggle="tooltip" data-bs-html="true" data-bs-placement="bottom">Tooltip</a>
```

# Modal

```html
<!-- data-include="auto" -->

<!--
  $modalTitle = "タイトル"
  $modalCloseLabel = "閉じる"
  $modalBody = "改行\n\n\n\n改行"
  $modalTarget = "exampleModal"
-->

<!-- data-attribute="data-bs-target" data-val=$modalTarget data-prefix="#" -->
<button type="button" class="btn btn-primary" data-bs-toggle="modal">
    <i class="fa-brands fa-twitter"></i> モーダルを開く
</button>

<!-- data-bloc = "modalButton" -->
<button type="button" class="btn btn-primary">
    <i class="fa-brands fa-twitter"></i> 登録
</button>
<!-- data-endbloc -->

<!-- data-include = "modal" -->
```
