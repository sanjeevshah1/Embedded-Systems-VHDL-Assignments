all:	result.vcd

result.vcd:	twoToFourDecoder.vhdl	twoToFourDecoderTest.vhdl
	ghdl	-a	-fsynopsys	twoToFourDecoder.vhdl
	ghdl	-a	-fsynopsys	twoToFourDecoderTest.vhdl
	ghdl	-e	-fsynopsys	bench
	ghdl	-r	-fsynopsys	bench	--vcd=result.vcd
clean:
	rm	-rf	result.vcd
