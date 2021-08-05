Openfed Composer Repository
===========================

This is [composer](https://getcomposer.org/) repository to speed up packages installation in Openfed.

To use Openfed Libraries, your project `composer.json` should contain:

```json
"repositories": [
	{
		"type": "composer",
		"url": "https://openfed.github.io/openfed-libraries/"
	},
]
```

Head over to https://openfed.github.io/openfed-libraries/ to browse available packages.

__NOTE__: actual composer repository is on [gh-pages](https://github.com/openfed/openfed-libraries/tree/gh-pages) branch


## Update Openfed Libraries

This project makes use of [Satis](https://github.com/composer/satis) and it's using its master branch

To update the available libraries, you'll have to:
- Update satis.json to add more libraries, always keeping the old versions to assure retro-compatibility.
- Run "make" in order for satis to generate the new files.
- Commit the updated files to master branch
- Commit the contents of "dist" folder to gh-pages branch 
