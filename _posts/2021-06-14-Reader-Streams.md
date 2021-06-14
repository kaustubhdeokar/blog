---
title: "Reader-Streams"
date: 2021-06-14
---
Streams 

Reader Streams

* Byte Reader Streams - InputStream

> To read a single byte. 
```java

   private static void readSingleByte(InputStream input) throws IOException {
        int intVal;

        while((intVal= input.read())>=0){
            byte byteVal = (byte) intVal;
            //using byteVal.
        }

```

> To read an array of  bytes.

```java 
   private static void readSingleByte(InputStream input) throws IOException {
        int bytesRead;
        byte[] byteArr = new byte[10];//could be any number, refers to the number of bytes you wish to read.
        while((bytesRead= input.read(byteArr))>=0){
            for(int i=0;i<bytesRead;i++){
                byteArr[i]//has the value read.                 

            }
        }
    

```
* Text Reader Streams - Reader 

> Just replacing the byte with text.  