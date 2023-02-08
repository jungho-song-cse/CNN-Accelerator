# CNN-Accelerator

# Requirements
* Verilog
* MATLAB (Only if you want to verify outputs)

# Files
<pre>
Bus Interface
|   ahb_bram.v
|   ahb_lite_input_stage.v
|   ahb_lite_interconnect.v
|   ahb_lite_transactor.v
|   ahb_master.v
|   amba_ahb_arbiter_h.v
|   amba_ahb_decoder.v
|   amba_ahb_decoder_h.v
|   amba_ahb_h.v
|   amba_ahb_lite_arbiter.v
|   amba_lite_output_stage.v
|   map.v
|   top_system.v
└─  top_system_tb.v
</pre>

<pre>
Convolution Neural Network Implementation
├─  Layers
|   |   act_shifter.v
|   |   bnorm_quant_act.v
|   |   bias_shifter.v
|   |   cnn_accel.v
|   └─  cnn_fsm.v
├─  Ram(+Buffer)
|   |   bram.v
|   |   dma2buf.v
|   |   spram.v
|   └─  dpram.v 
├─  MAC(Multiplier+Adder)
|   |   mac.v
|   |   mac_kern.v
|   |   conv_kern.v
|   └─  mul.v
└─  Image writer(Output)
    └─  bmp_image_writer.v
</pre>

<pre>
Output verifier
└─  check_hardware_results.m
</pre>


# RUN
Use HDL simulator such as ModelSim
