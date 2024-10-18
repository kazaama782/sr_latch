# sr_latch


`timescale 1ns / 1ps


module sr_latch(q,qbar,s,r);
input s,r;
output q,qbar;
assign q = ~(qbar&r);
assign qbar = ~(q&s);
endmodule
