# CT3(TAB-A04-BR3) / CTX(TAB-A05-BD) / CTZ(TAB-A05-BA1)

### 対応端末

> [!IMPORTANT]
> **BLU** 必須です

- **TAB-A04-BR3 (a04br3)**
- **TAB-A05-BD (a05bd)**
- **TAB-A05-BA1 (a05ba)**

> [!TIP]
> いずれのビルドでも構いません。  
> 強制的に調整します。

## 利用方法

> [!WARNING]
> 予め、各自でオリジナルイメージのバックアップを取ってください。  
> バックアップは任意ですが、何かしらの問題が発生した際に復元できません。

> [!NOTE]
> **Windows** の環境で作業することを前提とします。

1. [**Releases**](https://github.com/s1204IT/CPadGmsSystem/releases/latest) から、ファイルをダウンロードする。  
  ファイル名は、対応端末を参照してご確認ください。
2. ダウンロードした **ZIP** ファイルを展開する。
3. 端末を **bootloader** へ再起動する。
  - `adb reboot bootloader`
4. `INSTALL GMS SYSTEM.bat` をダブルクリックして実行する。
5. **Model** を注視し、端末背面の認証機器名と一致しているか確認する。
6. 続行する場合は、「**Y**」キーを押す。
7. 端末が再起動するまで絶対に端末には触れず、処理が完了するまで待つ。
8. 端末でセットアップウィザードが起動すれば成功です。

## fastboot でチャレンジパッドが検出されない
以下のドライバを適用する事により解決出来る可能性があります｡

> For automatic/direction installation:
> [Click here to download](https://mega.nz/file/YfgSkILT#8ST9kN0hVLaEtviUg1AhrlFnzKzGEAYy63KI6MYDlNE)
> ---
> For manual installation:
> [Click here to download](https://drive.google.com/file/d/1qVmxaQxddvPRjEKHjQVjj3Eo_cawSE9C/view?usp=sharing)

## CT3 で画面ロックを設定したい

下記の APK をダウンロードし、インストールしてください。

<https://github.com/s1204IT/ResetPasswordTester/releases/download/v1.0.0/ResetPasswordTester-nougat-v1.0.0.apk>

インストールが完了すると、ホーム画面に南京錠のアイコンで「パスワードを変更」と言う名前でアプリが配置されます。  
起動すると、初回のみ端末管理アプリの有効化が求められるので有効にし、もう一度アプリを開くとパスワードの設定を行う画面になります。

ADB を介さずに端末のみでインストールするには、初回のみ次のコマンドを実行する必要があります：
```
adb shell settings put secure install_non_market_apps 1
```
