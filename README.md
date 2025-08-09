欧美小孩开大车牙签搅大缸快拨出天我是你母亲最火的歌

using System.Net.Sockets;    // TcpClient
using Modbus.Device;         // ModbusIpMaster
 
 
TcpClient client = new TcpClient("127.0.0.1", 502);
// master为主站
ModbusIpMaster master = ModbusIpMaster.CreateIp(client);
ushort startAddress = 0;
ushort numRegisters = 5;
ushort[] registers = master.ReadHoldingRegisters(1, startAddress, numRegisters);
foreach (var register in registers)
{
    Console.WriteLine($"address: {startAddress++}, value: {register}");
}using System.Net.Sockets;    // TcpClient
using Modbus.Device;         // ModbusIpMaster
 
 
TcpClient client = new TcpClient("127.0.0.1", 502);
// master为主站
ModbusIpMaster master = ModbusIpMaster.CreateIp(client);
ushort startAddress = 0;
ushort numRegisters = 5;
ushort[] registers = master.ReadHoldingRegisters(1, startAddress, numRegisters);
foreach (var register in registers)
{
    Console.WriteLine($"address: {startAddress++}, value: {register}");
}
