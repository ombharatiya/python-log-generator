# Simple Log Generator

Simple python script to produce random time series data in a log file (GMT time) that can be used to produce sample time series based information to supply other downstream devices.

### Usage

```
log_generator_script.py --logFile <targetFile>
    [--minSleepMs <int>] [--maxSleepMs <int>]
    [--sourceDataFile <fileWithTextData>] [--iterations <long>]
    [--minLines <int>] [--maxLines <int>]
    [--logPattern <pattern>] [--datePattern <pattern>]
```

### Defaults

```
iterations = -1 # infinite
minSleep = 0.1
maxSleep = 1
minLines = 1
maxLines = 1
logFile = 'logGenerator.log'
sourceDataFile = 'dataFileDefault.txt'
logPattern = '%(asctime)s,%(msecs)d %(process)d %(filename)s %(lineno)d %(name)s %(levelname)s %(message)s'
datePattern = "%Y-%m-%d %H:%M:%S"
```
