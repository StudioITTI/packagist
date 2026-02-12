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
Tips on specifying version constraints with `composer require`: https://getcomposer.org/doc/articles/versions.md#writing-version-constraints

### Github authentication
To allow composer to download the `dist` variant instead of `source`, you need to create a personal access token
- Go to https://github.com/settings/personal-access-tokens
- Create a token which can access all organisation repositories, with read-only permission for "Contents"
- Copy and save the generated token
- Execute `composer config -g github-oauth.github.com YOUR_GITHUB_TOKEN`
- Now you can do `composer install` and it should

### Windows usage
For using composer in Windows environment with cmd.exe, you need an environment variable `GIT_SSH` pointing to
plink.exe in order for pageant keys to work. Press `Start` and enter 'Environment'.
