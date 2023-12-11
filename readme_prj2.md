```
git clone https://github.com/hdzungx/pintos-hdh pintos
```
```
cd pintos
```
For PRJ2:
```
cd src/userprog
```
```
make
```
```
cd build
```
```
pintos --filesys-size=2 -p ../../examples/echo -a echo -- -f -q run 'echo x'
```
```
make check
```