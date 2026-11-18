# Shortcut-Virus-Remover

Plugged in your pen drive and your files are gone, with only shortcuts left? This tiny Windows script brings your files back and deletes the fake shortcuts the "shortcut virus" left behind. Your files are usually still there, just hidden.

## What it actually does

Two commands, nothing hidden:

```bat
attrib -s -h -a /s /d D:\*.*   :: clears the system/hidden/archive flags the virus set on your files
del /a /q /s D:\*.lnk          :: deletes every .lnk shortcut on that drive
```

So it **recovers files the virus hid** and **removes the shortcut files**. It does not find or remove the virus itself, so scan your computer with an antivirus too. Run it on the infected removable drive, not on your system drive.

## How to use

1. Download `Shortcut Virus Remover 1.0.bat` from this repo.
2. Double-click it.
3. Type the drive letter of the infected drive (for example `D`) and press Enter.
4. Wait. A drive with many files takes a while.

> **Careful:** it deletes *every* `.lnk` shortcut on that drive. If you keep real shortcuts there, move them off first.

## License

MIT License — Copyright (c) 2020 Fayaz Bin Salam.

## Contributing

Contributions are very welcome, thank you! Before you start on a pull request, please open an issue and tell me what you would like to add or change. That way we can agree on it first, and your time is not wasted on something that might not fit. Thanks for helping make Shortcut Virus Remover better.

## You might also like

<p><a href="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/0"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/0-dark.svg"><img src="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/0-light.svg" width="50%" align="top" alt="More apps by p32929 on OpenStore (1)"></picture></a><a href="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/1"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/1-dark.svg"><img src="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/1-light.svg" width="50%" align="top" alt="More apps by p32929 on OpenStore (2)"></picture></a><br><a href="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/2"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/2-dark.svg"><img src="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/2-light.svg" width="50%" align="top" alt="More apps by p32929 on OpenStore (3)"></picture></a><a href="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/3"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/3-dark.svg"><img src="https://openstore.pfay.workers.dev/more/p32929/shortcut-virus-remover/personal/3-light.svg" width="50%" align="top" alt="More apps by p32929 on OpenStore (4)"></picture></a></p>

<p><a href="https://p32929.github.io/share/?repo=Shortcut-Virus-Remover"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-share-dark.svg"><img src="https://p32929.github.io/readme/footer-share-light.svg" width="50%" align="top" alt="Share this project with your friends in one click"></picture></a><a href="https://p32929.github.io/support/"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-support-dark.svg"><img src="https://p32929.github.io/readme/footer-support-light.svg" width="50%" align="top" alt="If you like my work and want to support me, feel free to support"></picture></a><br><a href="https://openstore.pfay.workers.dev/add"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-join-dark.svg"><img src="https://p32929.github.io/readme/footer-join-light.svg" width="100%" align="top" alt="Put your own apps on OpenStore: free, your listing lives in your own repo"></picture></a></p>
