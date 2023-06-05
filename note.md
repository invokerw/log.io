
### init
cd server/

执行
```
npm install --save-dev @types/node
```

如果有报错
```
AttributeError: module 'collections' has no attribute 'MutableSet'

改文件 collections 变成 collections.abc
```
然后执行
```
npm run build
```


build ui
```
./bin/build-ui.sh
```

cd ./input/file
然后执行
```
npm run build
```
### dev
```
// regist
echo -ne '+input|stream|source1|hello\x00' | nc localhost 6689

// send msg
echo -ne '+msg|stream|source1|hello\x00' | nc localhost 6689
```

