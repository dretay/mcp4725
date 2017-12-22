# MCP4725 for STM32


Invoke Like this:

```c
	uint8_t mcp4725_config_cnt = 2;
	MCP4725_CONFIG mcp4725_configs[mcp4725_config_cnt];
	mcp4725_configs[1].addr = 0xC4;
	mcp4725_configs[1].p_i2c = &hi2c2;
	mcp4725_configs[0].addr = 0xC6;
	mcp4725_configs[0].p_i2c = &hi2c2;

	MCP4725.configure(mcp4725_configs, mcp4725_config_cnt);	

```
