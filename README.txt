This is Library to interface I2C peripheral of avr microcontrollers.

Data Writing:
	To write data in particular register of slave, use function
		TWI_WriteRegister(uint8_t DeviceAdrr , uint8_t RegisterAdrr , uint8_t data)

Data Reading:
	To read data of any register of slave with Not-acknowledge, use function 
		TWI_ReadRegisterNACK(uint8_t DeviceAdrr , uint8_t RegisterAdrr)

	To read with acknowledge, use function
		TWI_ReadRegisterACK(uint8_t DeviceAdrr , uint8_t RegisterAdrr)
	For further reading use only
		TWI_ReadACK()
	And to send Nack at last use
		TWI_ReadNACK()

Detailed Specifications:
	Clock rate being used is 100 KHz which is typical for most of sensors.
	You can change it by defining F_SCL at desired frequency.
	All functions for reading data return data in 'unsigned char' data type.
	 
	
