all:	result.vcd
result.vcd:	lcm.vhdl	tb_lcm.vhdl
	ghdl	-a	-fsynopsys	lcm.vhdl
	ghdl	-a	tb_lcm.vhdl
	ghdl	-e	-fsynopsys fsmtb_lcm
	ghdl	-r	-fsynopsys fsmtb_lcm	--vcd=result.vcd	--stop-time=20us
clean:
	rm	-rf	result.vcd
