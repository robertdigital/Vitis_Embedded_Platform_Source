OUTPUT=../platform_repo/tmp
HW_PATH=$(OUTPUT)/vivado
VIVADO=$(XILINX_VIVADO)/bin/vivado

all: hw

hw:
	mkdir -p $(HW_PATH)
	$(VIVADO) -mode batch -notrace -source $(PLATFORM)_xsa.tcl

clean:
	$(RM) -r vivado.* vivado_* ${PLATFORM}_vivado $(PLATFORM).xsa .Xil

