# Report

| Verified by | Date |
|:------------|:-----|
|`MS`|`11/7/25`|

## Speculation

> In your own words, describe what the 6522 tester code does.

The first set of 5 instructions turns on the 6522 (interface). The next set of five instructions latches the value 55 onto the 0x6000 address. The following set of five instructions latches the value aa onto the 0x6000 address. The next set of 3 instructions below loop back to the second set of 5 instructions.

> There are some addresses dedicated to using the interface. What are they and what do they seem to do?
> _HINT_: for this part, focus on the wiring of the _address bus lines_.

The addresses dedicated to using the interface are 0x6000 and 0x6002. 0x6002 sets up the interface so that we can use it. 0x6000 is the address you sent data to if you want to latch it.

> Why is creating specific, separate addresses important to achieve this function?

We would be unable to latch data if we did not create a separate address. Additionally, without 0x6002, we would be unable to use the interface.

> What is the value of the interface module (i.e. what does it _do_)?

It latches data! So it holds the most previous data inputted into the 0x6000 address. It "latches" AKA holds that data until it is overwritten. It is a way for the chip to communicate to us, to make reading it easier.

