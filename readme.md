# For standard users and non-intel power users

1. Install docker

2. Clone:

```
git clone https://github.com/guglielmopadula/dockerfiles.git

```
3. Enter the directory

```
cd dockerfiles/units2122-2nd
```

2. build:
```
docker build --tag uni .    
```

3. enter your working directory (tipically home):
```
cd
```

4. run:
```
docker run -v$PWD:/data -t -i  -p 8888:8888 uni
```
A Jupyter notebook will start with all the dependencies installed.

# For intel power users

1. Install docker

2. Clone:

```
git clone https://github.com/guglielmopadula/dockerfiles.git

```
3. Enter the directory

```
cd dockerfiles/units2122-2nd-intel
```

2. build:
```
docker build --tag uni .    
```

3. enter your working directory (tipically home):
```
cd
```

4. run:
```
docker run -v$PWD:/data -t -i  -p 8888:8888 uni
```
A Jupyter notebook will start with all the dependencies installed.
