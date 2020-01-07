# testPrj
## Prerequistic
* hostname : Master is hadoop master

* example
```
sudo -i
echo "111.111.111.111 master" >> /etc/hosts
```

### Keyfile
* keyfile name : mykey.pem
```
$ ls
do.sh hive_empdept.sh mykey.pem
```

##install
```
git clone http://github.com/finfra/testPrj.git
cd testPrj
scp ~/mykey.pem ./
. do.sh
```

## Result
```
~
~
Time taken: 11.183 seconds, Fetched: 3 row(s)
Query ID = hadoop_20200107050402_81b002a6-8059-4c60-a430-9b135bfb3829
Total jobs = 1
Launching Job 1 out of 1
Status: Running (Executing on YARN cluster with App id application_1578362785160_0008)

Map 1: 0(+1)/1  Reducer 2: 0/1  Reducer 3: 0/1
Map 1: 1/1      Reducer 2: 0/1  Reducer 3: 0/1
Map 1: 1/1      Reducer 2: 1/1  Reducer 3: 0(+1)/1
Map 1: 1/1      Reducer 2: 1/1  Reducer 3: 1/1
OK
20      2518.75
10      2916.6666666666665
Time taken: 1.174 seconds, Fetched: 2 row(s)
OK
dept
emp
Time taken: 0.021 seconds, Fetched: 2 row(s)

```

## Copy Right
2020.01 : ID N mail
