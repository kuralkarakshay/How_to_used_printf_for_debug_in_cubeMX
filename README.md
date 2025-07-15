# How_to_used_printf_for_debug_in_cubeMX

int __io_putchar(int ch)
{
 // Write character to ITM ch.0
 ITM_SendChar(ch);
 //HAL_UART_Transmit(&huart2, (uint8_t *)&ch, 1, HAL_MAX_DELAY); // uncomment this line when you want to use this line printf function instead of the HAL_UART_Transmit
 return(ch);
}

when stm32 board is debug at that time printf() function is used 
