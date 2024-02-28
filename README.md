<div align="center">

![](https://www.gstatic.com/devrel-devsite/prod/v937c5f592532c0ad2ebbf299686fcceed4f5934a648172aa45e00618ae0982d7/android/images/dynamic-content-card-default.png)

</div>

#### Desinstalar apk

```sh
adb uninstall br.com.nome.dopackage
```

#### Filtrar (Grep) React-Native no macOS

```sh
adb shell logcat | grep "ReactNativeJS"
```

#### Ativar porta do Reactotron

```bash
adb reverse tcp:9090 tcp:9090
```

#### Filtrar (grep) React-Native no Win

```sh
adb shell logcat | Select-String -Pattern "ReactNativeJS"
```

#### Espelhar apps Android
usando a ferramenta screen copy 
([scrcpy](https://github.com/Genymobile/scrcpy)), digite o comando

```sh
scrcpy
```

#### Listar packages

```bash
adb shell pm list packages
```

#### Instalar multiplos packages

```bash
Get-ChildItem *.apk | ForEach-Object { adb install -r $_.FullName }
```

#### Instalar multiplas apk 

```sh
for file in *.apk; do
    adb install -r -d "$file"
done
```
