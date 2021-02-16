WM800 node red project - IPC modbus TCP/IP
=====

### About

QR-code are created by Node Jason in the IPC of the machine.
The created QR-code are visualized in a Web frame of the IPC.
The PLC makes production data and machine ID accessible on Modbus TCP/IP.
The IPC is the Client and the PLC the Server.

PLC Modbus TCP/IP Server registers:
PLC -> IPC
%MW0: PLC MACx0
%MW1: PLC MACx1
%MW2: PLC MACx2
%MW3: PLC MACx3
%MW4: PLC MACx4
%MW5: PLC MACx5
%MW6: Machine ID number
%MW7: Cut depth in 0.01mm  (Value 123=1.23mm)
IPC -> PLC
%MW20.bit0: Internet status = TRUE
%MW21: Valid Leasing 1
%MW22: Valid Leasing 2
%MW23: Valid Leasing 3
%MW24: Status sold 1
%MW25: Status sold 2
%MW26: Status sold 3
%MW27: Lock the machine
