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

## Share

<a href="https://p32929.github.io/share/?repo=Shortcut-Virus-Remover"><img src="https://p32929.github.io/readme/share.svg" alt="Share this with your friends in just a click" width="420"></a>

## Support

<a href="https://p32929.github.io/support/"><img src="https://p32929.github.io/readme/support.svg" alt="If you like my works and want to support me, feel free to support" width="420"></a>
