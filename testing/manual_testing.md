# Manual Testing

## Setup

1. Download recent build from the PR in appveyor
1. Ensure any existing Puppet Extension installs are [gone/deleted](#ensuring-a-clean-slate)
1. Disable Extension [auto-update](#disabling-autoupdate)
1. Install from [VSIX](https://code.visualstudio.com/docs/editor/extension-gallery#_install-from-a-vsix)
1. Follow the [checklist](/checklist.md)

## General Comments

## Ensuring a Clean Slate

VSCode tries to make installing extensions as easy as possible for the user. One of the things it does makes testing extensions slightly more difficult, as it leaves the install folder on the system after uninstalling the extension. When installing different versions many times, this can give you an impression that the new version is installed when it was not because VSCode used the cached folder. To work around this, always clean the install directory as well as uninstalling the extension.

1. Open VSCode and uninstall any existing Puppet VSCode extensions

```
> code --list-extensions
jpogran.puppet-vscode
> code --uninstall-extenion jpogran.puppet-vscode
```

1. Delete any remaining Puppet Extension folders inside $home/.vscode

```
> ls $home/.vscode/extensions

    Directory: C:\Users\james\.vscode\extensions

Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----       11/28/2018  10:17 AM                jpogran.puppet-vscode-0.14.0
```

1.
