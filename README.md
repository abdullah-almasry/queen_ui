# Queen Ui 👑

**pre built flutter widgets**

## components

- [x] navigation bar

## [**Demo**](https://maxland-a4698.web.app/)

![in small screens](https://github.com/maxzod/queen_ui/blob/master/images/nav_bar_in_small.png?raw=true)
![in large screens](https://github.com/maxzod/queen_ui/blob/master/images/nav_bar_in_large.png?raw=true)

## Example

```dart
 @override
 Widget build(BuildContext context) {
    final size = MediaQuery.of(context).size;
    return QueenNavBar(
      color: Colors.blue,
      logo: Padding(
        padding: const EdgeInsets.all(horizontal: 8),
        child: Text(
          "Queen 👑",
        ),
      ),
      children: [
        OutlineButton(
            title: 'home',
            onPressed: (){},
            ),
        OutlineButton(
            title: 'about',
            onPressed: (){},
            ),
        OutlineButton(
            title: 'contact',
            onPressed: (){},
            ),
      ],
      drawerButtonBuilder: () {
        return Padding(
          padding: EdgeInsets.symmetric(horizontal: size.width * .01),
          child: OutlineButton(
            child: Icon(Icons.menu),
            onPressed: () =>
              print('Long Live The Queen 👑')
            ,
          ),
        );
      },
    );
  }
```
