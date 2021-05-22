from machine import UART, Pin

uart = UART(1, baudrate=9600, tx=Pin(4), rx=Pin(5))
led = Pin(17, Pin.OUT)

while True:
    kod = uart.read(1)
    kod = kod.decode("utf-8")
    if kod == "1":
        led(1)
    elif kod == "2":
        led(0)
