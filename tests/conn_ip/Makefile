APPLICATION = conn_ip
include ../Makefile.tests_common

BOARD_INSUFFICIENT_MEMORY := chronos msb-430 msb-430h nucleo32-f031 nucleo32-f042 \
                             nucleo32-l031 nucleo-f030 nucleo-f070 nucleo-f334 nucleo-l053 \
                             stm32f0discovery telosb weio wsn430-v1_3b wsn430-v1_4 \
                             z1

USEMODULE += gnrc_netdev_default
USEMODULE += auto_init_gnrc_netif
USEMODULE += gnrc_icmpv6_echo
USEMODULE += gnrc_ipv6_default
USEMODULE += gnrc_conn_ip
USEMODULE += od
USEMODULE += shell
USEMODULE += shell_commands
USEMODULE += ps

include $(RIOTBASE)/Makefile.include

test:
	./tests/01-run.py
