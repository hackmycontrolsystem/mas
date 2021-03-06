# MAS
MAS stands for Modbus Attack Scripts.

## Prerequisites
```bash
apt-get install python-pip python-dev
pip install pymodbus
```

## read_all_holding_registers.py
```
usage: read_all_holding_registers.py [-h] [-p PORT] [-u UID] [-sa START]
                                      [-ea END]
                                      ip

Read all holding registries from a TCP MODBUS Slave

positional arguments:
  ip                    IP address of the slave

optional arguments:
  -h, --help            show this help message and exit
  -p PORT, --port PORT  Modbus Port. Defaults to 502
  -u UID, --uid UID     Modbus Unit ID. Defaults to 1
  -sa START, --start-address START
                        Starting Address for the scanner. Defaults to 1
  -ea END, --end-address END
                        Ending Address for the scanner. Defaults to 65535
```

## write_all_holding_registers.py
```
usage: write_all_holding_registers.py [-h] [-p PORT] [-u UID] [-sa START]
                                      [-ea END] [-v VALUE]
                                      ip

Write all holding registries on a TCP MODBUS Slave

positional arguments:
  ip                    IP address of the slave

optional arguments:
  -h, --help            show this help message and exit
  -p PORT, --port PORT  Modbus Port. Defaults to 502
  -u UID, --uid UID     Modbus Unit ID. Defaults to 1
  -sa START, --start-address START
                        Starting Address for the writer. Defaults to 1
  -ea END, --end-address END
                        Ending Address for the writer. Defaults to 65535
  -v VALUE, --value VALUE
                        Value that will be written. Defaults to 7777
```
