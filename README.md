  [<img  src="https://i.postimg.cc/qMnWscmy/New-Project-4.jpg"  alt="">](https://www.buymeacoffee.com/flutterzilla)

<hr>
Default Flutter gridview changes the ratio of it's container based on the screen sizes. So, in small screen your gridview may look fine but in bigger screen it may look bad or vice versa. This package lets you use a fixed height for your gridview.
 

## Installation

  

1. Add the latest version of package to your pubspec.yaml (and run`flutter pub get`):

```yaml

dependencies:

flutterzilla_fixed_grid: ^0.0.4

```

2. Import the package and use it in your Flutter App.

```dart

import  'package:flutterzilla_fixed_grid/flutterzilla_fixed_grid.dart';

```

  

## Example

There are a number of properties that you can modify:

  

- height

- crossAxisCount

- mainAxisSpacing

- crossAxisSpacing

  

<hr>

  

```dart

    GridView.builder(
      gridDelegate: const FlutterzillaFixedGridView(
          crossAxisCount: 2,
          mainAxisSpacing: 20,
          crossAxisSpacing: 20,
          height: 143),
      padding: const EdgeInsets.only(top: 30),
      itemCount: 6,
      shrinkWrap: true,
      clipBehavior: Clip.none,
      physics: const NeverScrollableScrollPhysics(),
      itemBuilder: (context, index) {
        return Container(
          padding: const EdgeInsets.symmetric(horizontal: 25, vertical: 25),
          color: Colors.purple,
          child: const Text(
            "Your contents here",
            style: TextStyle(color: Colors.white),
          ),
        );
      },
    ),

```


[<img  src="https://i.postimg.cc/h4QffcQv/1645091374288-1.jpg"  alt="">](https://www.buymeacoffee.com/flutterzilla)