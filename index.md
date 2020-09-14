## Mobile 1 Pertemuan4: Navigator
Navitgator merupakan cara untuk berpindah dari satu page ke page lain, ada bebrapa cara yang bisa digunakan yaitu
>## Cara 1: Dengan Menggunakan Route
Metode navigator ini dengan menentukan route masing-masing page pada bagian materialApp dan kemudian dapat setiap halaman yang akan dituju akan panggil sesuai nama route.
dengan metode ini  jumlah halaman tidak terbatas.
langsung saja dipraktekan dengan membuat 2 buah class yaitu

Class: Halutama
```dart
class Halutama extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: AppBar(
        leading:IconButton(color:Colors.white,icon: Icon(Icons.home),onPressed:null,),
        title: Text('Home'),
      ),
      body: new Center(
        child: new Container(
          child: new IconButton(
            icon: Icon(Icons.headset, size: 40.0),
            onPressed: () {
              Navigator.pushNamed(context, '/Haldua');
            },
          ),
        ),
      ),
    );
  }
}
```
