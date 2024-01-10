This package contains a set of lint rules for Gajeroll team
to encourage good coding practices.

This package is built on top of Flutter's `flutter.yaml` from [package:flutter_lints].

## Usage

1. This package is not published to pub.dev yet. So, you can only use it by
   depending on the Git repository directly in your `pubspec.yaml` file.

  ```yaml
  dev_dependencies:
    gajeroll_lints:
      git:
        url: https://github.com/gajeroll/gajeroll_lints.git
  ```

2. Create an `analysis_options.yaml` file at the root of the package (alongside
   the `pubspec.yaml` file) and `include: package:gajeroll_lints/gajeroll.yaml`
   from it.

Example `analysis_options.yaml` file:

```yaml
# This file configures the analyzer, which statically analyzes Dart code to
# check for errors, warnings, and lints.
#
# The issues identified by the analyzer are surfaced in the UI of Dart-enabled
# IDEs (https://dart.dev/tools#ides-and-editors). The analyzer can also be
# invoked from the command line by running `flutter analyze`.

# The following line activates a set of recommended lints for Flutter apps,
# packages, and plugins designed to encourage good coding practices.
include: package:gajeroll_lints/gajeroll.yaml

linter:
  # The lint rules applied to this project can be customized in the
  # section below to disable rules from the `package:flutter_lints/flutter.yaml`
  # included above or to enable additional rules. A list of all available lints
  # and their documentation is published at https://dart.dev/lints.
  #
  # Instead of disabling a lint rule for the entire project in the
  # section below, it can also be suppressed for a single line of code
  # or a specific dart file by using the `// ignore: name_of_lint` and
  # `// ignore_for_file: name_of_lint` syntax on the line or in the file
  # producing the lint.
  rules:
    # avoid_print: false  # Uncomment to disable the `avoid_print` rule
    # prefer_single_quotes: true  # Uncomment to enable the `prefer_single_quotes` rule
# Additional information about this file can be found at
# https://dart.dev/guides/language/analysis-options
```

[package:flutter_lints]: https://pub.dev/packages/flutter_lints
