# ENSTA_ROB305

**Zheyi SHEN & Mengyu PAN**

**Pour simplifier, pour le Raspberry, les processus de scp et ssh sont omis**

## TD1

### a)
For PC
```
cd TD1
g++ -Wall -Wextra TimeSpec.cpp main_td1a.cpp -o main_td1a -lrt
./main_td1a
```

For Raspberry
```
cd TD1
arm-linux-g++ -Wall -Wextra TimeSpec.cpp main_td1a.cpp -o td1a.rpi2 -lrt

./td1a.rpi2
```

### b)
For PC
```
cd TD1
g++ -Wall -Wextra TimeSpec.cpp main_td1b.cpp -o main_td1b -lrt
./main_td1b
```

For Raspberry
```
cd TD1
arm-linux-g++ -Wall -Wextra TimeSpec.cpp main_td1b.cpp -o td1b.rpi2 -lrt

./td1b.rpi2
```

### c)
For PC
```
cd TD1
g++ -Wall -Wextra TimeSpec.cpp main_td1c.cpp -o main_td1c -lrt
./main_td1c <nLoops>
```

For Raspberry
```
cd TD1
arm-linux-g++ -Wall -Wextra TimeSpec.cpp main_td1c.cpp -o td1c.rpi2 -lrt

./td1c.rpi2 <nLoops>
```

### d)
For PC
```
cd TD1
g++ -Wall -Wextra TimeSpec.cpp main_td1d.cpp -o main_td1d -lrt
./main_td1d
```

For Raspberry
```
cd TD1
arm-linux-g++ -Wall -Wextra TimeSpec.cpp main_td1d.cpp -o td1d.rpi2 -lrt
./td1d.rpi2
```


## TD2

### a)
For PC
```
cd TD2
g++ -Wall -Wextra TimeSpec.cpp main_td2a.cpp -o main_td2a -lrt -pthread
./main_td2a <nLoops> <nTasks>
```

For Raspberry
```
cd TD2
arm-linux-g++ -Wall -Wextra TimeSpec.cpp main_td2a.cpp -o td2a.rpi2 -lrt -pthread
./td2a.rpi2 <nLoops> <nTasks>
```

### b)
For PC
```
cd TD2
g++ -Wall -Wextra TimeSpec.cpp main_td2b.cpp -o main_td2b -lrt -pthread
./main_td2b <nLoops> <nTasks> <schedPolicy>
```

For Raspberry
```
cd TD2
arm-linux-g++ -Wall -Wextra TimeSpec.cpp main_td2b.cpp -o td2b.rpi2 -lrt -pthread
./td2b.rpi2 <nLoops> <nTasks> <schedPolicy>
```

### c)
For PC
```
cd TD2
g++ -Wall -Wextra TimeSpec.cpp main_td2c.cpp -o main_td2c -lrt -pthread
./main_td2c <nLoops> <nTasks> <schedPolicy> <protected>
```

For Raspberry
```
cd TD2
arm-linux-g++ -Wall -Wextra TimeSpec.cpp main_td2c.cpp -o td2c.rpi2 -lrt -pthread
./td2c.rpi2 <nLoops> <nTasks> <schedPolicy> <protected>
```


## TD3

### a)
For PC
```
cd TD3
g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp main_td3a.cpp -o main_td3a -lrt
./main_td3a 
./main_td3a <waitTime_s>
```

For Raspberry
```
cd TD3
arm-linux-g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp main_td3a.cpp -o td3a.rpi2 -lrt
./td3a.rpi2
./td3a.rpi2 <waitTime_s>
```

### b)
For PC
```
cd TD3
g++ -Wall -Wextra TimeSpec.cpp Timer.cpp main_td3b.cpp -o main_td3b -lrt
./main_td3b
./main_td3d <n>
```

For Raspberry
```
cd TD3
arm-linux-g++ -Wall -Wextra TimeSpec.cpp Timer.cpp main_td3b.cpp -o td3b.rpi2 -lrt
./td3b.rpi2
./td3b.rpi2 <n>
```

### c)
For PC
```
cd TD3
g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp Timer.cpp Looper.cpp Calibrator.cpp CpuLoop.cpp main_td3c.cpp -o main_td3c -lrt
./main_td3c
```

Raspberry
```
cd TD3
arm-linux-g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp Timer.cpp Looper.cpp Calibrator.cpp CpuLoop.cpp main_td3c.cpp -o td3c.rpi2 -lrt -Wno-psabi
./td3c.rpi2
```

## TD4

### a)
For PC
```
cd TD4
g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp PosixThread.cpp Thread.cpp Increment.cpp main_td4a.cpp -o main_td4a -lrt -lpthread
./main_td4a <nLoops> <nTasks>
```

For Raspberry
```
cd TD4
arm-linux-g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp PosixThread.cpp Thread.cpp Increment.cpp main_td4a.cpp -o td4a.rpi2 -lrt -lpthread -Wno-psabi
./td4a.rpi2 <nLoops> <nTasks>
```

### b)
For PC
```
cd TD4
g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp PosixThread.cpp Thread.cpp Increment.cpp Mutex.cpp IncrementMutex.cpp main_td4b.cpp -o main_td4b -lrt -lpthread
./main_td4b <nLoops> <nTasks>
```

For Raspberry
```
cd TD4
arm-linux-g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp PosixThread.cpp Thread.cpp Increment.cpp Mutex.cpp IncrementMutex.cpp main_td4b.cpp -o td4b.rpi2 -lrt -lpthread -Wno-psabi
./td4b.rpi2 <nLoops> <nTasks>
```

### c)
For PC
```
cd TD4
g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp PosixThread.cpp Thread.cpp Mutex.cpp Semaphore.cpp SemProducer.cpp SemConsumer.cpp main_td4c.cpp -o main_td4c -lrt -lpthread
./main_td4c <nProd> <nCons> <MaxCount>
```

For Raspberry
```
cd TD4
arm-linux-g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp PosixThread.cpp Thread.cpp Mutex.cpp Semaphore.cpp SemProducer.cpp SemConsumer.cpp main_td4c.cpp -o td4c.rpi2 -lrt -lpthread -Wno-psabi
./td4c.rpi2 <nProd> <nCons> <MaxCount>
```

### d)
For PC
```
cd TD4
g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp PosixThread.cpp Thread.cpp Mutex.cpp FifoProducer.cpp FifoConsumer.cpp main_td4d.cpp -o main_td4d -lrt -lpthread
./main_td4d <nProd> <nCons> <n>
```

For Raspberry
```
cd TD4
arm-linux-g++ -Wall -Wextra TimeSpec.cpp Chrono.cpp PosixThread.cpp Thread.cpp Mutex.cpp FifoProducer.cpp FifoConsumer.cpp main_td4d.cpp -o td4d.rpi2 -lrt -lpthread -Wno-psabi
./td4d.rpi2 <nProd> <nCons> <n>
```

## TD5
For PC
```
cd TD5
g++ -Wall -Wextra *.cpp -o main_td5 -lrt -lpthread
./main_td5
```

For Raspberry
```
cd TD5
arm-linux-g++ -Wall -Wextra *.cpp -o td5.rpi2 -lrt -lpthread -Wno-psabi
