# UrlLauncherFactory

[![Flutter](https://github.com/daohoangson/flutter_widget_from_html/actions/workflows/flutter.yml/badge.svg)](https://github.com/daohoangson/flutter_widget_from_html/actions/workflows/flutter.yml)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=daohoangson_flutter_widget_from_html&metric=coverage)](https://sonarcloud.io/summary/new_code?id=daohoangson_flutter_widget_from_html)
[![Pub](https://img.shields.io/pub/v/fwfh_url_launcher.svg)](https://pub.dev/packages/fwfh_url_launcher)

WidgetFactory extension to launch A tag via [url_launcher](https://pub.dev/packages/url_launcher) plugin.
This is a companion add-on for [flutter_widget_from_html_core](https://pub.dev/packages/flutter_widget_from_html_core) package.

## Getting Started

Add this to your app's `pubspec.yaml` file:

```yaml
dependencies:
  flutter_widget_from_html_core: any
  fwfh_url_launcher: ^0.16.0
```

## Usage

Then use `HtmlWidget` with a custom factory:

```dart
import 'package:flutter_widget_from_html_core/flutter_widget_from_html_core.dart';
import 'package:fwfh_url_launcher/fwfh_url_launcher.dart';

// ...

HtmlWidget(
  html,
  factoryBuilder: () => MyWidgetFactory(),
)

// ...

class MyWidgetFactory extends WidgetFactory with UrlLauncherFactory {
}
```
