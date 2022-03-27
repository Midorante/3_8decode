VERILOG = iverilog
TARGET = 3_8decode.vcd

$(TARGET) : 3_8decode.vvp
	vvp 3_8decode.vvp

3_8decode.vvp: 3_8decode_tb.v 3_8decode.v
	$(VERILOG) -o 3_8decode.vvp 3_8decode_tb.v 3_8decode.v

clean:
	-del $(TARGET)