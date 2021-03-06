# Gunpowder

Gunpowder aims to provide an all-in-one API for your server modding needs.

## Support

If you find a bug or want to suggest a feature, go to the [Issues tab](https://github.com/Gunpowder-MC/Gunpowder/issues)
If the bug is related to one of our modules, go to that specific module [here](https://github.com/Gunpowder-MC)
If you want to ask for help and/or clarify a bug, or even contribute to the project, you can find us on the [AOF discord in #gunpowder](https://discord.gg/6rkdm48)

## Official modules

- [Gunpowder Currency](https://www.curseforge.com/minecraft/mc-mods/gunpowder-currency)
- [Gunpowder Market](https://www.curseforge.com/minecraft/mc-mods/gunpowder-market)
- [Gunpowder Teleport](https://www.curseforge.com/minecraft/mc-mods/gunpowder-teleport)
- [Gunpowder Sleepvote](https://www.curseforge.com/minecraft/mc-mods/gunpowder-sleepvote)
- [Gunpowder Utilities](https://www.curseforge.com/minecraft/mc-mods/gunpowder-utilities)

## License

This mod is available under the [MIT license](LICENSE).

## Contributing

More information will be provided soon. Contributions should follow the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).

## Extending

If you want to use Gunpowder, use our [template project](https://github.com/gunpowder-mc/gunpowdertemplate) or follow the steps below:

Add the following to your build.gradle:

```gradle
dependencies {
    modApi "io.github.gunpowder:gunpowder-api:${gunpowder_version}+${minecraft_version}"
}

repositories {
    maven {
        name = "Gunpowder"
        url = "https://maven.martmists.com/releases"
    }
}
```

Create a class extending GunpowderModule (e.g. com.example.ExampleModule), and then fabric.mod.json, add:

```json
{
  "entrypoints": {
    "gunpowder:modules": [
      "com.example.ExampleModule"
    ]  
  }
}
```

