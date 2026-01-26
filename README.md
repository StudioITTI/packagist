## Description

Storage for the `packages.json` file which references all ITTI Composer projects.

## Usage

Put this in your `composer.json`:

```json
{
    "repositories": [
        {
            "type": "composer",
            "url": "https://github.com/StudioITTI/packagist/raw/refs/heads/main/packages.json"
        }
    ]
}
```