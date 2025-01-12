<h1 align="center">
	<img src="https://github.com/orisai/.github/blob/main/images/repo_title.png?raw=true" alt="Orisai"/>
	<br/>
	Virtual File System
</h1>

<p align="center">
    Emulate file system with plain PHP
</p>

<p align="center">
	📄 Check out our <a href="docs/README.md">documentation</a>.
</p>

<p align="center">
	💸 If you like Orisai, please <a href="https://orisai.dev/sponsor">make a donation</a>. Thank you!
</p>

<p align="center">
	<a href="https://github.com/orisai/vfs/actions?query=workflow:CI+branch:v1.x"><img src="https://github.com/orisai/vfs/actions/workflows/ci.yaml/badge.svg?branch=v1.x"></a>
	<a href="https://coveralls.io/github/orisai/vfs?branch=v1.x"><img src="https://badgen.net/coveralls/c/github/orisai/vfs/v1.x?cache=300"></a>
	<a href="https://dashboard.stryker-mutator.io/reports/github.com/orisai/vfs/v1.x"><img src="https://img.shields.io/endpoint?style=flat&url=https://badge-api.stryker-mutator.io/github.com/orisai/vfs/v1.x"></a>
	<a href="https://packagist.org/packages/orisai/vfs"><img src="https://badgen.net/packagist/dt/orisai/vfs?cache=3600"></a>
	<a href="https://packagist.org/packages/orisai/vfs"><img src="https://badgen.net/packagist/v/orisai/vfs?cache=3600"></a>
	<a href="https://choosealicense.com/licenses/mpl-2.0/"><img src="https://badgen.net/badge/license/MPL-2.0/blue?cache=3600"></a>
<p>

##

> This package is remake of [php-vfs](https://github.com/michael-donat/php-vfs) from [michael-donat](https://github.com/michael-donat). Thank you, Michael!

```php
use Orisai\VFS\VFS;

// Register VFS protocol
$scheme = VFS::register();

// Write into virtual file
file_put_contents("$scheme://file", 'content');

// Read content of virtual file
$content = file_get_contents("$scheme://file");

// Unregister protocol, delete the virtual filesystem
VFS::unregister($scheme);
```
