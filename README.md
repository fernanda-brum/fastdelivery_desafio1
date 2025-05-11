Aplicativo FastDelivery para consulta de CEP com acesso ao histórico de consultas e também possibilita traçar rotas.

Pré-requisitos: 
- Flutter SDK (≥ 3.0)
- Android SDK (via Android Studio) ou Xcode (para iOS)
- Dispositivo Android/iOS conectado ou emulador/simulador rodando

Tecnologias Utilizadas: Flutter, Dart, MobX, Hive, Dio, Geocoding, url\_launcher

(clonar o repositório)
```bash
git clone https://github.com/<seu-usuario>/fastdelivery_desafio1.git
cd fastdelivery_desafio1
```

(instalar as dependências)
```bash
flutter pub get
```

(gerar código MobX e Hive)
```bash
flutter pub run build_runner build --delete-conflicting-outputs
```

(para executar no Android ou iOS abra um emulador ou conecte seu dispositivo via USB, e ao fim verifique o ID do dispositivo)
```bash
flutter devices
```
(inicie o aplicativo)

```bash
flutter run -d <deviceId>
```
Ou rode:
```bash
flutter run
```

(gerar APK de Release - Android)
```bash
flutter build apk --release
```

Para instalar no dispositivo:

```bash
adb install -r build/app/outputs/flutter-apk/app-release.apk
```

(executar testes automatizados):

```bash
flutter test
```

* Para validar a API ViaCEP:

```bash
dart run tools/test_viacep.dart
```




