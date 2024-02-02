
all:	result.vcd
result.vcd:	counter.vhdl	tb_counter.vhdl
	ghdl	-a	-fsynopsys	counter.vhdl
	ghdl	-a	tb_counter.vhdl
	ghdl	-e	-fsynopsys tb_counter
	ghdl	-r	-fsynopsys tb_counter	--vcd=result.vcd	--stop-time=20us
clean:
	rm	-rf	result.vcd
