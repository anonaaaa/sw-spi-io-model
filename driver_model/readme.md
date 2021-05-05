SPI driver model

### Files
- `driver_writeScript`: defines the `dr_write` function and related functions that issue write requests to the SPI controller according to the driver state.
- `driver_readScript`: defines the `dr_read` function and related functions that issue read requests to the SPI controller according to the driver state.
- `driver_checkScript`: defines the `dr_check` function and related funcions. It updates the driver state based on the reply from SPI hardware for previous read request.
- `driver_stateScript`: defines datatypes for the driver model.
- `driver_relationScript`: defines relations for driver model itself and the composed model of SPI hardware and driver.
