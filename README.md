## Description

Storage for the `packages.json` file which references all ITTI Composer packages.

## Usage

Put this in your `composer.json`:

```json
{
    "repositories": [
        {
            "type": "composer",
            "url": "https://raw.githubusercontent.com/StudioITTI/packagist/refs/heads/main/packages.json"
        }
    ]
}
```
