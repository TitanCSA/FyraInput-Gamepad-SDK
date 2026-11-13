# FyraInput-Gamepad SDK packages

Public Windows x64 user-mode SDK source packages. These folders contain the existing SDK and its licenses; no kernel driver, activation secret or installer is included.

- [Native SDK source and recipes](https://github.com/TitanCSA/sdk-packages/blob/main/projects/FyraInput-Gamepad/packaging/native/README.txt)
- [Registry status](SDK-PUBLICATION.md)

Downloadable release artifacts do not imply publication on a central package registry.

<!-- central-sdk-packages:start -->
## Paquets et installation

Les sources, licences, guides API et exemples sont regroupes dans [le depot SDK dedie](https://github.com/TitanCSA/sdk-packages/tree/main/projects/FyraInput-Gamepad). Choisis le paquet a installer puis execute sa commande dans son dossier.

| Paquet | Registre | Disponibilite | Installation / utilisation |
| --- | --- | --- | --- |
| `fyrainput-gamepad` | vcpkg | Registre TitanCSA disponible (configuration ci-dessous) | `vcpkg install fyrainput-gamepad:x64-windows` |
| `fyrainput-gamepad` | Conan | Registre TitanCSA disponible (configuration ci-dessous) | `conan install --requires=fyrainput-gamepad/0.1.0 -r titancsa --build=missing -s compiler.cppstd=17` |
| `FyraInput-Gamepad.Native` | NuGet | Publie et verifie | `Install-Package FyraInput-Gamepad.Native -Version 0.1.0` |
| `FyraInputGamepad.SDK` | NuGet | Publie et verifie | `dotnet add package FyraInputGamepad.SDK --version 1.0.0` |
| `fyrainput_gamepad` | PyPI | Pas encore disponible / validation en cours | Commande prevue apres publication : `python -m pip install fyrainput-gamepad==1.0.0` |
| `fyrainput-gamepad` | Conda | Canal TitanCSA disponible ; acceptation conda-forge encore en attente | `conda install --override-channels -c https://raw.githubusercontent.com/TitanCSA/sdk-packages/089bc73095aa8eda89bacbe10d0b9e58394b0207/conda-channel -c conda-forge fyrainput-gamepad` |
| `fyrainput_gamepad` | crates.io | Publie et verifie | `cargo add fyrainput-gamepad@1.0.0` |
| `fyrainput_gamepad` | npm | Publie et verifie | `npm install fyrainput-gamepad@1.0.0` |
| `io.github.titancsa:fyrainput-gamepad` | Maven Central | Publie et verifie | `io.github.titancsa:fyrainput-gamepad:1.0.0 (pom.xml / Gradle)` |
| `com.github.TitanCSA:FyraInput-Gamepad-SDK` | JitPack | Publie et verifie | `com.github.TitanCSA:FyraInput-Gamepad-SDK:java-sdk-v1.0.0 (avec le depot JitPack)` |
| `github.com/TitanCSA/FyraInput-Gamepad-SDK/FyraInput-Gamepad-Go-modules` | Go Modules | Publie et verifie | `go get github.com/TitanCSA/FyraInput-Gamepad-SDK/FyraInput-Gamepad-Go-modules@v1.0.0` |
| `github.com/TitanCSA/FyraInput-Gamepad-SDK/FyraInput-Gamepad-Go-modules` | pkg.go.dev | Publie et verifie | `Documentation : https://pkg.go.dev/github.com/TitanCSA/FyraInput-Gamepad-SDK/FyraInput-Gamepad-Go-modules@v1.0.0` |
| `fyrainput_gamepad` | PowerShell Gallery | Publie et verifie | `Install-Module FyraInputGamepad -RequiredVersion 1.0.0 -Scope CurrentUser` |
| `fyrainput_gamepad` | pub.dev | Publie et verifie | `dart pub add fyrainput_gamepad:1.0.0` |
| `fyrainput_gamepad` | RubyGems | Publie et verifie | `gem install fyrainput-gamepad -v 1.0.0` |
| `fyrainput_gamepad` | Packagist | Pas encore disponible / validation en cours | Commande prevue apres publication : `composer require titancsa/fyrainput-gamepad:1.0.0` |

Pour vcpkg et Conan, configure d abord le registre TitanCSA avec [le guide complet](https://github.com/TitanCSA/sdk-packages/tree/main/projects/FyraInput-Gamepad/README.md). Le guide explique aussi Maven/Gradle, les prerequis et le chargement des DLL. Les pilotes/applications du produit sont installes separement. Les commandes marquees prevues ne sont pas encore disponibles.

Les anciens imports Go et versions JitPack gardent leurs tags. Pour les anciennes archives SDK, utilise [les liens de remplacement](https://github.com/TitanCSA/sdk-packages/blob/main/release-assets/URL-MIGRATION.json).
<!-- central-sdk-packages:end -->
