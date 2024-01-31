
all:	result.vcd
result.vcd:	gcd.vhdl	tb_gcd.vhdl
	ghdl	-a	-fsynopsys	gcd.vhdl
	ghdl	-a	tb_gcd.vhdl
	ghdl	-e	-fsynopsys fsmtb_gcd
	ghdl	-r	-fsynopsys fsmtb_gcd	--vcd=result.vcd	--stop-time=2000us
clean:
	rm	-rf	result.vcd
