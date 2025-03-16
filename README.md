# Lain-Says

Lain-Says is a fun command-line tool inspired by cowsay, but with Lain from Serial Experiments Lain. It displays random sofware, hardware and science curiosities along with an ASCII representation of Lain.

## Installation

### Installing from `.deb`
You can install Lain-Says using the `.deb` package:

```bash
sudo dpkg -i lain-says.deb
```

If you encounter missing dependencies, run:
```bash
sudo apt-get install -f
```

### Uninstalling
If you ever want to remove Lain-Says, run:
```bash
sudo dpkg -r lain-says
```

## Usage
Once installed, you can use it in the terminal:
```bash
lain-says "Hello, world!"
```

If no message is provided, it will display a random curiosity.

## Building from Source
To build your own `.deb` package, clone the repository and use `dpkg-deb`:

```bash
git clone https://github.com/DamperDoor56/lain-says.git
cd lain-says
mkdir -p lain-says-pkg/DEBIAN
mkdir -p lain-says-pkg/usr/local/bin
cp lain-says lain-says-pkg/usr/local/bin/
cp control postinst postrm lain-says-pkg/DEBIAN/
dpkg-deb --build lain-says-pkg
```

This will generate `lain-says-pkg.deb`, which can be installed as shown above.

## Releases
For the latest `.deb` releases, visit the [Releases](https://github.com/DamperDoor56/lain-says/releases) page.

## License
This project is open-source and released under the MIT License.

---

Let's all love Lain 📟



