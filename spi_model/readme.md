SPI hardware model

### Files
- `board_memScript.sml`: defines physical addresses of SPI registers and board RAM region.
- `SPI_stateScript.sml`: defines the datatypes for SPI controller. Basiclly, the SPI controller model includes SPI registers, an error flag, and a general state includes init, tx, rx, and xfer automatons.
- `SPI_update_regsScript.sml`: describes how SPI controller updates its states and regs according to driver-issued PA and Val.
- `SPI_return_regsScript.sml`: describes how SPI controller returns a value if the driver issues a read request to memory-mapped register.
- `SPI_tauScript.sml`: defines functions of SPI controller internal operation for init, tx, rx and xfer automatons.
- `SPI_data_trScript.sml`: shows the SPI hardware model's interface to transfer data with three different modes, including TX, RX (both half-duplex) and XFER (full-duplex).
- `SPI_relationScript.sml`: define SPI controller labeled state transition relation `spi_tr`.
