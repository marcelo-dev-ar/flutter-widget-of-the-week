# week_82_AboutDialog

A new Flutter project.

## Getting Started

- Sometimes, an app needs a place to put the legalese, the version number, the licenses, and all the other small print. In fact, some stores won't even let you publish your app unless it has all these formalities. You should not leave the creation of such an important part of your app until the last minute, of course. We know you would never do that, but if this happens to you, there's a widget for that!  
- Official Youtube Tutorial: https://youtu.be/YFCSODyFxbE
- Official Doc: https://api.flutter.dev/flutter/material/AboutDialog-class.html

```dart
class _MyHomePageState extends State<MyHomePage> {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(widget.title),
      ),
      body: Center(
        child: RaisedButton(
          child: Text('About'),
          onPressed: () => showAboutDialog(
            context: context,
            applicationIcon: Icon(Icons.accessibility),
            applicationLegalese: 'Legalese',
            applicationName: 'About App',
            applicationVersion: '1.0.0',
            children: [
              Text('A Text Widget'),
            ],
          ),
        ),
      ),
    );
  }
}
```

