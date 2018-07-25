# Levigo

### Install
~~~
cd $GOPATH
mkdir deps && deps
git clone -b v1.20 https://github.com/google/leveldb.git
cd leveldb && make
cd $GOPATH 
CGO_CFLAGS="-I$GOPATH/deps/leveldb/include" CGO_LDFLAGS="-L$GOPATH/deps/leveldb/out-shared" go get github.com/ivanabc/levigo
~~~
