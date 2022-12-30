#FlutterSayfalarArasıGeçiş

class HomePage extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Ana Sayfa'),
      ),
      body: ListView(
        children: <Widget>[
          ListTile(
            title: Text('İkinci Sayfaya Git'),
            onTap: () {
              Navigator.push(
                context,
                MaterialPageRoute(builder: (context) => SecondPage()),
              );
            },
          ),
          ListTile(
            title: Text('Üçüncü Sayfaya Git'),
            onTap: () {
              Navigator.push(
                context,
                MaterialPageRoute(builder: (context) => ThirdPage()),
              );
            },
          ),
        ],
      ),
    );
  }
}
