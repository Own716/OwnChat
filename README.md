# 💬 OwnChat

OwnChat is a customized third-party Telegram client for Android, based on Cherrygram and the official Telegram App for Android.

- **GitHub Repository**: [https://github.com/Own716/OwnChat](https://github.com/Own716/OwnChat)
- **Base Project**: [Cherrygram](https://github.com/arsLan4k1390/Cherrygram) & [Telegram App for Android](https://github.com/DrKLO/Telegram)

## Maintainers

- [Own716](https://github.com/Own716)

## API & Protocol Documentation

Telegram API manuals: https://core.telegram.org/api

MTproto protocol manuals: https://core.telegram.org/mtproto

## Compilation Guide

You will require Android Studio 2025.1.4+, Android NDK 27.2.12479018, and Android SDK 36.

1. Clone the OwnChat source code with its submodules:
   ```bash
   git clone --recursive --shallow-submodules https://github.com/Own716/OwnChat.git OwnChat
   ```
   In case submodules were not initialized, run:
   ```bash
   git submodule init && git submodule update --init --recursive --depth=1
   ```
2. Configure your signing keystore (`storeFile`, `storePassword`, `keyAlias`, `keyPassword`) in module build.gradle files (`TMessagesProj_App`, `TMessagesProj_AppHuawei`, `TMessagesProj_AppStandalone`).
3. (Optional) In Firebase Console, create an Android app with application ID `org.ownchat.messenger`, enable Firebase Cloud Messaging, and place `google-services.json` in the `TMessagesProj` directory.
4. Open the project in Android Studio (use **Open**, not **Import**).
5. Customize `TMessagesProj/src/main/java/uz/unnarsx/cherrygram/Extra.kt` with your Telegram API ID and Hash.
6. Build and enjoy OwnChat!


## Thanks to:
- [Catogram](https://github.com/Catogram/Catogram) and [Nekogram](https://gitlab.com/Nekogram/Nekogram)
- [exteraGram](https://github.com/exteraSquad/exteraGram) and [OwlGram](https://github.com/OwlGramDev/OwlGram)
- [Telegraher](https://github.com/nikitasius/Telegraher) and [Telegram Monet](https://github.com/c3r5b8/Telegram-Monet)
