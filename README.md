# Easy-AVR-USART-C-Library
easy to use C avr uart library


int main(void)
{
	uart0_init(BAUD_CALC(9600));
    sei();
    while(1)
    {
		uart_puts("hello world\r\n");
		_delay_ms(1000);
    }
}

gives

		   text	   data	    bss	    dec	    hex	filename
		    468	     14	     69	    551	    227	avrt.elf

Program Memory Usage 	:	482 bytes   1,5 % Full
Data Memory Usage 		:	83 bytes   4,1 % Full

defined  NO_USART_RX flag gives

		   text	   data	    bss	    dec	    hex	filename
		    390	     14	     35	    439	    1b7	avrt.elf

Program Memory Usage 	:	404 bytes   1,2 % Full
Data Memory Usage 		:	49 bytes   2,4 % Full